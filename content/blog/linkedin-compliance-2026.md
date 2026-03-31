---
title: "Your LinkedIn Profile Is Training the Algorithm That Will Score You"
date: 2026-03-31
tags: ["Compliance", "EU AI Act", "Privacy Engineering"]
summary: "The EU AI Act's enforcement deadline is August 2026. LinkedIn defaults your profile into AI training. That AI scores candidates. Here's what that means for engineers in regulated sectors."
---

The EU AI Act's enforcement deadline is August 2026. That's five months away.

LinkedIn's default setting opts your profile data into AI training. That AI scores candidates. Right now, you're contributing training data to the same model that will assess you for your next role.

That's not speculation. It's in LinkedIn's privacy settings, and it's on a collision course with EU law.

## The Consent Problem

GDPR requires "freely given" consent for personal data processing. An opt-out model doesn't meet that bar for sensitive processing. Recruitment AI sits squarely in the sensitive category.

The EU AI Act classifies candidate-scoring systems as high-risk under Annex III. High-risk systems face strict rules around training data quality, bias auditing and transparency. When enforcement begins in August, platforms won't be able to rely on opt-out consent for this kind of processing.

A platform using opt-out consent to train high-risk AI is a compliance problem. Enforcement actions are being prepared now.

<div style="margin: 2.5rem 0; border: 1px solid hsl(var(--border-color)); background: hsl(var(--bg-card)); border-radius: 4px; overflow: hidden;">
  <div style="padding: 1rem 1.5rem; border-bottom: 1px solid hsl(var(--border-color));">
    <span style="font-family: 'JetBrains Mono', monospace; font-size: 0.65rem; text-transform: uppercase; letter-spacing: 0.12em; color: hsl(var(--text-secondary)); opacity: 0.8;">The Training Loop</span>
  </div>
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));">
    <div style="padding: 1.5rem; border-right: 1px solid hsl(var(--border-color));">
      <div style="font-family: 'JetBrains Mono', monospace; font-size: 0.65rem; opacity: 0.4; margin-bottom: 0.75rem;">01</div>
      <div style="font-weight: 700; font-size: 1rem; line-height: 1.3; margin-bottom: 0.5rem;">Your LinkedIn Profile</div>
      <div style="font-size: 0.8rem; color: hsl(var(--text-secondary));">Public. Detailed. Default opt-in to AI training.</div>
    </div>
    <div style="padding: 1.5rem; border-right: 1px solid hsl(var(--border-color));">
      <div style="font-family: 'JetBrains Mono', monospace; font-size: 0.65rem; opacity: 0.4; margin-bottom: 0.75rem;">02</div>
      <div style="font-weight: 700; font-size: 1rem; line-height: 1.3; margin-bottom: 0.5rem;">AI Training Data Pool</div>
      <div style="font-size: 0.8rem; color: hsl(var(--text-secondary));">Your work history, skills, and tenure ingested.</div>
    </div>
    <div style="padding: 1.5rem; border-right: 1px solid hsl(var(--border-color));">
      <div style="font-family: 'JetBrains Mono', monospace; font-size: 0.65rem; opacity: 0.4; margin-bottom: 0.75rem;">03</div>
      <div style="font-weight: 700; font-size: 1rem; line-height: 1.3; margin-bottom: 0.5rem;">Candidate Scoring Model</div>
      <div style="font-size: 0.8rem; color: hsl(var(--text-secondary));">Trained on profiles like yours.</div>
    </div>
    <div style="padding: 1.5rem; border-left: 3px solid hsl(var(--text-primary) / 0.4);">
      <div style="font-family: 'JetBrains Mono', monospace; font-size: 0.65rem; opacity: 0.4; margin-bottom: 0.75rem;">04</div>
      <div style="font-weight: 700; font-size: 1rem; line-height: 1.3; margin-bottom: 0.5rem;">Your Application Scored</div>
      <div style="font-size: 0.8rem; color: hsl(var(--text-secondary));">No visibility into the result. No right of explanation.</div>
    </div>
  </div>
  <div style="padding: 1rem 1.5rem; border-top: 1px dashed hsl(var(--border-color)); font-family: 'JetBrains Mono', monospace; font-size: 0.75rem; color: hsl(var(--text-secondary));">
    ↩ Step 04 feeds back into model retraining. Your future applications are scored by a model your past profiles helped build.
  </div>
</div>

The circular nature of this is worth sitting with. You don't know what weight the model gives your profile history. An old job title might be penalising you. You'd have no way of knowing.

## The FCA Angle

This one's specific to engineers in financial services, but it's worth knowing.

