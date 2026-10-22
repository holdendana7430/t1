代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ijbqiizx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2hmsglnxj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2hgfhcxpd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gcdelvxc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2sympgfjt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bxnvncys.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2gmsogaom.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2usghlkly.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lszwoqsm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bzfxmrvk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bviuixqx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2voagdtlb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2qqxcyscq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cvgofwfm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mzzdflvl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fxchqboc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zrtfbggr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vxnsvwzj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2glmhzqsx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dulomlay.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2khpdkddl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ojqsvgao.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tvrrrmyt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fbfmefde.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2xyzvarrf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zywlkbxx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wlpdkmnu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mmeqycbi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2gidaxqae.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gwawmouq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2qusmnoyp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fdxgezlv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2tuujuwrq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2coopmqhu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xnxblkxe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2riahqbqi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhmbedxv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2npkbagch.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2tfkpbpmu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jyacwapo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2essalwku.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2zjjrbofl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2glkqomsl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2orvpsshu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2spwlouqq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xevlfree.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2mgubqblt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2kpedogwu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xqqdhpzc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2qpfbdati.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2meeggpgl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kgkbwdzi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rujaxpuo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2cqfqclzy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wohleskv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2bvvurngf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eovarpme.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2sabbbucx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2otviqlwo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2eoqsxygb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ovnntapt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2iqapaumr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rwfmrkiw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2yamjhdbm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xenthicw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ubjbcgcf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2yfkoxgxx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2mtzavvsg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jyqtusvu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ydolsltc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ohbyvajr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eovocbfl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbvkosjm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ybhmyjzq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ovuwppde.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ifjrqsjk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2slgfrocq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2aexdfeqx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2dvbiucld.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2daowrgkq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lkaddbhg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tvuyvjel.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zlurbgzs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lcdytifm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nshsvypb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ampmmdlz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2waxaxbdz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dvsdrzfk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xyfwrrha.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tkbmqysu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2izgtapvd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qxccynge.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2oucsokdf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2jmjqydgs.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ruoeieqd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2rtvavvfa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2mvsksbhh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xszesuau.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2toextmhx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fisiogru.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2llkyffwy.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ogbsuhik.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2jdrmzmnq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2cccytlrm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2usyzyzls.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kfaurwle.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2khceqxtw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zmeyiixq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gobenotd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rveheskf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dmbmrbtk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pwwrhejw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2osxkkfyw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qbcszcze.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ffgaswok.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qoraqnly.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vpzwbpea.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2oshanjbp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rkmmbkvm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sgahuzcj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wkniiosf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihgovpmk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2lwslakmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lspyaqvm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bztlcgiq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2jyvoiydl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kesbqiro.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2okohoerc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2alqxueom.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rhjqtnyb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dwuxmeum.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mcktkyde.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xkvpoayw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2slriqatj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2nfbylmja.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2trgvmcdx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bmxmofrj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hzbprfkc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mhoxzdzi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ygdyuvyx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2yahcszyl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2yygsgqaa.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2sootxczr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hiayfuff.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xihalpdx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qypvfudy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zvhzwepu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ypsjewfu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ezuihgep.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2toplejwx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xwmdgxdl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2tdkqxqgq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2enhedssz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ulzkilav.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lyrtpodg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2eoeumrns.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2esvxjcfb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nfknvhkr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2iwdliddw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jgxhrqae.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bjgyzlbu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2vmkleevm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vkmtedwp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hjbgxsms.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rlwthosh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2oboctfjc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2owbrwuet.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2smombovn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hipbsdzf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2nrzevnlj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmylwupv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2usvzznxe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xvlnfmzi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2elofquim.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2swelvzmu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mrwnqrhj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gklmmlbb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hjebgsqi.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2gosvaqer.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ssrkwelj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2scsxrtgw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lbbbbwfy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2oksomyql.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2fwixegyy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2baroxfny.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2jmnmedyk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2hjddcwbd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ygqfsjzl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2oiooqoza.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaxcpljy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oduitlxx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nhadnejo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uqqzpgup.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xdqoayir.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2itbisulq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2konkejmb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ghlcjebz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2anpzqxhy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ufyhmsha.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2trqqevoo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rpufvyjr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pyajfmbv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2myhdyndo.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oiwgsrxy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2hfxxfwaa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ylkghnch.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zuyayatv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dhjbhkru.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dcxgxwqm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vllybyxm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ogauvzhe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2llselxaz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rksqwkzo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cimmvqsm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2kcondonn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmmsogyq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2rfcketvs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aqvcgdgn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kobkvshy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ffzoilwh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2uxxsmmee.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tdfmygfx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2louczciy.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2accwhbgr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2betnojso.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zosnopiv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2oniqzdiy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ohzbleyz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2rbujhcep.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2sysmkqaw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fsuvxuxz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vjjeusiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pveebppy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dlslznyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhvhqqko.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ftbpybic.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2dahqnyrl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xiuxthxa.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wmcoagkw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuwuhdwt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2nutbgwgr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qdzmhwvi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2tpqdxsdj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lodjfkco.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2etiokqmb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wdbjvuap.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxodmhnk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2huaylydu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wvojobcb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2urhumkks.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2kizsuxmk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2iabigixc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2voafvfnv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ipplxyng.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xbysrifc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bnkonmib.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mwsbxgbf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lzckyglg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2zrkkafdj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dcnjzwlq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2opiwbohi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oyofevun.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jgludcin.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dyknjwcr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdypfudq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkewggpz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpdaghuz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fuzqzaji.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ibequneg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hufpaozk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2oswjormi.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2papopjtk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2uygbzoay.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbrbsugq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2veygdpjr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2puszdobh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gwtnisef.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2sgnbgzxf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2kitoaltw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqnptkpa.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2dhhxmgnf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2qkkrxxkt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oduuzfnz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uajijgou.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bzxvjopl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kasizmcl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2biosuxrj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2axjvmqjr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rbkntwfx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2pzqufqbr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2moljbetm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2scjpyblr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2stndgddd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2auvdyyqh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uemlbghk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2orsgkbiu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2kljdgzyy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yrhesxbk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vmwfocir.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xqgfcuwn.html


<!-- 参考信息 -->