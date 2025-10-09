<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Yearly Crime Trend - Dashboard</title>
    <script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.3/dist/chart.umd.min.js"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        
        * { margin: 0; padding: 0; box-sizing: border-box; }
        
        body { 
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #333;
            min-height: 100vh;
        }
        
        /* Navbar */
        /* FIXED NAVBAR CSS - Replace the navbar/dropdown CSS in ALL your HTML files with this */

.navbar { 
    display: flex; 
    justify-content: space-between; 
    align-items: center; 
    background: rgba(26, 35, 126, 0.95);
    backdrop-filter: blur(10px);
    padding: 16px 40px;
    color: white;
    box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
    position: sticky;
    top: 0;
    z-index: 100;
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.navbar h1 { 
    margin: 0;
    font-size: 26px;
    font-weight: 700;
    letter-spacing: -0.5px;
    background: linear-gradient(135deg, #ffffff 0%, #a5d6a7 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.nav-links { 
    display: flex; 
    gap: 30px; 
    align-items: center; 
}

.nav-links a { 
    color: rgba(255, 255, 255, 0.9);
    text-decoration: none;
    font-size: 15px;
    font-weight: 500;
    transition: all 0.3s ease;
    padding: 8px 16px;
    border-radius: 8px;
}

.nav-links a:hover { 
    color: #a5d6a7;
    background: rgba(255, 255, 255, 0.1);
    transform: translateY(-2px);
}

.nav-links .active {
    color: #a5d6a7;
    background: rgba(165, 214, 167, 0.15);
    font-weight: 600;
}

/* FIXED DROPDOWN - This is the key fix */
.dropdown { 
    position: relative; 
    display: inline-block;
}

/* Invisible bridge to prevent dropdown from closing */
.dropdown::before {
    content: '';
    position: absolute;
    top: 100%;
    left: 0;
    right: 0;
    height: 10px; /* Creates a bridge between button and menu */
    background: transparent;
}

.dropbtn { 
    background: none;
    border: none;
    color: rgba(255, 255, 255, 0.9);
    font-size: 15px;
    font-weight: 500;
    cursor: pointer;
    padding: 8px 16px;
    border-radius: 8px;
    transition: all 0.3s ease;
}

.dropbtn:hover {
    background: rgba(255, 255, 255, 0.1);
    color: #a5d6a7;
}

.dropdown-content { 
    display: none;
    position: absolute;
    background: white;
    min-width: 220px;
    box-shadow: 0 12px 48px rgba(0, 0, 0, 0.15);
    z-index: 10;
    right: 0;
    border-radius: 12px;
    overflow: hidden;
    margin-top: 8px; /* Gap between button and dropdown */
    animation: slideDown 0.3s ease;
}

@keyframes slideDown {
    from { opacity: 0; transform: translateY(-10px); }
    to { opacity: 1; transform: translateY(0); }
}

.dropdown-content a { 
    color: #333;
    padding: 14px 20px;
    text-decoration: none;
    display: block;
    font-size: 14px;
    font-weight: 500;
    transition: all 0.2s ease;
}

.dropdown-content a:hover { 
    background: #f5f7fa;
    padding-left: 24px;
}

.dropdown-content .active-dropdown {
    background: #e8f5e9;
    color: #1a237e;
    font-weight: 600;
}

/* Show dropdown on hover */
.dropdown:hover .dropdown-content { 
    display: block; 
}

/* Responsive */
@media (max-width: 768px) {
    .navbar {
        flex-direction: column;
        gap: 16px;
        padding: 16px 20px;
    }
    
    .navbar h1 {
        font-size: 22px;
    }
    
    .nav-links {
        flex-wrap: wrap;
        justify-content: center;
        gap: 12px;
    }
}
        
        /* Dashboard Container */
        .dashboard-container { 
            padding: 40px 20px;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .chart-card {
            background: white;
            padding: 40px;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.1);
            margin-bottom: 30px;
        }
        
        .chart-area { 
            height: 500px;
            position: relative;
        }
        
        h2 { 
            color: #1a237e;
            padding-bottom: 16px;
            margin-bottom: 32px;
            font-size: 28px;
            font-weight: 700;
            text-align: center;
            border-bottom: 4px solid #a5d6a7;
            position: relative;
        }
        
        h2::after {
            content: '';
            position: absolute;
            bottom: -4px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: #1a237e;
        }
        
        .chart-description {
            text-align: center;
            margin-top: 24px;
            padding: 20px;
            background: #f8f9fa;
            border-radius: 12px;
            font-size: 15px;
            color: #666;
            line-height: 1.6;
        }
        
        /* Stats Cards */
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }
        
        .stat-card {
            background: white;
            padding: 24px;
            border-radius: 16px;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.08);
            text-align: center;
            border-top: 4px solid #d32f2f;
            transition: all 0.3s ease;
        }
        
        .stat-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 12px 40px rgba(0, 0, 0, 0.12);
        }
        
        .stat-label {
            font-size: 13px;
            color: #666;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            font-weight: 600;
            margin-bottom: 8px;
        }
        
        .stat-value {
            font-size: 32px;
            font-weight: 700;
            color: #1a237e;
        }
        
        .stat-change {
            font-size: 14px;
            margin-top: 8px;
            padding: 4px 12px;
            border-radius: 20px;
            display: inline-block;
        }
        
        .stat-change.decrease {
            background: #e8f5e9;
            color: #2e7d32;
        }
        
        .stat-change.increase {
            background: #ffebee;
            color: #c62828;
        }
        
        @media (max-width: 768px) {
            .navbar {
                flex-direction: column;
                gap: 16px;
                padding: 16px 20px;
            }
            
            .navbar h1 {
                font-size: 22px;
            }
            
            .nav-links {
                flex-wrap: wrap;
                justify-content: center;
                gap: 12px;
            }
            
            .chart-card {
                padding: 24px;
            }
            
            .chart-area {
                height: 350px;
            }
            
            h2 {
                font-size: 22px;
            }
        }
    </style>
