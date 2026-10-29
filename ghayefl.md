代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gchkhpwdr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/geeifslmu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gjmegktty.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gktzykchd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/grjfltyqi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gqncakvdl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/ggjqlrzqx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/ghxefifjs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gzzxjvmuk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gkseqdvcv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/ggxedixic.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gmcmhjtpt.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/goscavalh.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gcmqnbnbu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/guhdmunqh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gtklofanw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/grwuyvmsq.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gdvqixwnh.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gqyslvjfj.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gladvjrfk.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gkuzvxdxz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gracsnjxq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gpokpezvt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/galhqoynf.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gidgvymbq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gvxfhvuvn.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gjjcoqpyt.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gyfbyivew.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/giowpfyuc.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/geeqbmamy.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gaqnlkssp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gdhhrwick.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gluiuljxi.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gpgmocjps.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gbpldpaap.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/ghubludjq.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gareuhzjc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/grmnxfomi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/guqjsiexu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gkqlbhvvr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/giotucwhi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gmnjfqeza.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gkaoerreq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gwcfahjkh.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/geosuyuwn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gvmwamiof.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gniodmqgx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/ghcrwihys.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gbbshzyja.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gkevspqwn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gvyyghtoh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gcpabpnab.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gfgfzhnjb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gqqitflmb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gdcfnhate.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gzynwvczj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gvdqrwrrb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/geyfexlcq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/glbpvojph.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gdvjqttib.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gkynnfhzb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gddrmmyyc.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/guqxqpdfu.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gmefnmswi.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gdgdvzkpq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gtoaaaiss.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gdcmzfddd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gfmbatbyw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gwdcumfru.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gtsuzjtie.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gveudtuws.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gmwwhufdo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gngozebif.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gcqibnmsj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gccuourkd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gfhukdost.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gdqbjmhgx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gltkejhvp.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gzknkqysc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gpcdnjihh.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/grbhpbnho.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/guuckcxnl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gxbgzaxwp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gpoqackxu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gtradjamf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gkucruoho.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gbgqcgwqx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gvywfopxj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gkynrginl.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gjjzgnrdq.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gwqxlktjt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gsqrawski.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gbgmtnzsj.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gtskykpma.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gojpbpmlp.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gaivkxpon.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/grflhhfdm.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gxkdyhxvq.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gxjfmtloo.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gufvcgtue.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gyvfjuhfv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtdffvriy.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/ggffziqym.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gflenkdxk.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gjnzqelxj.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gzyrbqfjj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/glutsbceh.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gkflfltoo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gjhbaqnfn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gpmgjekhk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gnvmrcghj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gihebrpgh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gtstjttia.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gqclytxje.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gbklszvtd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gnlazwjtd.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gbxvusacy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/guglgwdvm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gyjncvcil.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gkltdyqua.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gwaodupdy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gooecudox.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gfjnhglyv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gcieumsjr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/grurnscax.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gptcrhnbp.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gkkvgdsgc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcdzupkat.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gcfeqoyqe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/galuzweiu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gusuwygib.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gncqitkoe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gdonwefwc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gszsoktrh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gutycmecn.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdxjagopf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gdvwqbczo.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gihllqfcy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/githaggmr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gsfanghwv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gjigfjekd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gegrvdtvi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gimyiodqv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gjdqyllre.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/goeignhyo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gjbbzrjjq.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gfhxhgvtl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gfutucegt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gtlelpcol.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gvxcjwtys.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gsemehfgf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gqcijcxft.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gopbqzqfn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/glkpozjjg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gfssyzfxr.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gpwafzqbf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/grzpgjriy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/goamfokqb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gvipufyfi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/grfvmhynm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gdbqxznjk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gosnaekbl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gkwbmoofe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gaqlzflai.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gjcbiutbi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gewjupbfj.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gzpolikta.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnijcfaxl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwenqphlt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/glfebucza.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gmummoycr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyebcwxww.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsbzigzlq.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gvjpxllcb.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqudxbfrh.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbmbvxfkm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvmbgovsf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkmnknvrf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gkocyafbl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gshogmqfp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtiwehllo.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gcyqpgttf.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gfpzwlbbx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gussuckea.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/ghquliqqy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gzragetqt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gsvxurbey.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gvojftcpn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gthladkgq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gevukqzbw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gfjmwvcls.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gllocqeji.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/ggkusziuq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gwwxwrzwh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gtjbcinrx.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gcyykoclb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/glrtzelun.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gtglmqyut.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gcvcyhkab.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gqeypdxxm.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gmxfgrtkd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gewtbqyfe.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gjmvwlyth.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/goxvoipzt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/guawmbfua.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gejdhrfog.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gixnrzrzz.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gztxzjbhl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gtaczzsfm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gwdotramy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gflswcpyk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqpticqrr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gdwtxjvnp.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggquufbox.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gxubwcmry.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gswieizyq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/goyffwpiz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gwifvhvzy.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gzorchwmz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gqgmuwvtw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvhlekozt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gurynufmi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjcyhntzn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gvwuryorg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gxvkbwggm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyuiwcoms.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gvwaspdxs.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/grmlsvpux.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gpnbfhlnx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/ggiugyobf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gqyryohfj.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gnhiraxqc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gqqpwxxks.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gcmbxyrso.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gwygyiumo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gerbbxcxu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gasgbjtyt.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gomxnrbcg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdzjwexhy.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/ghdawkxak.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gfdiavdmy.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcoimmoya.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/ggpuohrgd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gvvjpcwcz.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/giumwbbua.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gkednuecg.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gnvdwogjl.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gymbvrtob.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/goxheansp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gygflrmbt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gucheztgq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/ghdafjzpd.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gnbmbphom.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/ghlusgeae.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gcscvkdwu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gwpjmxirg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gisuxcbdg.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gptbxsxck.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gxcqllntq.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/goyfmzgxf.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gwnpcmcby.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gocojotxu.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gzzgcgxsg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gjctwvbwy.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gnnmqyfpn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/ggynaqpab.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gbdnyxmkk.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/ghggrcpab.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/ghrktdsnh.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ghalhngna.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gumzjyybi.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gxshjwxbe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gxnucxyfe.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghoyqtxec.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gleeedooh.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gcvpbatrz.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/ggzkheekf.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gpcpkaifx.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gkoausdyc.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/geqcndryr.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjytnbhru.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gwedzqoxa.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/ggjzlfwji.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gyumefozx.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gsjjvbylu.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/ghmftrfjt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gtlboxvjs.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gnduwzzpl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gxamdbqkf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gdsamolgc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/ghhywfbss.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gkicazyql.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gzsykruar.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gmvdoitbw.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gtanfuryn.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gfmaoionq.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gfldsykxz.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gjytfgbro.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gukgnijck.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gazivmhsf.sHtML


<!-- 参考信息 -->