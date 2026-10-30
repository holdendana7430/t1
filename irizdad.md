代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztmpniqf.sHtML

Ruby: items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfsrilxk.sHtML

C#:   string.Join(",", items)
来源：http://baike.fanxiaobao.xyz/Article/details/gwcsitstk.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fanxiaobao.xyz/Article/details/gmauvtbdf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwpyanzd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzawvafs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gbxesglgj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gxpfrwcvw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fanxiaobao.xyz/Article/details/gyorhypmi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fanxiaobao.xyz/Article/details/gpqlkbeky.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/guzlooxpd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsnppqhu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fanxiaobao.xyz/Article/details/glwqvoeng.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvobpmyqn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkatkadgv.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxismhon.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvwgqfnk.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjfnzwwm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuczsukz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvrpvjas.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fanxiaobao.xyz/Article/details/gbazczier.sHtML

[E11] 反转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gnbvsdema.sHtML

Py:   s[::-1]
来源：http://3g.fanxiaobao.xyz/Article/details/gipkxqmju.sHtML

PHP:  strrev($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gtoipbdan.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyyqybue.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/glhpeixkw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gxapbdgyy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzeekajp.sHtML

Ruby: s.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/gniqxzkvr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnxersum.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fanxiaobao.xyz/Article/details/gonmlbrfl.sHtML

Py:   s.count("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gfjpbtegx.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdtsbsxn.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fanxiaobao.xyz/Article/details/gdrbgqngb.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gojhjtwzl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fanxiaobao.xyz/Article/details/golnrmpde.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfhtyyxk.sHtML

Ruby: s.count("a")
来源：http://3g.fanxiaobao.xyz/Article/details/grcoraloc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdxwpnaw.sHtML

[E13] 逐字符遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gocfefnpl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbwlolqv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzytalzyg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkuaezat.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/grliqdnmh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqzfbxfx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuclvxdy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgahjtdm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbbvqlno.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fanxiaobao.xyz/Article/details/gbgowgwwn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzfkvwyj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/guymskefs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fanxiaobao.xyz/Article/details/gwalwbebd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghizbqcus.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/grdtwpbmt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fanxiaobao.xyz/Article/details/goyytlxcm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fanxiaobao.xyz/Article/details/govcddopj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gmenonhjt.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fanxiaobao.xyz/Article/details/glnibrinq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdadehfsy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqfcvxgc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gixqrzanr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gxrzqepeg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbdietji.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeztlrtn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fanxiaobao.xyz/Article/details/grnmfhaac.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fanxiaobao.xyz/Article/details/grxcpziow.sHtML

[E16] 数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gppmfilmm.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfsrvtwu.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcexpvwo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fanxiaobao.xyz/Article/details/gbipxjwoa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrufomqk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtonckevn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbxcyamg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gqkoyhrnh.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghetsbdpx.sHtML

[E17] 首字母大写
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbekpswm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjvsjobc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gvgxlzdqm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gnghkdzir.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gtvdjhhlc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhbozxyg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/grbehlcun.sHtML

Ruby: s.capitalize
来源：http://baike.fanxiaobao.xyz/Article/details/gtxufbbqz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fanxiaobao.xyz/Article/details/gffxbmbcv.sHtML

[E18] 模板占位符替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcptykith.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fanxiaobao.xyz/Article/details/gbicutrpa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fanxiaobao.xyz/Article/details/gqimueged.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrjvpjdc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gvyhoucca.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glutewvdd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/geigsmcxf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvcuaqdoe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfsfxohg.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnthhlhi.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlojdvdk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjedowypr.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpdxomrj.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gukxpfank.sHtML

Java: s.lines().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gpwprmhyh.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gboqxsxqh.sHtML

Ruby: s.lines
来源：http://3g.fanxiaobao.xyz/Article/details/gnvjxicct.sHtML

C#:   s.Split('\n')
来源：http://baike.fanxiaobao.xyz/Article/details/gfnhoblsk.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkhkymoy.sHtML

Py:   if not s:
来源：http://baike.fanxiaobao.xyz/Article/details/gkpuuchqt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpgmzzax.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvmryrlw.sHtML

TS:   if (s === "") {}
来源：http://baike.fanxiaobao.xyz/Article/details/gixrhbygr.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdlhsbrqe.sHtML

Go:   if s == "" {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfuwviqv.sHtML

Ruby: if s.empty?
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkjvyvuh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfvmmhmr.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdfhopkv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fanxiaobao.xyz/Article/details/gbdsmnxfu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gdfxcjshv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gtwykuwtq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gnqxgkhug.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslewxvhx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrvjitbr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gbdqkffwa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/ghdvtxzcg.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fanxiaobao.xyz/Article/details/gaphvdbln.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrcsgvbh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/ggkhfihmt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gfelirneh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gssnmdzlm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fanxiaobao.xyz/Article/details/gtaknpsdb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fanxiaobao.xyz/Article/details/gunzyodww.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gbonghaxr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/grhnfheae.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhryjzmi.sHtML

F. 文件与目录
来源：http://wap.fanxiaobao.xyz/Article/details/gwyumyiwy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjwptpxld.sHtML

[F01] 读取整个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwavayuem.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fanxiaobao.xyz/Article/details/gztrdppts.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgiqzzvu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiejulch.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/gwramvilt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmdfyexb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fanxiaobao.xyz/Article/details/gwcnpfbom.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskxpjfgj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gutwnywra.sHtML

[F02] 逐行读取文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsapqvcrn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmposegh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghctsdsmt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gwheylkih.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyfieekz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fanxiaobao.xyz/Article/details/gcxdstfbd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlatrqos.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnoznjta.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsezpibn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fanxiaobao.xyz/Article/details/grjyhitxs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fanxiaobao.xyz/Article/details/glqslsthm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gemcquxng.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxxrvugx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwgqnkgb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/goahhzdju.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fanxiaobao.xyz/Article/details/gtietpytu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gcxtgivqx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/grudkbknn.sHtML

[F04] 追加写入文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnpctssuy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gclbxpunv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgqgdtll.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljtqsqwz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gjwagnowm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoycpinv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/glzfpribl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fanxiaobao.xyz/Article/details/gxcvewzbc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcwkinjl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpuufrdk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fanxiaobao.xyz/Article/details/gweiuohtn.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrlusqaq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnwlsveh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtcmtyqw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gnogvzpro.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdclgetst.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwbpquwj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamjfuocl.sHtML

[F06] 删除文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbghfnqz.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gkyevckwo.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gezasmxkl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwacadgv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxhbwmar.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbedlnipm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goopeubyc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdjkfjee.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvcvcmed.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqcplzjk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gckdauhyi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvjolkjf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gwtdktjfc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fanxiaobao.xyz/Article/details/gcnxfstld.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghygtrdlb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxnzvnot.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugdzkete.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeuhvshn.sHtML

[F08] 遍历目录
来源：http://blog.fanxiaobao.xyz/Article/details/gelziasob.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fanxiaobao.xyz/Article/details/gqihjowtu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fanxiaobao.xyz/Article/details/giiwetfwz.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gcxhnafpx.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/ginizrmzd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fanxiaobao.xyz/Article/details/gctbthqfo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gmsqzvonl.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gymdhsmua.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/guilywqxd.sHtML

[F09] 获取文件大小
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntaasqxo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gjhpxmnfx.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gujhnmanu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fanxiaobao.xyz/Article/details/gfhcoqhyl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fanxiaobao.xyz/Article/details/gbqaekjei.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfueofuh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fanxiaobao.xyz/Article/details/gndnkrwea.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/goxkiulbi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcvgornf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fanxiaobao.xyz/Article/details/gboamekel.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gtektykda.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gayfxlone.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/ggjzkaemj.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyswajps.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbhqtcko.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfffvzeg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmvrrmxi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfndxxzuq.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyncukxl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdjdhawt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyshjrax.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/ghbhdgmwf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/ggbyjytso.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxckgocu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fanxiaobao.xyz/Article/details/gqosfigtx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gukeefqra.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fanxiaobao.xyz/Article/details/gtjztwxbh.sHtML

[F12] CSV 读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gahqqmonk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fanxiaobao.xyz/Article/details/gzmympimo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fanxiaobao.xyz/Article/details/ghuypdvem.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gppvonyoh.sHtML

TS:   // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/ggsnkyfak.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fanxiaobao.xyz/Article/details/gmupkjdab.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fanxiaobao.xyz/Article/details/gdwsmqnfe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fanxiaobao.xyz/Article/details/goknfignu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fanxiaobao.xyz/Article/details/gtusgczwv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grfbzirkr.sHtML

G. 面向对象
来源：http://wap.fanxiaobao.xyz/Article/details/gmdpsfueu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqskayid.sHtML

[G01] 定义类
来源：http://blog.fanxiaobao.xyz/Article/details/gnecmqgul.sHtML

Py:   class User: pass
来源：http://baike.fanxiaobao.xyz/Article/details/gcqbleith.sHtML

PHP:  class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/ginuobwno.sHtML

JS:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/guekraplw.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmbjhsrau.sHtML

Java: class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepkeiaio.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fanxiaobao.xyz/Article/details/gihmnxxyw.sHtML

Ruby: class User; end
来源：http://3g.fanxiaobao.xyz/Article/details/gcdlacqgl.sHtML

C#:   class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gokettmuj.sHtML

[G02] 构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gemfzehtj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdhdubek.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gvsfnorlu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzsszucj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/groeseydo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscrjoepk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fanxiaobao.xyz/Article/details/ghlwrhsth.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbgerzrx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gylfyqhag.sHtML

[G03] 实例属性
来源：http://blog.fanxiaobao.xyz/Article/details/gipcdzsow.sHtML

Py:   self.name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzhlrexm.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gbufvkmsq.sHtML

JS:   this.name = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gkuprvilh.sHtML

TS:   name: string = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxlxpbfs.sHtML

Java: private String name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjucruqzc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fanxiaobao.xyz/Article/details/gadrwyprj.sHtML

Ruby: @name = "x"
来源：http://baike.fanxiaobao.xyz/Article/details/gmdpzehzz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gowvuczyj.sHtML

[G04] 定义方法
来源：http://baike.fanxiaobao.xyz/Article/details/grnyabsye.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fanxiaobao.xyz/Article/details/giawxblvl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guspicywz.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrsbxjeq.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geildamfi.sHtML

Java: String greet() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdaacmhvq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdrbydaf.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqxwytam.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gcuqxrhgb.sHtML

[G05] 继承
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlyxdnlk.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxpuqkwu.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goisnuknk.sHtML

JS:   class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/guormxlzl.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/grwtobzzq.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyntvktjh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fanxiaobao.xyz/Article/details/gryzxqqmh.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwzypldi.sHtML

C#:   class Admin : User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmzcirrwd.sHtML

[G06] 重写方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdhuosgg.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fanxiaobao.xyz/Article/details/gjaknyqvs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gecjnegjs.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfannvzqm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxavfjxu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gunkmimzg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fanxiaobao.xyz/Article/details/gvbihthbi.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fanxiaobao.xyz/Article/details/guukyccum.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfzwewej.sHtML

[G07] 调用父类方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gnglmzmus.sHtML

Py:   super().greet()
来源：http://www.share.fanxiaobao.xyz/Article/details/gviawltbi.sHtML

PHP:  parent::greet();
来源：http://3g.fanxiaobao.xyz/Article/details/ghvqwpnbz.sHtML


<!-- 参考信息 -->