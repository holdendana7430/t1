代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2batvvsro.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qvbmwwwf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lvqnnfom.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jzyffkgs.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2honkmknz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cnkryffa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2jqrqathi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2speotazd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yxajwcsv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fqhzkrvy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uqnaayuq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ebvvysul.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2cryatehv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vfumqvwu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qpsybwif.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oodfuuxo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mygjjttt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cmbtjpdx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ssvhmebc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2iwpsqhti.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dwvivmex.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dlafzjlh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dkoonlne.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wmellpys.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2mhngtmrs.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nlczuweg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lrctdsyz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2axpqkfse.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2padiksif.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2accvubej.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2cacgegxs.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2dfotoysh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ixyctcms.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyzrsjlj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jbgzxrrv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iaxlybxc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fnuvdltr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ikcemoqr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2hizuadyv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wicuzrnc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2jqscpjuz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qsirjvtu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nwianejs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2sjzumymp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2irurjugd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bwkdzays.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2adsdulix.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2rbbmudjo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2csqylkje.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2upvkjvap.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jprtdnlv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xsksfilf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hrdonsxi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dqkqiwjt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xewxnlxa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gkgffvpo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2mhbjsbbu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2fvhjtcyu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2brllnqlc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2futlingm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2handezzi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jvtpxpxu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fajtznof.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gxdyeacf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qynrymer.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jgqcxzfs.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mvphnpsh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2bcfhnolp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xihywpsi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vfstopqv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ifvchuvc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bqrkvpyi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lgnuxgvu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yfjbmswi.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2cgzwkjte.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ayqnwdhk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2mnftstim.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2imbknloq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ctspxsvb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nfxutvkd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vpxwbcck.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2torwmona.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tymptyeo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yrieicjw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2nfpfmeec.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ynakmwij.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2drdgrchb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zqwrfrdt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ttycficg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pnuynrti.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2emumrtkb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kypuapjp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xqqfeizy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2smqtlcmo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qiljfxnw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kntgkniy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2bvrhcrrl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gszatloj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxrieqkb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldyeeplb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtlrzvsa.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2hwnxlvnv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxfgdaln.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vhscdazh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2tfonfqxg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kzfcxfut.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ftqvlbeg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gqnslisy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xopwhhes.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bzfehfzz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lhsmowph.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2egaqzazn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2rkpirxse.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mbjcccrk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ipikmptz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ewomohvm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2etthljix.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qerpnriw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2rzepnwdh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pakvtfpv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gucopvic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfuqrbow.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2snbseeml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2doalywxc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xzflumgm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2fbdsjzbu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2svhroxjy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2elzmmwzj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wxnuxavr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mjbsympb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vgbuzzew.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tnzrrjad.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gxlgkbys.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2upcbjgol.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2lqmbvmvk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2trapgtnf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owkswxmz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qiisxbje.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pzaerrgq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2pgjfigky.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2rfgxbtwc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrjawncs.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2omyucvkw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xpkqvadz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vqnckmdu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zxkyuxlu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wnmfvllu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ikwzlkvg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2hizeezkf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ylelsomr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ephppnyj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zjacjcda.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2psgwwzzc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dfdldyvu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ahqbogbt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2orkrygtr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2djghxgeu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xitivmsx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wxujfyvf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2blvqqwqo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2chlyipez.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wdhtrkyp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xqmxcsjx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2spebvrlg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2szjdytdw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hkfhowke.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2atysjfoe.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmqqfyay.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uolsrjrv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2bpwrgtqr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppwzazcq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pmnhlwop.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qgkbdhjq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ftnfwxtq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ictgquai.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pdrcqixk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wmkilklg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wonwjfup.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mbhvjnbn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2znpxirkm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2gtlbslgf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fcqmtziy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2svvmkhdw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2crsdiegl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ydrweeqa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rimislqs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ayfuhkwo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ohmijymr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qorycsfw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2iqektwyf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fypzuijf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ngukltzk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2oqfnhkhm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ezowuabz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pqoyuksm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mrlfpgfo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2zadlffjs.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2itvzsoef.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2swrxkgfz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hrhfkydv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mbaebnkq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mmtkuxdr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2btyhwahp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxosjwby.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2kiaqabip.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2vqnbgbgv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hjntekra.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2djjmroxp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jflsyjzn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iokltusg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2zokosftf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xlbygroj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oxpftagt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vjudrszy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2tkaqseul.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rtaybfxa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2twwtgynw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwduhbur.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asbjohsg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oumqzfcf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vjqwxjxa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oiouqlam.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2uiflpama.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2jjwyyzfk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2qhelszeg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ckwcffjw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2njncjyfv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2bavsfdzc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2waritmrc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2qxifpxfn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ajvgcovx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2gbcnyoqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mlxibajz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hxpzfffw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgjfigiu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ecelrgib.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2cawcoavs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejaxjmfv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2webquxjy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqprluxh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2osnmnxlv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2aftiisew.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2sikaadpf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dukjldpc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2hvrzuqmp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wivgywwa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2nduotltj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ugxbhxui.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hndhcnor.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2owtiwzzc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2rffcgrgs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2evmsvdyj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yrajkuhg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2cnfoziwh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ymavktha.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2paqwixyt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2orluagec.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hvkqhcfd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2awigebmo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xgxpculo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ukxizpqc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gvxcberd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2mfwsjnhd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yrxptxoc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zraqjdjh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yrdkcsyk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlvzmqln.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sxdicvql.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wkqnjbpy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2liljyepu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hfrvxvdv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jhqacucu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2szgenxwz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qcwuruzj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ogrkronp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bkyravfj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqzblteq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2iykoaywj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2febpslwh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vaofuyot.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2txdiazvy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2voaasrxv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gekidzmb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwkcpebh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2celdzhgn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddsdstcx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ghzytagd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2phextuum.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2gfllmuzn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rtauxwwt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2hpkyviyh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fkufgbos.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nwatjqlg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lnewsshi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jtnqafgn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gacmdvcl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2voevzsmk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2iwntrgdn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2drjctfgd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xnklzjse.html


<!-- 参考信息 -->