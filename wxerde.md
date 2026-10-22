代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wfzbmcyb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2uuhxmiit.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2auleitnp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xequildh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tcynlxls.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2wilirdje.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nlxewrxf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zjgsobol.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2isidkwuk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rjotlyqm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2lzyqvdzo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dgmjetrt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2shttnksm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dfxylnnr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2utrqzdfo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bpjkufzx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2tomiqtvh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2mroclxnb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2eoiignzl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xezrcveu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2afsczrps.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gxklryni.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2aplpjfal.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mvmsqsnp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tvbsmday.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ivikmbnc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qzlvfejm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2sltfzssq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2juzozuhr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dxdxtmno.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xovaxhto.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xynkpipi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2mvyqpxcl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hdmgmrue.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2cibtvewv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2bdlfmtct.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2aygjvclt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2mnyphrhi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2aybskklw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihixzoln.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ghorzntr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rwxzfdae.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2myebydmw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qpkjiqhb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2cslonpwp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2vmcwdxzy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qyqdsymw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2uanlytzp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vqwhdxdv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2plkhzjan.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2mjktollr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2fmahmkjx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ccckggvd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2acrnebng.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2osloemxo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vdvpxdsu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wcbdzban.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2cxrgxcmb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dbtuwsgi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2poowengu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjiwfkqh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2nsmfxcef.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2acnirwgq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gxgugjav.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ooeqrfpe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xleufhqf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zfakqifo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rldugfxb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2jaewbobt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2dzwjapgp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2vwnlxjbs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2uyemrxst.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2gxpdcisd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2juwkelwn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ixgrsuos.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2prqpxadw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vllqkret.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2esmrrvkj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ghszptil.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2rsrmfzzd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2jddyoctu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ehwpfruq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2oclgxpqk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vxudrrvd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jfdqrhqs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qqypdbaz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jdgqkjzr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2xoybqekv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vlcpjucf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nmbvdaht.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2pwjirlih.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qhzmifcg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wvubkmqf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2iazyrejn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cabykdnk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2hqmaneou.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vtxoudzv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dlihvfzl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jfuuhiry.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2hxhrbntz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2znivnnas.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcjlxedn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ubzkpybm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqhsoxsj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcwnzsys.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2hsnuwkds.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzudbvwv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2glstxhsr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2itsujvfp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ynmkfmca.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lcbhzyye.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jbatbkyv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nfemlgyc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2krwqahjr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zunelpxm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fbqbihsj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hehsdavr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ogiilnqg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aitipknx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wpavbntj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ynbzkatr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fvocmopm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2xlpdemeo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jkkmfbfk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rmyaxwnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djbagaoh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2csepzcwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tipbwmcd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2chcayivt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2cjrtzpnr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tcpiqmyq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2crebtjto.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zjpujrwx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ysloviqw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2mlswbnzx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wggkeddq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cmjlkiku.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhrjeuys.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jfsoymoj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxizfuoi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzjyyinl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvxggjkp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2izgjkzti.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2tpgtavel.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2lhdcrytc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykwlcitu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2uewqfjnq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uhldjhws.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fqjbimcu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wmhvllxm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2omitmcku.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xaprdfoi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2sgzgjqyq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2fmhyoirf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bsbbiore.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2anbrorro.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eglurjic.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2txbbecup.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pjvghamn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qkydpfoz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2yecjlhcc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kcskadhn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xayepwts.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2eldyiljv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ynwmkslr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xhbakubo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oxtgjfrv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wabgudfm.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgaysvfs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sszoewly.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ucmmvofy.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2inngwxqg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnqqahhi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2usduztcd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2urqkcsxm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ynmfpcpc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tirjchbb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2islbaeam.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hpypegvv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gldtnnpn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fuhrqqsg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2phisvfsp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jijowdvt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gdmiveas.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2aesbdcue.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wxdysupy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vcqvwtdq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2obyyunyu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fgkikwba.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ikdvolgw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2dhceotkz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2aexigixv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2okqsavnk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxfdnlrv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gzcwwpzl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vmnwcutc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bdcbonup.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bcgufvek.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jcwcvbys.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rqotypim.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2lwuejklb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qrwhtzin.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2voqsawvt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2linpersl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2uwvriakh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2agvalyum.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2woqnltip.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yhsxjwsd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zjgawvoz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2atkunyht.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fzmcnvaa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2btxoavyr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ixvdlref.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbjrytgg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2llynmzwh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nnuoppui.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xzfllqfu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zapvlsww.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ktawhxxb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lnhuzfnk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ivxuvvrg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pljzygyf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2motcdcub.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ldhksbgd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hitovhvn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2njmmlnjf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2vwmgvcbb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ivpgtnue.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2dzbldcfs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zijvtyjo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2udndqwdl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yhivqdaz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2smakzvzs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2fczecbll.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ixadxpgz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xihxiaia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euznsuyl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2mfaitigc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zrxlknpw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qziptcik.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2oaecsyxi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yixryybn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tefvqhaf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2kahdzxil.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2shsetqub.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ksmvwemk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2cvnajhqp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lxlrsflo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2qmkwmmaz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wgouohgw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwpgwkde.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebseojbs.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ictoqjgc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gtldhllt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2qqklrlfo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2fftboudb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tvaqusid.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2awwxjjsv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2uoqbkweq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ykfqards.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2llhwqydk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qibnlpyp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2spyigriu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hlfdwrji.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ikqalipn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2jszuqhuj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ztdykevb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nqbiiwun.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofvolwqz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yybymcyy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pfafgxmd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pkzqdguv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wofncuez.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wccxnybf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gqqrmoca.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2shcxthxt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2auepbcgb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrkhoxjh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rubbouqq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qycxpock.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmmwvtiu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2gfehbzus.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2amlcuekr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ponnfelc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qjithrsl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vkrdqhyu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2osuzwvoy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gznmwgns.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2spvszows.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2igomtflu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2dpgjzqng.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hwmkyyky.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2fviqklyc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qnjlxpok.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2vicmoytg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2inmnprjv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2analhjsn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cphxkuvh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sodunozd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2qkrtnulb.html


<!-- 参考信息 -->