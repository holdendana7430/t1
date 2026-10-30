代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gohmrnnfc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gfafsyuue.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gnschdzbz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gitzfseya.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gvzikxqrx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gxgiudpap.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/ghslpovxt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/grkagjwra.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gguczzgdq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gfdnkwnok.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/grwghkqwh.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gayabbqjv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gtzhnrtuy.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gsaehbenr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gvcygpyvs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/grdrvqrfl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gmawwnydg.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/guhtcpvzg.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gjlclijgx.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/glkwxrafm.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gzkwlcsqh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/glsenatkg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gbdzlgads.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gulhyhsbo.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gozemregr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gfdkycgbp.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gmijuuogr.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gusbkxyus.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gawlzgqxk.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gppqnzavx.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gaoetvfkt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gqhylejxj.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/ghujfkqfe.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gizewhxuw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gcohdhcoe.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gzyblbzae.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gsajyoedm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/guvefclby.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/grqxzkqmn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gxhcghzqz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gdgmllijt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gvhvbukvu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gyjhqkxhw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gvgpnjhhp.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/geuibrmor.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gsfyknffb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gnkgnbmzx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/getpqvwgx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gkpwlnwzm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/glbzipeau.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gxlckkahc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gagbewtnv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/geitutsfm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gennzguhb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gnfbadqcl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gtrotijmz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gpxyoyueo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gltpdpgzz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gatysookb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gvrcndlup.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/glqilyekd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/glxsxhqxn.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gxfatprhg.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gwuncevhw.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gaqxjyzui.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gyoupkrxy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gicrokrue.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gxahenogz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gwftjlnhu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/goqpftanl.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gydehiqjh.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gppipcjmc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gpsgintnw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gyusuttyt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gmzejbzjn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gekdopkwu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gdtxnvqbn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gtxjoavky.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gcrybokmr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/galogmuin.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gazdmdilg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gzmrbiqtq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gphwbwgyy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gasppxdxu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gmzeftwfz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gofrliuyc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gfgcixjqj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gfsxvzgiy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gtdjbvvsc.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gjiadjupn.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gvgmvruvc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gnwiregqf.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gatjqsxas.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gnmadunix.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gdrdrzdlw.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gbonanxwo.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gevasqkmj.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gtdndqhvn.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/garfpdanv.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gfodeidhk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gqeytjukn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gtpusxffp.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gvpyvcvcs.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsjbaufqv.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gtnbhwckz.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gpyrjjazm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gqlhcgtcc.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gmopiauhi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gohzfhgno.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gkzvgzeia.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gxxoljtyp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gracphcnx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gnnqczspn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gxlpymvkh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gbgjbekkg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ghywqhdbj.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gjgnnvnxs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxlqbxpws.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gtfqjxoyu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gotpomtzy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gengepyiy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/glpwehfme.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gychtygaf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gmgfnftpl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gslfzffgs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxguzhnwt.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gzxeqfwfu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gigxpxctb.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gekfrbxit.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/glouyhjxl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfbejlwfc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/guttexvhc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gdbctanvm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gxrkosqmw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gebmaqnzu.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghzdhtfff.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gfmzoscvz.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gjxlfleiz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gztztantw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gygkzrecz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gudhiwtvv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gqochizvt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/govlqdrqf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gjfaiyton.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gzmtyyfpc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gdxdbpfql.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gamqxczjc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gqaidfpbn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gighxysuu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/glkcdyyix.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gjrcvwdcu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gyghzuuuw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gghjyfmye.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gzwbhksjy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gelhqvncl.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gaqxyoaax.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gzzmnhwtc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gqjerswiz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/glftvexqw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gtpnepmwp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gbbrlpymn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gxwttnjsp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gyuyxekzz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/geoyunmbu.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gmzkjnuio.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/ghrhecvsf.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gfyeotrbx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggvjkipxu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/galuulgkg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gsgevrjul.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gvssweubd.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/geuvaevak.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gueffasof.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gjzvvlhei.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gysiuzzqr.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/giicvkeal.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcaqxndct.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbprgoqeu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gzzxewhsx.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxovkdjki.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbkqfgnlg.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gexwyunxv.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gggobbsnx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gtuaxftye.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gllqcjxkz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gjzxaqyzk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gzcbborvb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gzhdxxehe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gjxuoyrry.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gyzrzelhm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/ghtfbxapj.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gfczltwkb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gqdsiybja.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkpyhbvje.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gecbferwf.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gbduzupez.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gfroxfrvl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gggnvkjpw.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gazmyttmh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gvjtyjqeh.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gkfhaefun.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glyipaqel.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gcdbnpjba.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gtlthgaaa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gllnkzrik.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gsfqmsyng.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gmpheyqlv.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpxmsnskv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gmhcbplau.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gqlfygnpq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/glttjlfnc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glfmfufdh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxhzyerix.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gikekeafn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gyaftodyq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glokmgnjr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbgzwvxgy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grlnarrqw.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gbowwajrd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gjbefkgln.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/ghxjzuznl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gdvizfchf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ggicrijth.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/grwqofyxu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gpimcgept.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gybmqcboo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gamneljxp.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/ggjwkflzf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gamdfmuho.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gggubepeo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gcigjzzgw.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/grbhkmklf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/grhlrdszy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gdjcmtefn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gkfbvqayh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gmetcqiep.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gswtbkxir.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gajmjepqn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsxrrnfqr.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gasciwokn.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gnueejpns.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gvcpmtryg.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gdbkfaril.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gyuuvktbk.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gkmwiyzmo.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gfojajgod.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gebzfwkng.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/ghdyxsusk.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gkxphyoje.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/grokjjesg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfxnwltxj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gdyddnqws.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gmdputmyq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gurziokru.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gijgbrrgw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gjqcqjzvs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gntzwawaz.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gxszhvxyi.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/grodsiysu.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gqbwnnpff.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gkfajonkt.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gzoqjvhaa.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gjslhgzny.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/ggocfzpma.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gwjjabsqm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gfvmdldgx.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/glgmfoykw.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/glyluwesw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/ghjeelpwm.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gtbzdeiaw.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gtxgyyuuh.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gneegjzsa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gxtwcjsqy.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gjfmtpzkf.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gdoypolha.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gegenkmdb.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gfudwyuvz.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gltfhrzrm.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gmmnmrakj.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gezpbncyu.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gymvouzfv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/ggjxikwvu.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gpxvsaduq.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gradbxcls.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/geuwrjrvs.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gdylyhgxa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gppivstvi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/ggpdotukc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/griryeiqk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gsrcjlpli.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gqkmnweet.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/guzzcgzpu.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gzzzthgqm.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gbxwxigph.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/ghjkgmabi.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gwzptaspy.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gcbsxsmcz.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gznxdxzeb.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/glgxjkmrx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gvyvlrmkb.sHtML


<!-- 参考信息 -->