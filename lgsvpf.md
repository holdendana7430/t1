代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3kjbwqeak.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3asriiuix.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3cmymgrvc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mvbwemzn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fdoprzpc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ghlmfpdg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ccrhfgyp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eyqlwioo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3etjvtvnd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cqofgzlp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gyhofsmi.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3eoiqeane.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ispaajua.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sagevtkm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nnunwhqp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nnsxqwhw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ssvavqqv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wrxbqwgc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jrzkuxtj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3erxblcaw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xaixqzib.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ujouathp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cgtxwghg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ebvdnhzm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3gcfwrfye.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ofaojeoh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3enyuicuk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3bjmyusvc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3puoaiqti.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hqucxhxl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvofptep.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oghfiwer.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qmpzlmlq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3gcaqibcz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3txsvkacc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmtpfkmy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ioejsrqk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3saqvesky.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ooqlnswa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3qxvdxsxr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nhcoxtiu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ulyvirzh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3dwitndti.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3kmtzhqxj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fbqacalv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3jolhwvmg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3hydmkcqd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eolejgfj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3qtzpftue.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lylrgkzy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3fethoart.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3crtobhzo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mlalctld.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pzebhdeg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dhhrlhcl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3znlidelf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3aicjezwf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3shgkxhgi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3sqptjpui.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3afflzsuq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ivdquqml.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dgeanwiz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3fiinzaaa.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gambwosh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3vvkjepuf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3taapjeej.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3uvdhjuiy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mlkftgyi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbxgelkj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mbrvudjc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qwwskowj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3fcqiembd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3eugyzkod.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3irtntlbe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3scicuafp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wyfusxcq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fubciiqj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jxlczqpc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bosjcevw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uoyglbsi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3widdpnhe.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3txbfbndz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3wslszgah.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3engbanqg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3delghlgm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wafcefls.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rmacmdar.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bbxhyhdn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3zzyhemul.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3lvoefynr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3vgcehoov.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3lxyggczs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3bixbcywv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3jrtnzett.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3payuygie.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptpnjdpu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3lavewyxe.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3htukempf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3sgfutydq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3vsmamzlq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ckjizdzf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jxpqqkfj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ekjzuzmz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3abojgggm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tbzsaeol.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qownfbbg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wdhnxrun.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3grbvzokm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ksswbvwp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3votuovfh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mukwjdnm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zsdheqoz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3unsknbuv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hjdnzgoi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ohdlifxx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rgnardye.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xipizlej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlekmlzn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3xpccsbdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kljlrvsf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xvywgfsi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3wwvbihkp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xthuuijw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3cawygjmf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kxlspwia.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dwliwios.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3vdfqoozx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pxmziptx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3calcctxg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dxkgvnfv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3pgfojwbf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3fiftdrso.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jxlzhstx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbqtplgd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dxycqrty.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3fqcvddqo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3bqypemal.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3cwnukajn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qxpttnmc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zdprysyl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rqxfthri.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zmbzoioa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pemoijfz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xfyokqkx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3igekwiya.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fwsekatg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gldilfgg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3bhcvwstl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sbeibnhf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3qzmbcxwr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3dvegajqr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wtyyfcvl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3htfwchxw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bwnmsogb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3lvvlkbpd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3gsqrtply.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qsyeggfu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mxdrcqop.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lhfmuxms.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rdxszutu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kcvnqxxe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zhgydstw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3sqgvkidj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lizvfyjj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vjaydwmd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hyptktbn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jthxlpov.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uuoszlmr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujwauouv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kwfpoiip.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fzwmadbm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vrdjhjhh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3guasfelm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bqqsjqwe.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ionfqctv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qdfzqyzp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3atgwjyor.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ymqxpbbm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3canjbnie.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3zjovnfif.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ckqgjckr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fdjusewi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3yfezyvmd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3mqssfjia.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3undhdyfy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3glhnqqqj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3syldihov.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kkxrdrjo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hohxejlo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3kkmffnyq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gjseacmi.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3hpyudgsz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zswampjt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pasdcewx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dfrbgpbf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ihdxoujp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wsknjtcx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uvgccbta.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rbbptucj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3namzkeal.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3dpenkzuj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ulzvojic.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lwgtmquy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3stuvkrdr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pcisdqco.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wgkyytuy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3qjtlyvzx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xfkkllad.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhxerydi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgnrndtr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ffgmqitq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3aboygkty.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fzmzakcf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sqrnyrsx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wfobdnbh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3snilhheb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gfdptpzx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lmnajddg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3pnjyxyeb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3uevwukta.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3egcvfcbj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gqdkmekj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3knxmxoao.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3aubmftsz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ppfihvde.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3oclkcktd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3gkzxwcfv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3bslyltya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgftnwip.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3duuamvfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aexcxuup.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3mbgpnzhu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3vaqvssij.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxddpukl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sokqvihq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3akxqbjbl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3umkpnbfi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3cvacsyca.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sxmhkpxi.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytbgwxmm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3oxtowwyk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3yxctnqwh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3siezxxkh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynrmslcw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3mlrvzifi.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqzfeuoz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3omfmzerd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sxppuzqs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yzvfibzs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3lpzplzvc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zqiexuyl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ttlzgron.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sxczyxgv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tkkofcyz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3aibyspqs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ctgslwjh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gfetdcko.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3cjsrdnqs.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3cqwjwoki.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pikdjahy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3llsltucb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ziekjmvt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hltpplyn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nbyzkdnf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ojgmuobw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bnrylygb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mwdbrvxv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ynqakndo.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3bvujkhdb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzjqoeft.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpzhaese.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lljaapwo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3frlcubib.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3xefhtyhh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3utdzpjqv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejopcjqf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ndkdezbu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3czwqvgvm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vwbtgsri.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikuaxpwe.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmbdcrby.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pbyoabgx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3yysnmorq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3mlnkvfqt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ftdynzsa.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zltmtlld.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3qiobmqec.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3royqavbv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3klkmgpds.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nwgfxbny.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kdnezyyo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ixrxskju.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3zwclbvxt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3syrkvcxz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3dlsvrbcn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qkyllaiq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3afdpjxtv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hdsewakl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfpispem.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3kfgmlchm.html


<!-- 参考信息 -->