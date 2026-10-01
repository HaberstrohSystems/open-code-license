# Open Code License (OCL)

A license for proprietary software that customers can fully inspect. Customers receive the complete source code, may audit it and change it for their own use, and may not publish it, pass it on or sell it.

> **Version 1.0.** Written and checked by its authors, not by a lawyer. See [Not legal advice](#not-legal-advice).

The license text is in [open-code-license-1.0.md](open-code-license-1.0.md).

## At a glance

| Customers may | Customers may not |
| --- | --- |
| Read, review and audit the full source code | Publish the code or their modified versions |
| Run the software for their own business | Give, sell, rent or sublicense it to anyone else |
| Modify it for their own use | Modify it for others |
| Let contractors, auditors and hosting providers work with it for them; these are bound by the license directly | Host it for others, or offer it to others as a service |
| Say publicly what they think of its security and quality | Copy parts of it into products or services they offer |
| Publish vulnerabilities after reporting them (fix released, or 90 days) | Remove license keys or exceed the licensed scope |

The table is a summary. Only the license text is binding.

One limit comes from the law, not from the license: resale can only be ruled out for licenses that run for a limited term, such as subscriptions. Where a customer has paid once for a perpetual license, the law in some places, the EU among them, lets them resell their copy. Section 11.1 sets the conditions for that case.

## Why another license

Source-available licenses exist, but they are written for code that is published to everyone. The Open Code License is written for code that is handed to customers only.

| | OCL 1.0 | PolyForm Internal Use 1.0.0 | Elastic License 2.0 | Business Source License 1.1 |
| --- | --- | --- | --- | --- |
| Who gets rights | Customers with a contract | Anyone who has the code | Anyone who has the code | Anyone who has the code |
| Modify for own use | Yes | Yes | Yes | Yes, but production use only as far as the licensor allows |
| Redistribute | No | No | Yes | Yes |
| Source code stays confidential | Yes | No | No | No |
| Stated right to publish audit findings and vulnerabilities | Yes | No | No | No |
| Warranty and liability | Left to the customer contract. Where the contract is silent: full liability for intent, gross negligence and personal injury; otherwise only for breach of fundamental obligations and for foreseeable damage | "As is", no liability | "As is", no liability | "As is" |

## Using it

The license can be used in two ways.

**On its own.** The whole product is under the Open Code License.

**For an extension of an open-core program.** The core stays under its open source license, whichever one that is. The extension connects to the core through the core's extension interface and is under the Open Code License. Everything that is marked as having license terms of its own keeps them (section 2.3), so mark the core and every other open source part clearly.

```text
core/        open source license of the core
extension/   Open Code License 1.0   (customers only)
```

In both cases:

1. Put the license text and a completed license notice (see the end of the license) next to the code the license covers.
2. Mark each file the license covers:

   ```text
   // Copyright (c) 2026 Example Inc.
   // SPDX-License-Identifier: LicenseRef-OCL-1.0
   // Provided to customers under the Open Code License 1.0. Not for publication or redistribution.
   ```

3. Reference the license in your customer contract or order form, and give the customer the text before the contract is concluded. Without that reference the license is not part of the contract and does not bind the customer. The contract sets price, scope of use, term, support and warranty; the license sets what the customer may do with the code. Link to the tagged version, which does not change: <https://github.com/HaberstrohSystems/open-code-license/blob/v1.0/open-code-license-1.0.md>

For an extension, read the license of the core first. Open source licenses differ in what they ask of software that is connected to the core: some only require that their notices are kept, others require that works based on the core carry the same license. Whether your extension is a separate work depends on that license and on how the extension is coupled to the core.

## Reusing the license

Anyone may use this license for their own software. If you change the text, give it a different name.

## Not legal advice

The license was written and checked by its authors to the best of their knowledge. It has not been reviewed by a lawyer, and nothing in this repository is legal advice. If you use the license, you do so at your own risk; whether it fits your product, your contracts and your jurisdiction is for you to check.
