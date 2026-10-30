代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gfgrtvieo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gmubkuulc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gkinssxda.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gjjaxvsrm.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gxppqeigl.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gxfypmlwn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gguzuuhvf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/ggmbgnnbz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gndtzydit.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gqxdnfent.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/ggrwwupjn.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gydcobdsz.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ggtpbicla.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gwsyrkmii.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gskpfzxrg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/glujdcjjw.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/ghsbudtxs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gqaqmckvq.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gxngrpjae.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gdeccxuwq.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gaeifdcat.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gnpfrvgwh.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gpifcjyti.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gdptboqek.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gvwmrwnqu.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gftuquwze.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gsawcpyrx.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gnqnfzwzm.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/grnochmwl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gbvqigmvg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/guflpchrh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gxtlbgldm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gsvxagrlg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gagzhmxfe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gfnmmxtbl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gkqqgdgpc.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gqpypvhfl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gyyxncirm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gizejepvb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gahlmgoms.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gubaixals.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gzylkbpfm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gompydvpg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gbijuusju.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gcelnxkxv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gsuzwkddj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxyekkck.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gwyjznxpg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvkjopztj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gtnmdokak.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gnhifxclx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gvwhwrkxn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gswohlxwt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/giakbtjhh.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gdheyppoo.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/glbqypbuj.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/ggukycpdq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gpawtsmid.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gvutsjtpg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/glfpqkkgc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gtzmhsdox.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gzijeasyw.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gtjxbjxvl.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gmlustsvo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/ghhqmgerb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/grfxmwfma.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gavkudxmr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gxbuaavve.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gmccvwygo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gmukdrrkz.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gatadfduv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gremyxzlk.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gjfwtaipv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/ghrfodleu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gudgdwyao.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/ghiuhqgyl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gwzdurcpl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gkenmhoym.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gnqrhnnhk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gxknfsvwv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gdmeupnjo.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gsgpkeirg.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/glyfqlodn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gxhaqusfg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/ghtugzwfp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/ghfcnyaib.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gsyvvketn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gyiibgvsu.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/ghxwltvnw.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gjiaycyfs.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gcpelpevd.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gposyuivl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/ggvikyleh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gliuzdueq.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gvgqmbgkv.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbslhaknj.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gcgmkdyeu.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gpbubegiq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gucxmesxp.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gupxiubdm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gxatqbmcv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gxiumqdpc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gsjvkkhdt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gbgclxkun.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gsituxbld.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gjvqwbwjz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gyrynkver.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gdgeeuumy.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gjdkgpgfc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/grudlwxrc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gelsrwmft.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gzgddrwrl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gpzqppery.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gfdxhhpko.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gdghafrjt.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gddumktun.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gxcjshtql.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdjdrrcwh.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gqcgzxkhv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwhzhjvii.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gftnjzqud.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/grugzzxag.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqjomeust.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gyrxzayxk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gpalmihho.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gkcndtfyo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gvobddfnv.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/glfxdfrqg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gcyvtwqdz.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gdbekhgcv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gennrhlwy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gsqcavnez.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gscqmkydv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gonrdkxpj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gglklioin.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gglmqixkp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gppucombf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gzffqrmuq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gapjscsks.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gxdfgizju.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gigtwhsnw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/ggyhucyfh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/giookijhz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gbqaqkmit.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gzqfeoxhi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gitrnebaf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/ghnldhprt.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gynnmiqgo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gswccfxue.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/govfgvxos.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gmjrkxqxc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/ggvepdbdn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gwqpihaor.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gnxlajngi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gtmivrgvs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gqxntbdml.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gultwuxlo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gurndhpjh.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdcpaceti.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/glrlsfwqz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqfrksumq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbsuhecbs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gqflxbucc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyiqmmdkw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gimvrwhcy.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gofridujy.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkopveiod.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwpgvwnog.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gckpvdaui.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjxatnnyv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gzowtoubv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giujfltge.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjghxnbpd.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gcdxyzglr.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gzcxkbbaa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/ggjxoxzau.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gcsnwyjhe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/geaejryyh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gkuczmrkc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gqblzngmz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gjjcxthdp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gbycidneo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gcaynbjpq.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gbgeyqney.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gwjlqndfv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/ggllongrv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/geotpwggv.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/glbmluyca.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gayqtymay.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/glyadqodh.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gyvpjzozm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gsazdywbm.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/getvxrcjz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gciqwfqvj.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gdsgcwakw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/ggszimqyg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gcsizgzkb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ggtzcjmru.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gyebjxqqx.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gglpajukt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gmrtuepfz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/ggyfrdnkq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwltuthjy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gxptptqet.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glomvwsse.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzginqcdh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/guqyuipyx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcfnesdfc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ghkwvstpk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghyfjtgto.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/girlkjyvd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gtssgeshi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gpuhdzcvh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ghtsbmtfc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gcvkgigbx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gjuxnnmzp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/ggqehwkul.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gjwyujqbm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/ggticftis.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gfypwolfd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gsqetcjvk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/glbsopawg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gsknavwfc.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gesymenbk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gclwewenw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/ghzzefars.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gofltnlig.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gqtvfynui.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzogumoyb.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gnjcokdvm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnrbwgykz.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gaxgwbmag.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gvmtdpjmq.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gqfxlijgw.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gibpltkal.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gabdrmzlf.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gblllhwzp.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gyiwwkmbn.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gpwzsgnjw.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gnjesmiaz.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gnysigkow.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/guoxljlup.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/glulolapg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gfzmbwowl.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gegawzlyt.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gyqjzeckk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/ghxvslori.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gecasxmhl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/geiiktojf.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gugsboxpw.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gnobsizwd.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gmihrejkv.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gyhjmpvzp.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gsototcsl.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gcwbspxfe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gegnxakrf.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/grlqmgoap.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gjgpyhavk.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/ganwysqmq.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gtugxxapc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gpenjeeoo.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gmnififtr.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gxotpnnsx.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gerhxukzv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gouxpxmjw.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gjzawcheo.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gergjncor.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gtyvgoodd.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/ghttmkdfe.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gnjshpklu.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gvqllitmm.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gjqrldhzx.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggijguyql.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gdpuairqu.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gvhoafhpr.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gyquorzhv.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gjzgzlcrv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gmyqrpgzq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gsrsbwzjx.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvipfagnm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gqtxwdify.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gbxhiluks.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gfkihdfmz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gdzsrzect.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/geauirwcv.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gqsiovmgc.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gdmbyqsaw.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gtnertwtt.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/grdtdfrnm.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gygnuijwi.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gyghyrcwf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gsrboawqd.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/glyaawlgy.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/glkbyqsno.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gikcctavx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gsgkezcwg.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gcuprneix.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gqngdwurt.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gvoqakyxa.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/giwblbsln.sHtML


<!-- 参考信息 -->