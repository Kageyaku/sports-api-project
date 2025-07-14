<?php
function fetchAPIData($url) {
    $curl = curl_init();
    curl_setopt_array($curl, [
        CURLOPT_RETURNTRANSFER => true,
        CURLOPT_URL => $url,
        CURLOPT_SSL_VERIFYPEER => false,
        CURLOPT_CONNECTTIMEOUT => 10,
    ]);

    $response = curl_exec($curl);
    $error = curl_error($curl);
    curl_close($curl);

    return $error ? false : $response;
}

// ✅ Premier League upcoming events (max 15)
$apiUrl = "https://www.thesportsdb.com/api/v1/json/123/eventsnextleague.php?id=4328";
$json = fetchAPIData($apiUrl);
$data = $json ? json_decode($json, true) : null;
$events = $data['events'] ?? [];
?>
<!DOCTYPE html>
<html>
<head>
    <title>Football Game Schedules</title>
    <style>
        body { font-family: Arial, sans-serif; padding: 20px; }
        h1 { color: #003366; }
        table { border-collapse: collapse; width: 100%; margin-top: 20px; }
        th, td { border: 1px solid #ccc; padding: 8px; text-align: left; }
    </style>
</head>
<body>
    <h1>Football Game Schedules</h1>

    <!-- ✅ Keep only this link -->
    <a href="api_view.php">View Teams</a>

    <h2>Upcoming Premier League Matches</h2>

    <?php if (empty($events)): ?>
        <p style="color:red;">⚠️ No events found or failed to fetch from API.</p>
    <?php else: ?>
        <table>
            <tr>
                <th>Date</th>
                <th>Time</th>
                <th>Match</th>
                <th>Venue</th>
                <th>Status</th>
            </tr>
            <?php foreach ($events as $event): ?>
                <tr>
                    <td><?= $event['dateEvent'] ?? 'N/A' ?></td>
                    <td><?= $event['strTime'] ?? 'N/A' ?></td>
                    <td><?= $event['strEvent'] ?? 'N/A' ?></td>
                    <td><?= $event['strVenue'] ?? 'N/A' ?></td>
                    <td><?= $event['strStatus'] ?? 'Upcoming' ?></td>
                </tr>
            <?php endforeach; ?>
        </table>
    <?php endif; ?>
</body>
</html>
