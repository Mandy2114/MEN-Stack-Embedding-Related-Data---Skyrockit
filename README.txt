building out router logic here
controllers/applications.js
router.get('/', (req, res) => {
  res.send('Hello applications index route!');
});
||
controllers/applications.js
router.get('/', async (req, res) => {
  try {
    res.render('applications/index.ejs');
  } catch (error) {
    console.log(error)
    res.redirect('/')
  }
});
controllers/applications.js
