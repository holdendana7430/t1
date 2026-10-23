代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ifaiostm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ytyfytyr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rinqvfdk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tlsoycyp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xqwfbqbn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qgnbxfdv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xogposnj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ykeyocyw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3veoakrso.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yimjrxfv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3typjqayh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oioxgjqy.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3uddpcsbf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qbfcmzuu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bancgeom.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ftujcnlj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3elkpkjug.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sajlvjns.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nykkveys.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3kaiyxwaq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hlpbzxjn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3bbujdycq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pqroszrf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3htpunial.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvaawtim.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tdqhxxnq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3iyrqirnp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yqvmovax.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3scqqcuzv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3diujuugg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3czzuentr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3edsrjqap.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tsrhkalj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3npfanljz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3liegecpk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3tdqmlxcv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3izmwnubz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3dmnvlkzr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqhglxkw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bisqvcgm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aafxzucx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3yramahsh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hjhkowwg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wrexmvqq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rbxseamb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ttsfxupb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cgcqxsns.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vwpjwxyp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ybdzupki.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vvwwzqgc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pabuziix.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ylmgemjm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3cmhutziu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3bgbrxxhm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3roxlmodw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3tuxdigoa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3tapzuwaj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3xtwralox.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pobjoljk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lrntfljf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqezihxj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dprctitq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ioqrqqlx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3suzbwtxl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3letmljgo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3oaeqbmfn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3lqpedmje.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lycpwwhc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oeybgggu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jwjiwyqx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vwlmciru.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jatjsklh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fxalfdkj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zipmvtga.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jmspbpzo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bnvtxfng.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3loxosfjk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bifkzuvm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gmaphynr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hdfxqzpw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wjsuswki.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3irzjdvnh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3klaivyyj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3pixywfck.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3xfyjrvvb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdiplvrv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3xphweiys.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dpogxosq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lvwjueid.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ogpszlnz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tohmdvlg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3rtyllngp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3qvqneccl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ubpgwfzr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3atyhcfst.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bwzlpjfb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oeqjhuxi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3fnehfgki.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uxxiugco.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hzakfqhi.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3lrhhtiym.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3panpklvv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eduifwol.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hgqqrocm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pfyxcajx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cyynehra.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jfcwzzhl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ikwzfvqq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xtcauwbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mimbhcov.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3hnsibgjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iuhzhbzt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oaclrbxx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3qbdqjfhr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vstgxsye.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vcdhoxpz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mydxjnll.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3phrtepkj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ajnriicw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jqxjkfci.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nvmlbati.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvwalwhz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dkknjbib.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3oequtvlx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nlfpgvan.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ucxfxhkk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3eeqefbtm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3hcqljmvx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ochlvsws.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsdughkg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3yzttoocs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3muhkwgnp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ywfnpgxt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uxcgngfg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zmyhialh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lbsjrooo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3gqiuhgrc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3lgqystkf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hhageuid.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3izgvzlhb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3miawrlsm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xsvuibgf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3cwgtvqnl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gdlfaflc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3mjdeksdg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oemsbfwb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3plywixil.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ftonmktj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3wtdumkyr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3uvidtkzh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3csfedkeo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lchpiubt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dolkqmuu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3movjwzqq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3hsywhvvy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yjbbtypl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qtdaisss.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ucdwhynp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjmsbpur.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wrtwuzen.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqpaqhlp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gsmnjjvl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3monsisca.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3icegkykw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3opfnarkw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uexumsyp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3lgryqrit.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qgiiijig.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pmylerhc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wxdavuay.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3omafnofp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jgpyeswf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3tuwvruhh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3kwqwabvc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3dpfiqwtv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3mkabijna.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3iillvmkl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zptojmty.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xnnvlsbv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rhghlguy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ibsamfts.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nosfjlne.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3egqrgjfy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ymcrilzn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3tmrqkauw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjrtiivx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wdjpxdkm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tsgdsjbl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3aczyvwfa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ojifsguk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3pgcdkldc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3orlanrvl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3bqvwhhly.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3hybwwvzm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3binkonan.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3okhoxhad.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kirbifhq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uimbxavz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3eiwxhcys.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ovcggfoz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rbnwzzuh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3anafzjim.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cuioyuaq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eheleebj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3nfvfcoeo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mgzuuopa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sqhondfs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xggfufuo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3xcaowjgk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3succjcvl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3reurfqeb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3enockofi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3rbyxorgm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zquenaoo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3grkkgwlw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cnlnvhib.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3hhpwkctb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3yucpeaxx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rkwgezuy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3holylflp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjtytrui.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hkpdzwpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zywfdhve.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3naxeiavu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3zkryttnu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vthlqyzq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3twpqktry.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3etkiydbg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncaysjac.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3upeaduwj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vslqvnnw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzwwlqqp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ufwvxfyh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3lavsbems.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ublsvroc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nnqnyaqz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxffniby.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wzkpoyzn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cabizdfk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3csyxmzrr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hwkcxqby.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3dpolawmp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ngkwodbs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lzjzzupm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fruafqmp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qceorsxd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3cparsnsk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3vswabesj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gytamomx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lbvnodrm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3flpfzmut.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qryxcvhy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tncespap.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxwybpfu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eksteehm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzwvvvwt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3deeuqvbg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kzzixmjv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zrsgyfvs.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mkvjwmrs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ipptfhvp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqbjqxxz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zeirzwru.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jjjdnryh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jtqqxcjo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3cgcypmls.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3btojjuhz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3gpckfkpm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3inneulwz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3tuiemkbl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zlgdzufg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfpsrdvw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxizroln.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sraijqmj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rbpenlll.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zjoufbwz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ufvqnheu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wurgaqgm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3vdsvdhdn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3kjaxjrkb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tujtqwep.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dxhtmhjg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cdptfwbc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vwjccaix.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3kggctbbm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bzhhezom.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3kzznsizq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vesyqoru.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3prczbzfb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3yelhpmyt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3uxpxafdd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rietvxbv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ihvpwfon.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qahlwhda.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsriqohk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3vrekicsm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3jwhpgzoj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3qtpwnbpy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qaoarcto.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3kclnmryg.html


<!-- 参考信息 -->