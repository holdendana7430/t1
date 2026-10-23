代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tdunqzwh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dcackpub.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sxvtmfbj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jvcvdymq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3jmeisayf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3irsxliem.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bhvkpekf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yktsueky.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qrwkxjzy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hrlpbsew.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3azxiobtr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3pqjrykki.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3suuyarkm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ssgttlex.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3qkkbuxim.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hficowqp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3tdgmeauy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mnzuenrp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mrcctsqn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3bdflmouu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vnhuvhkk.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rmnzrfer.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3seicqsaj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3pjvcxgyn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ayhdqihl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ielpebtn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ltyampfy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hhoqeuvq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3iisdzgcu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3zpgxevgf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3iwujeyua.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gfrtbple.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3znqbovvl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3bsxpljra.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3rxfgicqf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3swakbmip.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3zuevswdo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kmmioplg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3nnbadkmw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3okqlptwe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ykhqmxum.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rwczjesa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qzbeogvo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3dadttfev.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3hjiqzryt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3axjnpemn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tqklpgug.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3anldlmvg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3vocceqnd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqeoxjln.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vhqyxxkk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3fylzbsdo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3llszjerp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uwgweeuv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3juglrwtu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zclirmeg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ruxktupr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nepzdwhe.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ntptlpez.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3zrzbbnpx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3kobjymtn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qmriayqj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wbltvmux.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfpjnlqx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ldgmeadk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rbzycauv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wetfknnz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xpifiqth.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ahyyzsyy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3whvpqubz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3dfgwrpch.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pkuobuiv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fkpathjh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zrrwnrdc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xopnalpi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3kmqjszrj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3erhnccqc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3usprriwc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fupnawki.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3stumivnj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wtfebxwb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xcubbhdi.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3lzcexfyt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fjrtvhax.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3eeispsne.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3mrvglgdl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3bdltalhj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3cwiwmqon.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3kitdhbxa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gacliemd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqfsnuhr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rnaiuunc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3snyukull.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3gldeudjz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3mgcxqdhx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3bnjsjoqs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ijtlledt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dhawygpz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hxlfyakp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cnwvjjgp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xtgbrsox.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3suylorht.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jhusnjdj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lonebfht.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3faqkxqxg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3xhvjunjb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3csqzcdij.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ohklbdhu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3evrujjjb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tqfkbzex.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tjvxktkc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yerxprjy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kwwhgehy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjuuzrde.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3lljolifa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spezyfct.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3glfvjgnx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3iynknzht.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mpegbgvp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3dmdlvohu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pngxqsjr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xciaqbyj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3jzvjjzct.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3afpjkwqa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3odmtdlqb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3uxkazxzc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3nvwnivdw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uaizfcej.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uglbqazy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvempzho.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bpdluoyl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3fhuurmsu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zvvmlaho.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ucdltoyy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3dpheqbpe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pdstcupf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3irwifhsu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gyxjdxnz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3inazggfy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3klkiqixa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bcdwddxa.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jubmwdot.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wxceijky.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3avsvtnxl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pimhuekf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pdwshmnc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vvjzorrm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wfbbqozr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3nyxmxcro.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rmrracgk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3iawxgmke.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fbuuwhcw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yrlslzhd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3dbqsebvb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vyvbadbn.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tialyhhr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3swndcztb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rrywlyys.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3eotqktkg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gaubjajt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3muhruecz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3frrcleno.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3klbhnrad.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3arldqbqo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jtenrqnr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkndkswr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cfkzguhe.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cspfkkzi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwkvracd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fwyvaede.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wfnjcraj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mrfmvvts.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3flipfppx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xtndrmku.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3grssjtaq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3rhsfxxwn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ujluxekz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3swkdtgok.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3jgomrytn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rflpovpn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3npzeurfb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3yjhrgcjj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zqlsdpzq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ugdputqi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jwdubnva.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qgxewcsp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3fsirxbas.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ttsepjoe.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3sqfzjrys.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lrzrkeer.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wbmhrcfd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3uxbywens.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3loiywsqt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kzmqsitz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3kgcatpap.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ekszolkf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3lxgkwnlb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3whhcvfff.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fuvzsbtv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xwhhvzlm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggdmhbyr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ppowpeem.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3werguckh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pxdfvlyi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwabrtol.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gzgymbyz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ilizclhj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvssiurt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3kveatwwa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vdflrszm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwzfjwgb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ywdracps.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3fboiutdd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3towoqnee.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3pbfurlfs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3johioqdz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3vfstoyov.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3eixmgsnb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qqcbutug.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3vefjczvj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3yeccppei.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dkfriipf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3sklvxrwg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3obiiejyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vywelkxd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3adpvhfqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgytmbnd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3tjmguvlj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3rmhloiru.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlvdcorv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fohybumo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3imkkbfse.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cccgoasm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3hnzoestk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mpfvvroa.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3boasoffx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3xrrbpdnv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ryabznzn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jlksggvd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mbqxdbvx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsnepger.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3caczrxju.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3zgmlzxlo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3jlgsnrzc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wvvrkrod.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ctbnslgb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pelbsiil.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bpxemcty.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uaxlkthm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nooonaiy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3hsopvtzt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3zdpoiugd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pokzgpys.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wibbtntb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3uzewwadt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gosfavbc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kszxgyua.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjndfgoo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykkjutip.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3swqjvola.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zaaxfwco.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zefksjrr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qlinyscq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3lwymuyhu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3itwfdgjt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wcxmuivd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ppnsmujo.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mofajskw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pzonuavz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3msmwynre.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hcvzywxg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qgaxxzmb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xhwdxeap.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qykvjksw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3looohvho.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3shiojawg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eektyhja.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3asdqpwmf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3kzozkbdn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jntaqzhy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3svhhiwst.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xhcyxcyt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3icwctuah.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ztibtean.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3anivsyje.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3frambwdx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bwhrrfto.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ntmdomyy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3vibrqojk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fprbvjqh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3bkleksqz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ieykehzk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcpqutyg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3moeucvop.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcuxjzug.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvijfxzf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ainjpinq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ymomfzlz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3armzbnqe.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gpxsubns.html


<!-- 参考信息 -->