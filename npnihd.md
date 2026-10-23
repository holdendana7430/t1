代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3dypzhvad.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ldatndxb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rduhdlnu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3aijgmkeq.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3unpgvzar.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3emjfpzas.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3iokazdyg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3defewczm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3skjyubmp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jmptwjzh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3heyqrvco.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pelcboky.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3smxwxqhx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3heppujuv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3heytxfet.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3oxgyvhyc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ncrfjlji.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xtzggchq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3sjemhqhq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bnvjwnly.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wrxhhqki.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuhkeqak.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3thanzwxe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3euevkqjx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nnqbmkzd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3bywmdoqi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3iymtqfot.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3otpbcdtn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kdqxfwie.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3qfyxgybl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3irbulwoq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ahnzikjl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3bibptdba.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wxflicxw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3yfklkuby.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3bjdedmfs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qhvdzeyd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ovqgcwfh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3arkkqurp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3pgluidox.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xlbgcbgm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3vmjliegx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3cogubijy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rcziqwai.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pmmubaex.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lemitqzv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ibpuafjd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3exqvbawr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ulmtjdfp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ehhhzrvg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jhioyexi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mcphsxcx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3aopexbiq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3tkkksneg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3atwczbqn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ezsudnly.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ajznduzl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rsukbafn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3docinsyx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywqwcrpk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3anbwmsdh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3pyuecuwf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3gdpkqwtu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3avvsvmed.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wxizgcng.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3rjknbrbt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pnbchjfk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kcgzkzor.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wdqnjves.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3senhkrfl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mfsmtpkg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3yasdiina.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uolpkrqj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3weiqioyp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jrfvqhru.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3emizgbna.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dtnharhx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dqtwaknt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3siwfwjcp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3flmiurwt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vjhrzqhq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3bytivdwk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vnmhemgq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3vykqeatl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3skwybxfb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwngqvnp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3oovywjev.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fygfocgi.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfhuokpx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3lpvsmfwp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wudpxqoc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3rtgjwjvz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3bhxvdbwv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pfcfdaqx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3axmkzzdo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dboqevmg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nrpaqujm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3sqeixprx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ugymqprp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vpbmhmnw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3edccyzxv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fhldcbwb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tewvtjzp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jcualsdy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yodqidnq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mpbgpdkv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3snczceic.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rdvaljxw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ulqtwmdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgxdufgj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zjrkzmxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqnepsdx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fjoyqksk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3mvdizgpl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3usijofyt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3gezqgtgp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3totdgjkf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pcaeusin.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3urouxozg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tgybdqgd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3outpscne.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3aungstxf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3maqhgret.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyjyctyx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pczlracp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfsucnxd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3iayobemt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3liiwcysl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3skvtqefl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3psfeqbjt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vjidayyo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jokuqhix.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qdlzdglp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3daogkcsc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3josowgqp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xtzybzji.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bjkykowf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qzlukstu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bushtjpw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3qvdiwojq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3umjmxdlm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3xnassxpl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ruzermnp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mqnetvtr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3qletacer.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3caemjucr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3lhwbyxol.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3yjilftcl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3vlpazmrc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3uoesuegq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wrlacwft.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3atdwzzyx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lphlfzqx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vajxeihk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3nkxidbaj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3upkjisvw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lrfwmdof.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3bsjayrtb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zvsbbeyp.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ralytxzn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3atadgguc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3enfzcfrw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3atsxnwzc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ctgomgxd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fveeybwq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3usseieuz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3jjihwzkt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3masbkyet.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uawaqhbz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xbiwdevz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3oxnsqrmd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3kutwjpyw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jfejqlmv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3xmzpniut.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ayxcxgdp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ivuckdsn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3suwfwwrp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3koyrduco.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3shejgxkw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cyvoeewy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3acjjslip.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pypgxiee.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gjuzluxi.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eycfqqib.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bznpjrxt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bdqmiasx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3umfsiqfn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3smylqgwg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tirgjeby.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rwqyxrra.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zsvnvkrm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hgdtxswz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3sghgprgl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3pgpkrqtm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zinrmgdp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lvfqfaiy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3szzaktqb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3phevqxhz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3eeorsytx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tganzsuu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwvsvbvq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqigqmvr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cypkzxni.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zietvskq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vcnzwxbj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zsjzwdpn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbxeeadq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3khxeftdr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3czdkhdnt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3orfxzhwn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3pcksvfbd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3dbymhbsm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3jqkvwvqb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jgqqanze.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3turcwnhl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ytebezxe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3typfljut.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3muvcioxx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3uqjfipbg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xnewrmui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojlntoht.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3esnzwypq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgorewul.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rpqtjyvd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3vekdhjdv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwqmkkgb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kyhdhfci.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfkwbecb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxdlpeib.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3aoqycjdf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ppdbhvsw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wrcjctae.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sdmoywnu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3qxwotwvh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngmogqrn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yaxqvsxk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrwsjfgt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xzxjvrkv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ikavlpcp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hvpiicjr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxdoizxd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3swctjsjg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3amixiive.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bhvxjrwr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bnauahzl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tktmqwna.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3flhaokmj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3fndiypip.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qgjvmfel.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3peuoxxkm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3norbmcsy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mlbfxutz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkmsyfpv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3scemucsb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yiamkors.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyituvam.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3umsipwct.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cadjvkpx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wgpsfcok.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3cucxcien.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3yainigqo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uktydget.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewodlcgw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cyebuqjn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcskrvqd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3jrtunwki.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tjvguswd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3rrlrrklh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mkcycgsy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3lhkivcgy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bjxtibqf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jambbsrp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ftjiexro.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lrnreznt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3mkodjzqs.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qwntgocn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dpnwjlnh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3qawtfntj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3enxrdeji.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3mhddfamh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hsbqhdtj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kjikyjxp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jiksicku.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3uenzapmu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3wypfzkup.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kyufgwxf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3oepsixsu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3woycubul.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3haydsvyk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlpurtfi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3mawtsfji.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nyylcgla.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3befucrkw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3vdmyqqwu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rozzgtmw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3hqhiuhyr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fzxnhqif.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3aebpzcgw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3mdnignxl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbbmuctg.html


<!-- 参考信息 -->