</head>
<body>
    <div class="navbar">
        <h1>Smart Crime Analytics Dashboard</h1>
        <div class="nav-links">
            <a href="index.html">Home</a>
            <div class="dropdown">
                <button class="dropbtn">Analytics ▼</button>
                <div class="dropdown-content">
                    <a href="yearly_trend.html" class="active-dropdown">Crime Trend (Yearly)</a>
                    <a href="top_crimes.html">Top Crime Types</a>
                    <a href="top_cities.html">City Hotspots</a>
                    <a href="district_analysis.html">District Analysis</a> 
                </div>
            </div>
            <a href="about.html">About</a>
        </div>
    </div>

    <div class="dashboard-container">
        <div class="stats-grid">
            <div class="stat-card">
                <div class="stat-label">2019 Total</div>
                <div class="stat-value">38,645</div>
            </div>
            <div class="stat-card">
                <div class="stat-label">2020 Total</div>
                <div class="stat-value">31,325</div>
                <div class="stat-change decrease">↓ 18.9%</div>
            </div>
            <div class="stat-card">
                <div class="stat-label">2021 Total</div>
                <div class="stat-value">35,572</div>
                <div class="stat-change increase">↑ 13.6%</div>
            </div>
        </div>

        <div class="chart-card">
            <h2>Violent Crime Trend in Metropolitan Cities (2019 - 2021)</h2>
            <div class="chart-area">
                <canvas id="yearlyTrendChart"></canvas>
            </div>
            <div class="chart-description">
                📊 This chart tracks the total number of violent incidents reported across the 19 major metropolitan cities over a three-year period. Note the significant decrease in 2020 followed by a partial recovery in 2021.
            </div>
        </div>
    </div>

    <script>
        const yearlyTrendData = [
            { year: 2019, count: 38645 },
            { year: 2020, count: 31325 },
            { year: 2021, count: 35572 }
        ];

        function renderChart() {
            const yearlyTrend = yearlyTrendData.sort((a, b) => a.year - b.year);
            const labels = yearlyTrend.map(y => y.year);
            const dataCounts = yearlyTrend.map(y => y.count);

            const trendCtx = document.getElementById('yearlyTrendChart').getContext('2d');
            
            new Chart(trendCtx, {
                type: 'line',
                data: {
                    labels: labels,
                    datasets: [{
                        label: 'Total Violent Incidents',
                        data: dataCounts,
                        borderColor: '#d32f2f',
                        backgroundColor: 'rgba(211, 47, 47, 0.1)',
                        fill: true,
                        tension: 0.4,
                        borderWidth: 3,
                        pointRadius: 6,
                        pointHoverRadius: 8,
                        pointBackgroundColor: '#d32f2f',
                        pointBorderColor: '#fff',
                        pointBorderWidth: 2
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    interaction: {
                        intersect: false,
                        mode: 'index'
                    },
                    scales: {
                        y: { 
                            beginAtZero: true,
                            grid: {
                                color: 'rgba(0, 0, 0, 0.05)'
                            },
                            ticks: {
                                font: {
                                    size: 13
                                },
                                callback: function(value) {
                                    return value.toLocaleString();
                                }
                            },
                            title: { 
                                display: true,
                                text: 'Number of Incidents',
                                font: {
                                    size: 14,
                                    weight: '600'
                                }
                            }
                        },
                        x: {
                            grid: {
                                display: false
                            },
                            ticks: {
                                font: {
                                    size: 13
                                }
                            },
                            title: { 
                                display: true,
                                text: 'Year',
                                font: {
                                    size: 14,
                                    weight: '600'
                                }
                            }
                        }
                    },
                    plugins: { 
                        legend: { 
                            display: true,
                            position: 'top',
                            labels: {
                                font: {
                                    size: 14,
                                    weight: '500'
                                },
                                padding: 20,
                                usePointStyle: true
                            }
                        },
                        tooltip: {
                            backgroundColor: 'rgba(0, 0, 0, 0.8)',
                            padding: 12,
                            titleFont: {
                                size: 14
                            },
                            bodyFont: {
                                size: 13
                            },
                            callbacks: {
                                label: function(context) {
                                    return 'Incidents: ' + context.parsed.y.toLocaleString();
                                }
                            }
                        }
                    }
                }
            });
        }

        document.addEventListener('DOMContentLoaded', renderChart);
    </script>
</body>
</html>