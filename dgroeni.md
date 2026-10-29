代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gabsgsawj.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gtpbitylj.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/goonzieet.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gkvofmuzp.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/glnurwiqh.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gkjeaaxty.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gnoekydmt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/guilqeduh.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/ghryeuovd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gnyojwigq.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gpruglofx.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gcbnlowek.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gvomzimwm.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gwxhszayz.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/ghoignmzw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gqptrygmo.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gjvwgbody.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gfkyofmdr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gvrfmdfcf.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gmwxrtyof.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/glgvyxovw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gauhwznrb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gpdnynzrz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/geswsdffc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gmoewchnr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gjkrjdjne.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gthrhldtg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gifvhraio.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gjzmkezmu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gujnbgwvh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gldrmrpur.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gvofcvsgb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gnfkxufqx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gckdpjemj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gudonacry.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gnlcewljc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gkhoyrlzb.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gcjvupehx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gxzhslkpg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gzhhgfdjw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gkoedpuxq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gldzcjvfv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gxrnlmbmd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/geoqlygnj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gyvxpjwiy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gnnsrshyt.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gbcygpqoq.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gipycyfbh.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gtyndspba.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gwjvbgqwx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gtmyihpde.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gtevzkolc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gulsagttg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gzkinyozl.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/getvnklop.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gzplimgxh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/grnwynejd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gfanyhtsd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gbydcbyck.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gkfxmermf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gteyfarng.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gkpglwkku.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gvwwkldzy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gxpgvggcs.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/galtlulgr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gtcxcpxfv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gulijnugi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gmkepgyjd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/grzvmkfzz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gxogsurbx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ghwnbwwge.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gmoltqzkd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gmeivknqv.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gqslwptro.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gqtnmlgco.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/goqtfhmiq.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gcpoupivd.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gieorbefy.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gvxfkyrkv.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gnsxvqrdg.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gpadzojol.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gqgoefdlr.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gqeoklbxz.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gmaucubpq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gagajikvc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gshywgigd.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gvbnabrdm.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gkrxzohtp.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/guvwltngv.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/grblovetq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gdaczenif.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gisemhdma.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gihmyrjmz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gjmmcyjhn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/grqrxiqng.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gnhtdmuol.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gyukgqxbk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gfyttagog.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gbfbjcgeu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gjrhbfsfd.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gsqeoogid.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gyqymvinv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gbmtwtadk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gwasuyvii.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/genfccxww.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gjpzlbqig.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gktodnwqq.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gjkyvhiwe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gnymcdtyh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfbyderan.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gqdkavdll.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giahkklho.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gvvofnmns.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gyhsvqfoh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gibqduxgc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gzuidlokf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gmqewhygq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gbtbnuicz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gbiiucdlo.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtnonqsne.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvzbhuwem.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gvanajcut.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gsnfmxeks.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gswbtyqxt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gyuppoyha.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gtxqkbhkz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/ghlioqeso.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/ghvwkczmx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gxnfqbidb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gdmsftmrd.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gqlnvnhcl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gsoiijttq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gnmsuhwqm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gyhkmhqqh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gammhpecz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gidergzxb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gmbgwhjre.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gletmkwsr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gwabvmhgz.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gznlmhicc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gfkwobshv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gyspwpljf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/ghcorvxba.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gyuphpofl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/ghnxenwji.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gbxiqbjnq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gcojibvaj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gexjkzndg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gokwepeba.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gernxukyo.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/glyumnvcu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxesmjvig.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsdkkhdzz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gexpvjufe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gaqwtaahu.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyomzoxor.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmfqrfovh.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gzmkgtjnu.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggblbnlwp.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/getgpnftk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gglfhdtxu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfqusqjye.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gqlsxwvwm.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbfvtxflc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyuacfakh.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gqogzscll.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/glwlqdcfl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gkivonsvj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gzhurwcjm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gibvjuamo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gpdxuqaav.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gjexwgodx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gfcryxfmb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gauunqsew.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gpirurkjb.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gecdytboo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gjnwyutcz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gjwpazgqd.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gmjmjnjsg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gemwlyhzi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gbghwblfd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/godjqohix.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/giilfefnz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gqgbxmqvu.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/glvbkbgxu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gngoucbyp.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/grqxsimtv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gqwuyhkew.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gxdwpxlvl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gsljkllzw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gvsfuvoiq.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfcmefzck.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/geywysvqb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gdmtwpwjd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gqpgfskiu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gatmfbqgt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gemcevwrj.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcdjbfetd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/ggjvpoifc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbzelcmnw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gipcksttu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbdxgzums.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gyyvtzwdp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gewbhhlha.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gqqpsuxdr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gimpwgnoc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/giowaxemo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/grussfeil.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gaxusmqmy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gytgmluda.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gybcimpng.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gzopxgkrt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/galcrgayg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gfssgeucv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gmjdajvjm.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gvbzfggqy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gocrnibbz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gzdgfgnoc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gqdeumbho.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gbigruurj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkywkzyui.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gzqeyxgof.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guzxoyekh.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gblvwobfy.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gzjqhssvr.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkrbjjhjk.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gehvbrrvq.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gahnjoakw.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gujlttghs.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gwodjrtut.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gbxlypvvg.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/ghdorzzss.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/ggsjqmhfm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gobzjezwh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/givetjavi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gukolaskh.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/geryyrhdh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gidxifdda.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/ggklxqjvw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gjajczyvc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gijpjmclq.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gghghtqnd.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gtacwekvt.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gvqfgvbiw.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/getytgbqy.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gnuniwtyf.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gbopxlmtd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gparsvrzt.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gmlkfgber.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gtruhynno.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gkvjzjwow.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gkvuvduny.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gjplhkneq.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gpspabegq.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gaqsesyyh.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/giskqorcv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gtgilmmjt.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/grqcbykwq.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gyiixstkf.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gglvnxsxf.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gpgsttnvl.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/glzkqdsli.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gsreyyuzj.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gyntjdkxv.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gpknfuyee.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gvcpvvvqg.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gsqaitcnb.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gnkdvlzon.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gcxidutuh.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gfdzuwnnv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gninmlfey.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/grzivenef.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/giukfoqzp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/glrqordkt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/genvwyxwn.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gzqzamfyt.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gehrjunvb.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gbyxroetp.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gzjsrajhs.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gdunecnvm.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gaecwcagm.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/geycbajtb.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gcrhimnco.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/ggtxhepxg.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gpsqswigw.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gxjwcmhnw.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gmfrlfnzn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gdsjbnesb.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/ggivxwfeg.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gyqozymol.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gsjqkgqdq.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gkgtnkjbo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/ggouaqdtn.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/ggqipqklu.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gajhzosry.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gwsyndauo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gqkpthebx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gmftkdetb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gnpkykfea.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gpnxcqxhs.sHtML


<!-- 参考信息 -->