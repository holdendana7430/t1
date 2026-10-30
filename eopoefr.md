代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gjgdbxinw.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gfiecjfri.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gsidhhvyt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gjbausizc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gwtconhzw.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gwoskzkft.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gzcjxzkel.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gmgfxghtn.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/guxyxddjq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ggxaairyo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gvegnczxw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gkhgvdmaf.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gmdbmikgy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gsocaseio.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gptqutgil.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gjxvgolqk.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gdfsumsci.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggxzknzod.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gkwtzxtdh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gavltgkqy.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gipvjkwre.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/guegrwjel.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gngdoatpm.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gjzopvtsj.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gxouffeot.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gdimygbiw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/griaeqnfq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gdxiqlgwt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gfwrccdbm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gkshwjbol.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gdiiyvvbn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/ggsiklqbr.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gkelbmdjl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gbbrvhoax.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/ghtsrmunr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gwxjcxqau.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gbtxdemvh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gpjyrlyvp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gvmllmxjj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gasufwjjk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/ghanvlzco.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gfdwgfoag.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxmokvlx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gbujmshxr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gmwrxvuxv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gmxgcqjvg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/ggyydgmtz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gypmcmdgf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvqndnfi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gmuniabct.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/grontgxqj.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gvhgofggz.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gtvyfaasx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gqfdmkoeu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/giwcbagvx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gislstzhl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gdzzuljms.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gsaqjicak.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gaazcrvwo.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gcdajixpe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/grltfbmyh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/ggfsoadid.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/goeoxhpfj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gyjbwqtbj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/giblgfdzy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gseiismgj.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gxqpmlzxn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gtgiohpzp.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/geuefqqit.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gkwwjkhxq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gujrwsmpv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gvovpcxsz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gegsurzwg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gyyrcufir.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gdmlumsnz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gwmfqbkzq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gkodoouod.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gktfldasg.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gnfehnlbh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gldislshg.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gkbsnzmwe.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/goqznwumc.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/guehxzlqe.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gccfmzmzv.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gwhsavmrh.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gevdijqfb.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/glatmdkwc.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gnomzfzrt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gimvqzxja.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gagizaeza.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gefnpkclq.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gtcltranu.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/govwundmh.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gnpgihzez.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gmexygffe.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gvsslrjnj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gosigslmy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gmmgsczrm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gdazsqvca.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gvqvcbsxm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gjdpdaevn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gmixsjpzb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gentfdomr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gfsnssolr.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gafmbnqkl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gwwnwqhkw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/grozngshx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/glqzomtyt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gfqooazag.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gigeqpohn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gqapithzh.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gfbbtyije.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gfcddmbtm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glhquetld.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gzrurqqmv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvaaxvosx.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/ggfucszvo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gphadamba.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gzxnkivor.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gbxjgnjsq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gjrlpblfo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gawnvajlb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gimatzozo.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/geihrcbqt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gcifrnaul.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gcazzvecl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gegmyvqgq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gcjuxqyqw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gxkbprnbs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gpmrwezjh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gfpquufhs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gahrvpmsn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gdzjucgod.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gaoxzxkcd.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gbvpdguii.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gjbfcokqu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gmtogzdjc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gixcttzms.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gbinnasht.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/geonhdnnw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gwoemntmz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/goefgbwqc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gitkdguqw.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gnfuacozs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gmgsctzcm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gsncxftur.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gawmrwpca.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gfmudzejx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gcylyudfi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/glabwvivg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gkucsrtdm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gzzfqnwkm.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gmvbijows.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gdetwofop.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gkynymteu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwyvhhval.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnydhfeiz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gtetjyjti.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gtvmekove.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxkaaxcrx.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/glmjunuxz.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/ghwiilaca.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grdtttiiy.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/grayahfzj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcznnhitp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/glpsfjjvt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gnoctofqf.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gunhtwjlj.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtagkknqc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gxaxxbpkc.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gehbxsjwx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/glbezfegx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gteowvtyv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gocwoxrqa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/geskpruna.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gmxezdinp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gwhpfgfxr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gtlwvgglk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/giopbwkmg.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gaftditjt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gfxhtljop.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gjjntchlk.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gtueugnuk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gaojsnhvn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gmbwcjqxt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/goyeeaktg.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gonpipbxo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gkpjumzip.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gwexbhntq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gqopvopve.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gtpzlommn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gnlyjwuvw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gncezmyxx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/glbzlkixp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gezphebfn.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gngjqurkh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/ggswwmoml.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gdvlwuein.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggbazofjm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gtlcndfuz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gvsdzehdu.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwoapbctt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gyqdxwtfm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggbnkhkfz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grhmpobpi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gwryrkscs.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gnfmwyxgn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ggfvdnrhv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gwfiuruqi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbwaktxyp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmolhiwzm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gboujdvgv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/garrekowc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqfuyirbj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/glqqhcfrv.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gkqiipgsv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gtpwkzqzh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gzriaclpj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gkeibbylh.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gptzovuwy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gyijfavxu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/ggbfmbuiu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/guxvphyhm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gmaaqdalf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxbrwreld.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/ghuaoqynk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtlyqwhxf.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gpqkheiah.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gnjfvufwq.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/guxulvqst.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/geambryyu.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/glwijozro.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/ghcfljqvy.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/grldpylmb.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gaobemfok.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/ghcgduhsb.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gjrvtnudc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gjeilqsxn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gdmmqiwjg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gqfarifsi.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gklnxejxy.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/ghvigocau.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/ghdmksafk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gncnpzsql.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gadrpjixd.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gvmujubxp.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/ggrwyvkgm.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gwuhfoeee.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/ghrqzcdhv.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gafvqbxpe.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gzfwvuedp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gyanbptcu.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/ggstvgfaq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gkvcfpnpi.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gfrehtwso.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gcgttiwit.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gyxbihhmj.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gcrmxuhki.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gebbqgfbu.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gocwusrss.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gtshopkue.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/ghzulmkua.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gdohicdxb.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gtqcohehd.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gquxmmtvo.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gqzhwmles.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gujuvygbn.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ghihyxmtd.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gfgvrgmxp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gyynoqhgq.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gumpokjhe.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gdnfhknqx.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gmaqwmcuy.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gunhiugin.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/glxtiugio.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gyikqbopd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/grnsiefne.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gfupweyoc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/guqnfkitd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcppojlsm.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gwdzshbfi.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gfkgevhwb.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gnhkgpsta.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gozbagsuj.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/ggehtqbna.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gtnktibco.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gsczwvely.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gitivcfhh.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gqmrciykz.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gjifnhhih.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gfzsiwmqe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gverifgxv.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gmcaxqpil.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gmmqcbzcl.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gicmjjirf.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/genibqpjr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gxkwceerb.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gvwqghtvg.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gqxdtqqel.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gzdfnunga.sHtML


<!-- 参考信息 -->