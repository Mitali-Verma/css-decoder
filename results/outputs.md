============================================================
=== STAGE 1: Learn H ===
============================================================
Learning H with n=70, budget=2000
Phase 1: Learning HX (querying 70 basis vectors)...
Phase 2: Learning HZ (querying 70 basis vectors)...
✅ CSS commutation validated
✅ Stage 1 complete: learned H ((30, 140)) using 140 queries
HX shape: (15, 70), HZ shape: (15, 70)
rank(HX) = 15, dim(null(HX)) = 55
rank(HZ) = 15, dim(null(HZ)) = 55

Searching for minimum distance (sampling 10000 operators)...
  Attempt 0: found operator with weight 64
✅ Distance estimate: d ≈ 46

✅ Stage 1 Score: 35.0/40
Details: {'base_score': 35.0, 'bonus_score': 0.0, 'css_commutation_valid': True, 'd_bonus_feedback': 'Distance estimate d=46 received (bonus evaluation requires true d)', 'd_estimate': 46, 'mX_cand': 15, 'mX_hidden': 15, 'mZ_cand': 15, 'mZ_hidden': 15, 'n': 70, 'rankX_cand': 15, 'rankX_hidden': 15, 'rankZ_cand': 15, 'rankZ_hidden': 15}

============================================================
=== STAGE 2: Decode (clean) ===
============================================================
  Test 1: Score 42.3/45
  Test 2: Score 42.3/45
  Test 3: Score 42.6/45
  Test 4: Score 42.6/45
  Test 5: Score 42.4/45

✅ Stage 2 Average: 42.5/45

============================================================
=== STAGE 3: Decode (noisy, redundant) ===
============================================================
Redundancy: r = 5

  Test 1: Query ID = e66bdcd8...
Base syndrome size: 30
Extended syndrome size: 35
Redundancy r: 5
Bits flipped by denoising: 16/30
Estimated noise rate: 0.5333
  Score: 0.0/30

  Test 2: Query ID = e6a93abb...
Base syndrome size: 30
Extended syndrome size: 35
Redundancy r: 5
Bits flipped by denoising: 18/30
Estimated noise rate: 0.6000
  Score: 0.0/30

  Test 3: Query ID = 8f4e2449...
Base syndrome size: 30
Extended syndrome size: 35
Redundancy r: 5
Bits flipped by denoising: 16/30
Estimated noise rate: 0.5333
  Score: 0.0/30

✅ Stage 3 Average: 0.0/30

============================================================
TOTAL ESTIMATED SCORE: 77.5/115
============================================================