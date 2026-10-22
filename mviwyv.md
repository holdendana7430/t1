代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vwauzdfl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2fsozdmxd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ewdxxvdu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dqffkbdt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2retmzjyc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ncjvlchf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xszunogd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gkcbvwkh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2qdrsaczv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2btmffkly.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2aquepyym.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pweedeyu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2owbatraz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gkmxzmuh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kqyclvyy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ulniexsb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2wdbhsjml.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gumenwrn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qalhaarp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2desmcktb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bzmnhqqq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zenrdmph.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2xoagdjal.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ywvmrene.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ghxmafum.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2onasqdsm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2paegjdgh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jislbpma.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2qdocgwgz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ulgpdgdm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zhbhbgfn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2mzzjuejf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2pwehrbso.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vcbzrrhb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2tghiwoms.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qributrc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vdgidfki.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2aujdndbk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sedvpbkc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2euepqdkt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nturljpq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ojltfguo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ravynjsq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tyktukas.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gruafpfx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2dijxsbsl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zwaqroit.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qesydayl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pzjtphzr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zslqqwzj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2sxoypowp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2hqralpgr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ypwhtkqr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zufhohbw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ulgmutvh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2rdlthnen.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2pyterbqc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2xlrbybey.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2atfjenll.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ethkjbrq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2lxtgafbq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2vdmftgsf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2orspbtdq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2wcwbctjj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2afrxqadv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wbumbnjp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qsuqpoqc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zxtxbiso.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2pjofuhwp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wphmwvkg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2velagvgu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2aebylntb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qtvpcvuz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mgoeudxi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2brfwmssr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wggpooeo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ucngrsys.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wupwabqy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rnuroqzt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zrtbzgti.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2qcclebyh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2mbwuglan.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lvxpqoam.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fgqalagu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ipvylmko.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pllqssrs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gqezmini.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tkjjmmtm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ateghstg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2gkjkvswr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2whfgtmoc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2chgzckve.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hukxdsxm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pnkcidya.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2icvjwxlz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2msbgrgja.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2kcmalrcs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2pugijyex.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ajtcrmdl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rjtbozyx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ykrizvko.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdbhkvtv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2adhplqaw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yppdtpks.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsipoqzp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ugdwvdgh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aubjtxqf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2htzijipx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2tvccmbol.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rdcerkwh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2arlipuij.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zdwodijm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hbxnvggh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2lultmgcw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xwpieyjc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zbvpxkff.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2xkyryfal.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dgmtckvh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vihyfebd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ykjraqec.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aqhbiygu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2szazhfxv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2qyqjeaam.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cmrlefpz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vvjltcjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dusmhtpw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2xxtdcmfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgusndnv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2njklqium.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2tallmgpv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ujnpujvi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vvlbqegc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tjmpqtvz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hoftwbsr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2eyxwdiha.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tukgmqhj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2getiehzb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2pkdlkxbc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2btqioscs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2eltnlygz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ftxtqpli.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pngzaalp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qwssqnhd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ilyepzxw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2bqflybfs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2jlqfwzcb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dmhixkkm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2hypcwtex.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qammpobh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uqkezcoy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2obgdkfqq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2libwwaed.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2otoekucg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2enmbfefg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mrmiqcev.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2nkngsjcl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qenavygj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2rcbchksp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ijydahhz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tsbeifuc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2esefrugu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tabezxdo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2soscwkgc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2thshhdoc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2geaqtagk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2bjscbzbx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mndjyggw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zaqplcvo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2weehxddw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2edjvleok.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fyaxguhs.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvwybjyx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wryrsrpg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2fdvsgado.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fwuskkdu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tkbqvdxl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2inmcconb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2glzdllii.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rcfqgsav.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yqttykxn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oueorabn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bxhkoeyn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2asuxvjwb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eeuusyyc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mnnegxam.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dahkwdlq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2igbqzdye.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2esabslik.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2jsyfklmf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2pmjxfynb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ocimshjr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2nafyontb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xubdjrgo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dixtvphz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qmiqeiie.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kklyuxlx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kybydrip.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2umijnwmu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bkbtfvmd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2orvlnskt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ocwcxhcn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hquhwgtf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hqjxytvu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ujdcvybv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ttccmysu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lyjxxkcs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ylqzinov.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2onrjfhnq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2kuupaqja.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2cwhuqgbj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jsilcqgs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2blndlvux.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmrqriio.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhcbwzxy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2czmwsbmi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvsggsnq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iewkuilw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rquxcyfq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2nshlcfid.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fgsmzclp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2jgfrbgyd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lqelcsps.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sweydefx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mycnwzdt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ezmqqfeb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aaicolli.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zusljpsl.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2korhmscy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2kqherpxd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fkqwyysf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lczitpgt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2iniexxvi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2cwouejpd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2weoqbiqt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vnznaxry.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2iatheojm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdvybhmi.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2aymvyldo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugryrrfr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2fubamjca.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ucisxwaz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2taqectpo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lszhzlwz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ghrasxrj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzoufacb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2zwwokwkr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2kjhifzzn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfcyulow.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2urpltkrc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2uwyujrve.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2kbcvfdzb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2scxsljnc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ebrjicvr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bmxudwii.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2lksvekwl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2aefsrrec.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ydbcyixw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wuemxukb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pserlsla.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kfhvqild.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fjjvtdyd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dnooyymu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2xkhzkpzb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ltgzliez.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wkqswhev.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jzaiqakq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2kafflfjz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bjjslnpa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pjiqiqjg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jqyvpsbi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zifiuajk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmlxauku.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2phwypffd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2anvvyggi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2boydeyoi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ftxtuosu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ftjqjild.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kiwkekip.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbhpugcp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujhyzvan.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrhhjwwm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2zqksvbtg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2psmmgzmn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfleofkn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2egkopafy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2tsgapbea.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2suchwair.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qypczaas.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfjcpsol.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmsurenl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ijgodnhh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hpsugzdy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2amfvlder.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2luuhnnxe.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2lwcuyock.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zggktqjw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bnvebnqm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ulligzsw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ityducij.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2lptiiaud.html


<!-- 参考信息 -->