The FCA's Non-Financial Misconduct rules come into force in September 2026. These will allow fitness and propriety assessments to include behaviour outside the workplace. That includes social media activity.

A heated comment thread. An old post taken out of context. Either of these could feed into a conduct review for senior engineers at regulated firms.

Most engineers in Fintech don't know this is coming. Most compliance teams are still working out how to apply it. But it's in the rules, and it goes live in six months.

## The Engineering Alternative

The platform-sovereign model is LinkedIn's default. Your data lives in their database. They decide who accesses it, how it's processed and what it trains.

The alternative is Self-Sovereign Identity. The idea has been around for years. The infrastructure is now close enough to matter.

<div style="margin: 2.5rem 0; overflow-x: auto;">
  <table style="width: 100%; border-collapse: collapse; font-size: 0.875rem;">
    <thead>
      <tr>
        <th style="padding: 0.875rem 1rem; text-align: left; font-family: 'JetBrains Mono', monospace; font-size: 0.65rem; text-transform: uppercase; letter-spacing: 0.1em; font-weight: 600; border-bottom: 2px solid hsl(var(--border-color)); color: hsl(var(--text-secondary));"></th>
        <th style="padding: 0.875rem 1rem; text-align: left; font-family: 'JetBrains Mono', monospace; font-size: 0.65rem; text-transform: uppercase; letter-spacing: 0.1em; font-weight: 600; border-bottom: 2px solid hsl(var(--border-color)); color: hsl(var(--text-secondary));">Platform-Sovereign<br>(LinkedIn)</th>
        <th style="padding: 0.875rem 1rem; text-align: left; font-family: 'JetBrains Mono', monospace; font-size: 0.65rem; text-transform: uppercase; letter-spacing: 0.1em; font-weight: 600; border-bottom: 2px solid hsl(var(--border-color)); color: hsl(var(--text-secondary));">Self-Sovereign Identity</th>
      </tr>
    </thead>
    <tbody>
      <tr style="border-bottom: 1px solid hsl(var(--border-color));">
        <td style="padding: 0.875rem 1rem; font-family: 'JetBrains Mono', monospace; font-size: 0.75rem; color: hsl(var(--text-secondary));">Data location</td>
        <td style="padding: 0.875rem 1rem;">LinkedIn's servers</td>
        <td style="padding: 0.875rem 1rem; font-weight: 600;">Your identity wallet</td>
      </tr>
      <tr style="border-bottom: 1px solid hsl(var(--border-color)); background: hsl(var(--bg-card));">
        <td style="padding: 0.875rem 1rem; font-family: 'JetBrains Mono', monospace; font-size: 0.75rem; color: hsl(var(--text-secondary));">Access control</td>
        <td style="padding: 0.875rem 1rem;">LinkedIn decides</td>
        <td style="padding: 0.875rem 1rem; font-weight: 600;">You grant, you revoke</td>
      </tr>
      <tr style="border-bottom: 1px solid hsl(var(--border-color));">
        <td style="padding: 0.875rem 1rem; font-family: 'JetBrains Mono', monospace; font-size: 0.75rem; color: hsl(var(--text-secondary));">Recruiter visibility</td>
        <td style="padding: 0.875rem 1rem;">Always on, searchable by anyone</td>
        <td style="padding: 0.875rem 1rem; font-weight: 600;">On request only</td>
      </tr>
      <tr style="border-bottom: 1px solid hsl(var(--border-color)); background: hsl(var(--bg-card));">
        <td style="padding: 0.875rem 1rem; font-family: 'JetBrains Mono', monospace; font-size: 0.75rem; color: hsl(var(--text-secondary));">Third-party scrapers</td>
        <td style="padding: 0.875rem 1rem;">Can access freely</td>
        <td style="padding: 0.875rem 1rem; font-weight: 600;">Blocked by design</td>
      </tr>
      <tr style="border-bottom: 1px solid hsl(var(--border-color));">
        <td style="padding: 0.875rem 1rem; font-family: 'JetBrains Mono', monospace; font-size: 0.75rem; color: hsl(var(--text-secondary));">AI training</td>
        <td style="padding: 0.875rem 1rem;">Default opt-in</td>
        <td style="padding: 0.875rem 1rem; font-weight: 600;">Not applicable</td>
      </tr>
      <tr>
        <td style="padding: 0.875rem 1rem; font-family: 'JetBrains Mono', monospace; font-size: 0.75rem; color: hsl(var(--text-secondary));">Proof of claims</td>
        <td style="padding: 0.875rem 1rem;">Self-reported, unverified</td>
        <td style="padding: 0.875rem 1rem; font-weight: 600;">Cryptographically signed by issuer</td>
      </tr>
    </tbody>
  </table>
