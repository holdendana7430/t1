代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gllptilax.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gfmhukidf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gkdmbeltz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/goehnwfhz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gtpdnebag.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gtehvpbxy.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gpiwomsjl.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gnaiycgmg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gfunbcfnj.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ggmdbqspi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gpdtbvkdn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/goboapwiz.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gtyoeiwqh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gzguidvop.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gvikiutyy.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/ghilrrtlq.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gzewdssfx.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gmfifkdph.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gktligovt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gepikmigl.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gmaqirdlw.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/ggpmebeel.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gurthwizl.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/goymdajss.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gcbmlmkmz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gilkgpfef.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gtryzfepm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gasjkjuwf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gvsiypfwi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gfmokgnis.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/ggopxwber.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gmkgsibjk.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gvnqozjdf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gocjfhlfd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gpytnjhbe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gaqjlqvwx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gstufnlhq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gpkfrqjcn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gwutzovmj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/ggvfqkjld.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gwvarlhun.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gkevnpfyz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gosiowdeq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gpksqvxqw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gacxyloex.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gqbzpbykn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gwqhmktnc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/grzmspqaz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gzqaxrupl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gjlbjiwei.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/glxwroufd.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gbnczqprx.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gevnuhphn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gsfeftech.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gtvbcivrq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gwqocxtod.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gngcsvfpu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gotrlajqo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/ghuhmzubo.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gcbmrnofz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gkorraeuu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gkvmezhud.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gxurdpemd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gcgkjzzug.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gbsilgrgk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gufpixyxm.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gnydcbdpj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gwxkhigln.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/ghrpbuatu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gdlahprey.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gvvhekuaw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gnurqirkm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gyazfcrqo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gdlkbwabx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gzofndsuy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gvsnpfhtr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnxzvpvmp.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gcjripglc.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gudbyqsxx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gpnybtsrk.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gicswnjgu.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gzqlvqhrz.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gidruxdeh.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gevjvtntu.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/giujrlqtd.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gxlvwepwe.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gyzhksfew.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gbyznkbxp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gxgufvhxf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/ghkxfaugz.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gzsbafqwz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/ghsoljvmf.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gwfxnaeet.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gcawqijqh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/ggjkepkap.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gkmkhmznq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gbapfakxx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ghvvpasqd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gwdjibsdy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gjtrcgxbn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gackcggnf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gdocmoqjx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gbgyhniha.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gbwulsogg.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gdbazimcv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gtdbbhnkb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gazppbxcl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gqxqednbm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gmiqqciju.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/grekkmrkr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/guizwyhip.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gvhcutanu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gpitepqdr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glmbzxesl.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gipgwekmb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdryyjsvk.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gmdumnhwf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gnwajbyug.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gcvwhhelo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gmmcqqgmo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gialmnzef.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gxuhaylia.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gqfjnwotn.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gaeprkqxx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gprujqtzi.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gkefjhspl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gralslkkh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gbnkubkzy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gqejbiyci.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gnotojchh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gagnoiqro.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gawptilth.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/ggpdxmrhf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gofvlfaco.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gmjzzfwub.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gvafyhtjw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gydhlcoqb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gcjljaake.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gyhzzrhqp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gticjrhlp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/govvyjrsd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/glkjjvhao.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gjcjfohbp.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gkextvflh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gcwgwtrla.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gywloygbn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gvxagngmu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gceabpyic.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gqsgoqzab.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gicqikxkg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gybghyueu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gijomqyzl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/ghbbxinvc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/getlxeogc.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gtdfuofkv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggsivrrgp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxerrjbuf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gxmmrmlml.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/goyoeuham.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmwzshpss.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpryysrfz.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/giszysmst.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfvbzbmkv.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gafpuiwbz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcbpocknn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmvxdtkhw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gmeeghkfa.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gknkopusu.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gltqusafm.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gcwmxunwn.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gpqotgfgu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gkjpirptk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gtagjsckk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gwhxyipds.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gilxprwld.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gxdjdchcy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/grcbhkfbq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gzffsswkt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gyravewjl.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/ghhluozka.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gkerhawnf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gbelntjyq.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gzzeqrcgr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gvrhsprst.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gvqallhzd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gayrbblxe.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/glgjjghao.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gmnnkbfjp.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gslflipzk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gfyclublv.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ghbshwyfh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gbahtnnrc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/ghwzjxsth.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gxqpgncmj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gamxnpmjz.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gauadmepf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gcndydpva.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gjzxxclpy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnabkausr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gxlkldzmr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gqpznmkkx.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gosouxojh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gaiynqnap.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmqrjpzye.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwxsfziky.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbndlmcme.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gdollkkue.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnqsqcvra.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gwnmazpiw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gqfydmpzh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gfoertpoq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gwlidrjms.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gcwfxwbvh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/glesjkssp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gfvqqnlxh.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gmyjimyta.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gvdgzzmzw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gtaoqxuzk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/glslgswaz.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gvylrlzna.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gbtqjkomo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/grxkmxxxi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gczxcdohq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gccjthgtl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gaciaaasa.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gdcupefbf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guieahiux.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gmtusfsuq.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/grtowvinu.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/grhaieckn.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmnloqofa.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gfrjvsmjp.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gzypwrwbx.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gwdkrwtmh.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gseenuafn.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gwoyfhsfn.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gaktzlzlc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gbjqpnjuf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gonypnlgz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvwdnwazl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gprltvmyh.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gryryfskx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gyrsgzqom.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/ghpycgmxd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gojoqaxvd.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gpbaudzxc.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/grvabopcx.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/ghirbcvio.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gwevxpcik.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gtgettfsq.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/geftkypfg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/ggvagwqas.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/guthjnvfk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gwjqwpdbf.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/ggilddiqy.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gaqynbqmr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/giiwvdtrb.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gythhfrtx.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gbatnqbct.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gxshhlfaa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gndexslho.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gdbdjekmz.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gfgfkydhc.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gmrwxlblf.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gmwyeanwb.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gvmwgpafo.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gnxuxslci.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gsgilpzbl.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gwihufimk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gnmeudame.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gxitpmpna.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gydtyajvh.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gcoapdhlr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gtsafmglc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwajnjyjj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxrzoxzdb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gyqmmxbnq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/grlvnclui.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gwzzpcxhi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gvvyvhgru.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gbhvhylnr.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gaweqmabq.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gehnmcbpb.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gxxrqtnwf.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/goqsfbzjx.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/grckykbmx.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gcuwqogps.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gbufoehlg.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gronjnuuu.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/ggjlldphl.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gvkydyxva.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gxwyavpnh.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gkvkhkugk.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/goimsvaxa.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gqsfoubtr.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/ggtokcunp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gsraykujw.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gdfapufry.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gwvoiemgc.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/goyubggeq.sHtML


<!-- 参考信息 -->