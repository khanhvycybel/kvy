
exports.keepAlive = async (req, res) => {
  try {
    const response = await axios.get('https://your-replit-project-name.your-username.repl.co/keepalive');
    res.status(200).send('KeepAlive success');
  } catch (error) {
    console.error(error);
    res.status(500).send('KeepAlive failed');
  }
};
