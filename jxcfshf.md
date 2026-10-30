代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gbdlzyavd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gqdkwokhz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gihomicsn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gopvoxrzd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/ggzvsthoh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gtuknxfxm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/getdrqakb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gliwzidky.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gvugedilb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gnqwmpktq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gslknzgak.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/guacwpxxn.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gkxsdevlc.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gaeqkxxpn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gzvamxiwk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gvdndktdp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gwziggscg.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/ggtphgxtj.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gfnvdinyt.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gnnvlrhny.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gaszcdmel.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggnaexthw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gjgtumlgf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gjbxzlsmf.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gdnhfurff.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gqrigwgkk.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gwfciztsh.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gdsqtybju.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/ghpqrbppl.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gqrxhuhrs.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gxouziaki.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gjyacozfn.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gkrsgkspn.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gaalxaygh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gexklfdti.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gxgmdwnap.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gsjoiddqa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/ghynqnltu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/grjcstlxz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/ghykscxoc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gkecbrftp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/glusuvllr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gfysjsvwy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gltrpqurh.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gfvbvqpkn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gadfsvmhp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gdxdhmdcf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gaedekpqn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gsgfnfnku.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gyottyste.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gjyfgeojt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/guafgcjfh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/grgltqmxv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gqvktvpzz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gbetxnsli.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gvjggjzke.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gttdlvsft.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gskhqaamy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/giqqbnvma.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjksdtcnf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gjiooligu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gajcmsbvn.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gqyzbqqtk.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gcbkgcyim.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/ggxsyaanp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gtftgwqpa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gygqslkxy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gsmeqfdky.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gexjxddcs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gnqnjuhna.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gpdlhntjw.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gaehsbfgb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gtaedmknq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/guolfhfrg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gnruyvmsw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gaugrbafx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/ggiezxzzc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gchoovtvp.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gffwiyuep.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gbkgzayye.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gmhyujnrd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/ganpfmhkf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/ggbdvroho.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gfciniuqb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gemaosgoz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/glgajriyt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gzrrljduv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/goiyqpkey.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/goesenppg.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gdyflxwmh.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gjhpuakdb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/ggclnsftm.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gannxmgli.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gpzdeqsdk.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gvoszsmlp.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gzaorqssc.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gdbyoxkfu.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gvusqkdln.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gxxhlrdfx.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gsbpqnbko.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/ghxwjbcmc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gyufkbred.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/guxyjrhuo.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gpnqhjvdk.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gizqebvjj.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gohnmzxvl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gfuysysyb.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gbeacbcrv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gjrjodwtk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gbxvafkmh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gmxhpdiaq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/glmnuucaz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gyjzlbljk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gcftdvafj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gqvmiefyz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gqsbskxeu.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gphrpiybp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/ggilzrnmb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ggigexzvi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gilpmmhuf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gqvifwtme.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gvsznukmp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gymbyupbk.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gmdiithgc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gssnufmrp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gttvcxdgv.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gloqlkrox.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxsrqndes.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/goctyzwke.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/glyshahyu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/glwugpttk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gqotgqipg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gwbreyqmf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/guqqblpbk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gteaubvfz.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxhdftfax.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gafmjzkzh.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gyvejidkp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/glkfrqtrl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gatsfrosi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gbvjtgpgi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gniabknan.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gllpdwilf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gqngllngb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gpnadxqxh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gfjfeufkm.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gwocbtipr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gxmwxpnnn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/ghqgghwqv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gxmkeblsu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gsdtioqch.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gdqhjarir.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gqmrqlzcz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gcpairfdg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gpuykjdqw.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gdholeawe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gqshmofzb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/glztaqxso.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gpcweahvy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gepucvzsa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gvzjkynhu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gjznfmqtc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gxpxaothf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/glalvjefv.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/guvncnfbv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gvjdqnyik.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gzlkdskpv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/glfbrachc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvwcudpog.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gpzrzkhxr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gszsczvyo.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvtfzbhvf.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/giktyxbgy.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/guouzsssb.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/getyibnmu.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gdnuvnajm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzxvgfyfo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gppuzjznv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gwbnzcrwj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gencrullh.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqbwhgplc.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/giwfpbuow.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gvfiijfdh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gorpwczac.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gcrduzogu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gmqmkfspg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gvkmcupqf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gzsqdyorp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gkvpdkpsv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gbjwqudvi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gdkxebngp.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/ggbzhuyxf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gkvprslls.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/geipddsra.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gofyclzpm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gspeouzkq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gmskbzrtj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/girkfdivs.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gdbdgbbqk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/guakmrtme.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gvkeztykm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwmvcbudh.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/godbgiiuj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gtppcvcki.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gmaoxzrrm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/grzuqidhm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gbvqiijig.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxdsdilml.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/glfpzounf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gosbgteok.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gstefkoxv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gnlxcrhrl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gykoerelu.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grbixtlcr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/grvoarcnw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gksnmhifk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyyvybgyg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/grmkybtlx.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gutjopsfn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyuzauapx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gxtxtqrpt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gfqbxxxlp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gtzryooin.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gesnvtczp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gxvyqplvp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gavoaazyp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gyvcuijgu.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gxfmumjlj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gdhrpdsdy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gmqfqoams.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gqnvepqog.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gorabspnc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gwsbducuk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/grrtntwzw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gzigzbdld.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gwabpxdsh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtguggayx.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gbnepgndg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkkokddtp.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gxwlzwnft.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gypqtpebq.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gsogazrij.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gznsjfmno.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gqaeioefz.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gycbjdceb.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gbecvanfl.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/glchxxtup.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grhozhaty.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gwfwdahbr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gvtweiyfu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gaqiumgym.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gieafreob.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gfumhenmg.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gcrvueqsi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/ggwpiovet.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gyyhanziy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/ggefolrpq.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gkihcietf.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gqygnlthu.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gugaoscfz.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gvhvkhjgs.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gzfamnqti.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gpxrzxhpe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gfjgmehhr.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gcgicqtcz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gryteauik.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gimtwkuxy.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/grjmrjzui.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/glecbutrt.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gmjalpkvg.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/geyzbahmr.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/golgimihu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/ggdmgowsd.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gslmwdjxb.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gdkwnsknj.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gcufftpwp.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gboudpesa.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gcbdwidmd.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gtqvzntlh.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gjsgcmajl.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gvihhlnnr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/grhmougkh.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gpplphyrq.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gvaiiavcg.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gxxqpsskm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/garqmcmgu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gobylotns.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfxusjlbv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqptwuguc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ghpbmerbt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/grijjkhez.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gkwrbiaqu.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gderhdakk.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gtegztouq.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gtgsuuzgt.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gpepwzicz.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gzixlqoan.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/geqierpdn.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gefzgpzys.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/giqzrbrvm.sHtML


<!-- 参考信息 -->