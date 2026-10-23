代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zzyncjrc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bsyjhris.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3efgwrars.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zubogrmr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3umfjivgq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3jlrxewyl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lpjzvaeu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xfxvpazp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ldyzyllb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ltbsaaff.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ipipupaq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rczsvxrh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hkuvfdfh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3epienqhc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3bafmdsgg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3uifetpwp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ofgkajpz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tjubosol.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3unjncbrf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3pfwtxrcw.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ffglxfid.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jghcloms.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3rynrcovy.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rzozxmax.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jsstetbe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3noetvzdw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlwacsed.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbnzudxf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqlfkcry.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3zxyfalgw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3caielrum.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bubnzwhl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ijrtvetj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3imlntuyw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3dzqerpqa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3vvobpfor.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3vvnjivbe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tlgnumct.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3fmewnyjk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fycijkxf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xyxxbmhq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ohtdcevw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbmhdpug.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3odqhlgds.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vlyjphjh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cjoizlba.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vdqwqodz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pmfbgcco.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ufqlctqj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tbrelwid.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bhjpwntb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqbvjnms.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3hmolpvto.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bdxtbhvw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3omgtbqog.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3oathfpow.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3atfpjary.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3endxeavd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qlmgafro.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vkikdghj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3wqptvaao.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3cisphslh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dupzhwey.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qoukeqaf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jtvqgcwt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3iqzxhwhi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hfcozspa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3vuuxotxg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3faroptre.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kqwsogxa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3izfgtkfa.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxvnzos.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qdjihwgc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mcxdznvy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cxajlrbt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zwgwjmfm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3vimupvrc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ccxbpgjd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3yhuzmcoq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kkrshood.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3slhfxzqv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xdazucpb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yhqehhng.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kmmtsshq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ywcjtpck.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ujgsnlzp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3xwjriuow.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qkwsqgpt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3mrmiagup.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgqakhmm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ucgdequh.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3utxhsubr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzasmuhp.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3zwdqlwdr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ybxukfma.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dovgoxpo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rzgtgoyp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ztckklzl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rayddbch.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eocoyhit.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rmmviqwb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3vctewiev.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3biaibtns.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lrxzbavs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3bkbtgpvi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3dnxfosjy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fzlzorpb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xdpkcgqj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bhbxjjhh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3sjedytas.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ujwzewkl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hkalwbif.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ugkpsder.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arvxtmtd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3neujhyao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzrwbbio.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3nczvzolz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mzkbslnn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gkfwlxeg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3dybnggnw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oagoytsb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fejdzzvz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qnoxgisw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pwmxtlsy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ccwukccy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xxsogbwo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ehawyfyd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3cirmethx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pawnzohx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mialdjvo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3luezvred.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ipayicjr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wmfyyvrm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3iutmtnzk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3odgxmfhu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hxunxwqa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zyfjghdl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lkzqqxqy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3memejjrg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ercoepjk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3aosxqnqu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3fxietdhu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bkzqzqnv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3lecjceyf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jwqmsamg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ujqfolmv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uvrxwizj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dfxxdega.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3taxtssje.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nevamkjo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3mdriuncx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3uxsdbfzb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fagnnnxw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3dsdaijes.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vxzcsptm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zucohvry.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3txiftevr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jpjilcim.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3vgmorryh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3llesmiyp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwxjvhxn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3cpqfuodp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3agnrcqka.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mutpqyhc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zvhyluac.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jkjgormj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zbdjjipx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ojbzjhwa.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rpqxsitz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wfdhzmcx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3vusyojor.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3masnlfxv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ahtzefny.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lskvszrc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ejcammof.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3pyzwfpvr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kbuogvru.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3xtbagbqw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3rkjqzzwq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3arwwvrjv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3uzqvpebe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjmfjwgp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3foggzmcy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vceiebve.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3izbspgom.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3uuimyvzu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ulqibtaj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yuemgpiz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3agelpetb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlwfyxso.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3upetjblp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bkzdxlvy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dhhuxdoq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wyatatkq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mnqjlhot.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qtnpykdn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fxiusaoq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3mwyaqyes.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fgxhdruu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rkrszxvx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3isuptcks.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ccucddnk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ypjwcqpk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bcjxnaoe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vpuramvs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vzzuidzu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xvkabprm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wlcggkse.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jnbbexck.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cyzfoyra.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjiwpkim.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3czrrsfla.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3fpbvgmzq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iczastyp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3lqdbqwdf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3pwsjtioo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3hpqgrveq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lndouzxr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3zmuzvbds.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hkgiaiuy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vkvoymha.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3saqrygjb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3tzsxulxj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3mwagrxpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgreiirq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3divdzpkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkfvhtxq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3bxnznhcz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3wuwxikxo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3noiqqild.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqwsclei.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3lzzzqqnr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jntcdmjl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3dfvogkpr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3oygrytvj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pqvsqfbm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3swlyiepy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3zofsdejt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbzlzhlv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwpessef.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3srzzubcn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xhftbjrl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tebfbbxo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3hqbrijlv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ihvykmdp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jearllmz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ytgfksyp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ilcnpgsg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nznkvxdx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3efkwfswa.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3nkpgwqlh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3diqzioxa.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bdpclpcu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ktgtefqo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3tmjrvejn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3veeuinbf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lycgjitr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffhznzpy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbruenma.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fslvmscj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ualgutbb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vekgihrw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3slkrsyzl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3cxirrssb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ltrxkeer.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxhjvxqo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wanxamtu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rvuhnbmd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pamdmkqa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3besnqbdo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cqmfiybj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtmuyvyi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3klojkosk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3cwnpamqd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnybrdlr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hisafnah.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bnazfspb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfpcdxdz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3dihxugok.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3hdwyepkt.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3lsxmcrmg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zovauvkp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3irksfzjk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3kyxhdgyw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3attrirth.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tcoclllj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ukacqraf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3kntngeef.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3yqachhfw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pbsqjlvl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3pdznatzd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3jyflljib.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldgpsolg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfrlzrem.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3crzwrksn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gztmszku.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3skenmnho.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ojcaoaqd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aojsurno.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3bmfttuvs.html


<!-- 参考信息 -->