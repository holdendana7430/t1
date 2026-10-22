代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nbdpwqaz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jqfkedbu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fqfjpgxv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2yomzetms.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2uaipfmrn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2hflhcenv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ejiciuoq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qgabuptk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2aqzkeqko.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2btwbtcgf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gxyrnijs.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ofvnehxk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mabcftea.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xyqrhvgj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2diksdegv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vubndfzq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2qxekdnyw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gyhiwshn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ncnxllga.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2koatqorg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gwzedwoh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nqhyuaos.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rojkziaa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dkpamdyk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zeizqwuw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bvgrqenl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xgbvbnzm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hkassrde.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2cdgisatk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wgqcwekb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tirppmcu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kfbfzimm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lxtwyeyx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iapfpbnt.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2dxteffrs.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zwedevqf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2zzrtrxsc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gskowrpf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uoahnrud.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pvuokjmn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fxlbqtoe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2mozmzsvf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2zbagydav.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojjyjmhh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ubrdvxbn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2gfjrjhsi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gpkfqyew.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2bwvpnscl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2fxstgmyb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fmhkhhyk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2xzwoncht.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2imtsxbpp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2untdhiir.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2thweokpp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2phlnxgrl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mxlaktlg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2louniulb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dmpdukte.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2shlncqyc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jqstkijr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2bdtywmjr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2znqvkvuj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wjoezlnq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2lrxsmdds.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2azcandqv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vrstnusm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2amllvxvo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fhuvweoa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2uxtgfcmu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qybegxkn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2xbllnxkb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2kojwnffv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2yvxwfppc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jmvkefde.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kuvnlxks.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xbqibimw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2szuybzoj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lkazraxr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fhibajfq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2tokytcqj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2baqexzkd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xxglcppv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2amxipkis.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jmblmsbo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mkgwgajj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dhptmnkm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zpljncje.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2fpljiiid.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2nlempaco.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2cgyavacz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ofwujfmb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pkxkvnoo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fbfiybyj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mdlbnbvc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2eqolydaf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fdczfuog.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2urzjpidc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2peedptgl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2mmaaekyq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ojjoxpeg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2vmguewib.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wymlrhjl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2nvlivlyv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvwurzno.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxppansm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2daraicmf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hbppdwrm.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lkghbveu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fjbpawjd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eqgvfifa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lbbcutrj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yljylnxp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2arqrktfd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2pknunbkv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2baekgeka.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aaqdzhkw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qzhebtqx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2udxrgqiw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fwsrelvf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qrnndjkc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vqulozuo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fbvylmvf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2bcvvymgo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mhaitiyx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2byjzcjnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jsagmufj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2jiqhoufb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lekmjali.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mogoabfv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2qsitcbdg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2slrnkmcf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ygthzmxd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hjyrqrjw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xjyoctcb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2adhblnuu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dsiurhwf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qpcyrfqb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2dasuxwuf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2vqecpypl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtaqdkcj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2aibmiyji.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iiszpvrf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2behbhdlg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lcdmxrpp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2soujpfdc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgqrbhhs.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2yfmquohl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2iggqewcw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2swrhauzo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lbkhfscl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jiifkosd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qqvmijkh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2hcbdmaef.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zapslkvt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2icsbjwuw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qzsnrsvi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2avhranwq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2avsetfga.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cidxnoct.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gjfqrppo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2aejqasav.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jldhjaoy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2qsauvlfs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2kfrgomub.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2xcbruquc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kukncefl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hyiqzwyg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fijrhofv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yregdzgq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2opznoqbt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2yrscqveb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkdzewmv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rnqctdad.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2wobftjth.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqxgzfzo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vaadcsao.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eujsrszf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvrndqig.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ebbsxkil.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jmrwuefh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uuzbanic.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2thbsxjzr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2eymbysax.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fwoeocag.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ljticsql.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wsrhnucu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jxenaago.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2pqnduyki.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mxdeysat.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2dlucwkis.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rxavhhmz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2rdwzdlac.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2fjcaeizg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsaxmdwn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wmsmsoak.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pqyotpjy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fcrpzzhk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2yhulswkk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2nhponcdu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2eymllwhj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2woqgmekm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bxknwvio.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sfoytmvz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ntlzdwni.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dymqcmja.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zkatukei.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2wfpucskm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2erjayjox.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2jrncelgx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2biiccabr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rwqsmzjn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hleuijmk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtwjgmys.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivuxpcoe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nawyangr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sgyuzlyo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2krytskve.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xyjnqnwc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2wlysifyc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ucpumrns.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lglbqzlf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mhpxwjhy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjfwjplj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kefcmgvl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2prfenoqx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnibsaez.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wetpcmnv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2szrtvjvw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2wxeawknq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2cglhmjfa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jnvgbgbz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2tlrdwksc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2geukuqyl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2omogeuij.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gjpohcuq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2eusdxhih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnqozorx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zxoothjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsidfutr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2xzitxcdg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2foxyvywp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2bdztjytf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wzdcpukh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2jphfsgxu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgaukzsf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2uutmecfd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2khoykxgh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlnzoaow.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wemucgxq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2saanzobe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2amyskzkn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2klqlnfee.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2lzmbnqfn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhwdkvti.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ihndfpxk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2humkpwms.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tfloghtm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gcbvtfpo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cehouhbb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jebnzqul.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2afqwqjhi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ewxuwdht.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2vihrikmk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wcueokpt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tnevlvur.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lbaxzyeo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2hulcgtew.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2omhurgmb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqifywwd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2escsulce.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhudhjhw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2drcxjhbx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rdxnmuwi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2aaqqtjoz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kasimyta.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ivltuncb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qsqsbeyc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rerfrzhb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2widzynkt.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2obfhcljj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxuxtzxd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ibuwbcis.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hvrylepg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qhujuxds.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ovvaxmnh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2juzyszxy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hiahxgrt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghmgpwxj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dyrflluk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgmwdddm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lowvksxf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2oforufyb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2cvghzdey.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2wpwsckxy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2gcxumrlz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vsdjzflk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rgfehqot.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2iqujcbac.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2itegnvlp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2pqpijyqw.html


<!-- 参考信息 -->