</div>

Zero-Knowledge Proofs are the key mechanism here. A ZKP lets you prove a claim is true without revealing the underlying data. You can prove you have five years of Kubernetes experience without exposing your full employment history.

Verifiable Credentials work the same way. Your work history becomes a set of cryptographically signed statements. Each one is issued by the relevant employer or institution. You hold them in a wallet and present only what a specific role requires.

## What's Coming in 2026

This isn't theoretical. Three concrete regulatory shifts are landing this year.

<div style="margin: 2.5rem 0; padding-left: 2rem; border-left: 2px solid hsl(var(--border-color)); position: relative;">

  <div style="position: relative; margin-bottom: 0.5rem;">
    <div style="position: absolute; left: -2.45rem; top: 0.35rem; width: 10px; height: 10px; border-radius: 50%; background: hsl(var(--text-secondary)); opacity: 0.4;"></div>
    <div style="font-family: 'JetBrains Mono', monospace; font-size: 0.7rem; color: hsl(var(--text-secondary)); opacity: 0.6;">March 2026 — Now</div>
  </div>
  <div style="margin-bottom: 2.5rem; padding: 1rem; border: 1px dashed hsl(var(--border-color)); font-size: 0.85rem; color: hsl(var(--text-secondary));">
    LinkedIn's AI training opt-out is active but unenforced. GDPR challenges are in progress. The window to act before enforcement is now.
  </div>

  <div style="position: relative; margin-bottom: 0.5rem;">
    <div style="position: absolute; left: -2.45rem; top: 0.35rem; width: 10px; height: 10px; border-radius: 50%; background: hsl(var(--text-primary));"></div>
    <div style="font-family: 'JetBrains Mono', monospace; font-size: 0.7rem; color: hsl(var(--text-secondary));">August 2026</div>
  </div>
  <div style="margin-bottom: 0.5rem; font-weight: 700; font-size: 1.1rem;">EU AI Act enforcement begins</div>
  <div style="margin-bottom: 2.5rem; font-size: 0.9rem; color: hsl(var(--text-secondary));">Recruitment and candidate-scoring AI is classified as high-risk under Annex III. Platforms must document training data sources, conduct bias audits and provide transparency reports. Opt-out consent won't satisfy the requirements for high-risk AI systems.</div>

  <div style="position: relative; margin-bottom: 0.5rem;">
    <div style="position: absolute; left: -2.45rem; top: 0.35rem; width: 10px; height: 10px; border-radius: 50%; background: hsl(var(--text-primary));"></div>
    <div style="font-family: 'JetBrains Mono', monospace; font-size: 0.7rem; color: hsl(var(--text-secondary));">September 2026</div>
  </div>
  <div style="margin-bottom: 0.5rem; font-weight: 700; font-size: 1.1rem;">FCA Non-Financial Misconduct rules</div>
  <div style="margin-bottom: 2.5rem; font-size: 0.9rem; color: hsl(var(--text-secondary));">Fitness and propriety assessments for certified persons at regulated firms can include behaviour outside the workplace. Social media activity is explicitly in scope. This applies to senior and certified roles in UK financial services.</div>

  <div style="position: relative; margin-bottom: 0.5rem;">
    <div style="position: absolute; left: -2.45rem; top: 0.35rem; width: 10px; height: 10px; border-radius: 50%; background: hsl(var(--text-primary));"></div>
    <div style="font-family: 'JetBrains Mono', monospace; font-size: 0.7rem; color: hsl(var(--text-secondary));">Late 2026</div>
  </div>
  <div style="margin-bottom: 0.5rem; font-weight: 700; font-size: 1.1rem;">eIDAS 2.0 Digital Identity Wallet mandate</div>
  <div style="font-size: 0.9rem; color: hsl(var(--text-secondary));">Large employers in Europe must accept the EU Digital Identity Wallet for onboarding. Government-backed, privacy-first identity verification without a platform intermediary. This is what makes the LinkedIn-less engineer a normal thing rather than a suspicious gap.</div>

</div>

## What to Do Now

You don't need to delete your account. A ghost profile works fine: your name, your title, a link to your personal site. Notifications off. No activity required.

The substantive version of your professional identity should live somewhere you control. A personal site with a genuine technical perspective does more for credibility in regulated sectors than a well-maintained feed.

If you're in a regulated firm, check whether your social media activity is covered under your firm's conduct policy. Most policies haven't been updated to reflect the FCA rules coming in September, and most engineers haven't been told to check.

The compliance surface for engineers is getting broader. Worth knowing where you stand before August.
