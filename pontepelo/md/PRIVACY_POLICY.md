# Privacy Policy

Last updated: July 16, 2026

This Privacy Policy explains how PontePelo handles information processed by its backend services.

## Information We Process

The backend may process information needed to provide the app experience, including:

- Uploaded or selected photos used for hairstyle previews or related features.
- Hairstyle, catalog, task, and generation metadata.
- Account or authentication identifiers when required by Firebase or backend access controls.
- Technical information such as request timestamps, service logs, error logs, device or browser metadata, and API usage data.

## Face Data and Selfie Photos

PontePelo lets users take or select a selfie/photo to preview AI-generated hairstyles. These photos may contain a user's face. We do not use the photo to identify the user, authenticate the user, track the user, build a face recognition profile, create a biometric identifier, or determine identity.

We collect and process the selected photo only to generate hairstyle preview images requested by the user. The app may process facial appearance visible in the photo, such as face shape, head position, skin tone, and hair/scalp area, only as needed to produce the hairstyle preview.

The selected photo is sent to our backend and to Vast.ai rented GPU instances used for AI image generation. The backend does not intentionally store the original selected selfie/photo in Google Cloud Storage. Vast.ai GPU instances process the photo and may temporarily store workflow input/output artifacts because the generation workflow is asynchronous and uses image output nodes. These temporary files are automatically removed from the Vast.ai instance after 30 days.

Generated hairstyle result images may be stored in Google Cloud Storage under per-task paths so the app can retrieve completed asynchronous results. Firestore stores task metadata and storage references, such as task status and generated image paths, but not the original selected selfie/photo.

We do not sell face data and do not share it with advertisers, data brokers, or third parties for identification, tracking, or advertising.

On the device, the selected photo and generated images may be stored locally so the user can view current and previous try-ons. Users can delete generated try-on tasks/images in the app. Deletion removes the local copy on the device and requests deletion of the related async generation task/result data. Backend logs and security/usage records may be retained for operational, security, abuse-prevention, or legal purposes, but are not used to identify users by face.

## How We Use Information

We use information to:

- Provide hairstyle simulation, image generation, catalog, and administrative features.
- Return and display user-requested hairstyle preview results.
- Operate, debug, secure, and improve backend services.
- Prevent abuse, unauthorized access, and service misuse.

## Image and Generated Content

Photos and generated images may be processed by Vast.ai rented GPU instances used by the service. Images should only be uploaded when you have the right to use them and when the person shown has consented where required.

## Service Providers

The backend may rely on providers such as cloud hosting, Firebase, logging, and Vast.ai rented GPU instances for AI generation. These providers process information only as needed to deliver their services to PontePelo.

## Data Retention

User-selected face photos and generated user result images may be stored locally on the user's device until the user deletes them, clears app data, or uninstalls the app. Vast.ai workflow input/output artifacts are automatically removed from the Vast.ai instance after 30 days. Generated result images stored in Google Cloud Storage are retained so the app can retrieve asynchronous results and are deleted when the user deletes the related try-on task/image in the app. Task metadata, logs, and security/usage records may be retained as long as needed for app functionality, operations, legal obligations, security, abuse prevention, or legitimate business purposes.

## Security

We use reasonable technical and organizational safeguards to protect information. No system is completely secure, and users should avoid uploading sensitive or unnecessary personal information.

## User Choices

Users may request deletion or correction of personal information where applicable. Some data may need to be retained for security, legal, or operational reasons.

## Children's Privacy

The service is not intended for children under the age required by applicable law. Children should not use the service without appropriate parental or guardian consent.

## Changes

We may update this Privacy Policy as the service evolves. Updated versions will replace this document and include a new effective date.

## Contact

For privacy questions or requests, contact the PontePelo project owner or administrator.
