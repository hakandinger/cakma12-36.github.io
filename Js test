
function generateCalendar() {
  const calendar = [];
  const groups = ["08:00-20:00", "20:00-08:00", "İstirahat"];
  const days = 15;

  for (let day = 1; day <= days; day++) {
    const group1 = groups[(day - 1) % groups.length];
    const group2 = groups[(day) % groups.length];
    const group3 = groups[(day + 1) % groups.length];

    calendar.push({
      day: day,
      "1. Grup": group1,
      "2. Grup": group2,
      "3. Grup": group3,
    });
  }

  return calendar;
}

const calendar = generateCalendar();

console.log("Takvim:");
console.log("---------------------------------------------------");
console.log("|  Gün  | 1. Grup      | 2. Grup      | 3. Grup        |");
console.log("---------------------------------------------------");

calendar.forEach((day) => {
  console.log(`|  ${day.day}   |  ${day["1. Grup"]}   |  ${day["2. Grup"]}   |  ${day["3. Grup"]}       |`);
});

console.log("---------------------------------------------------");
