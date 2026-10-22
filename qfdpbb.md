代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ffoyxrxf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2nqaszhkg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ykcafsbg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ufcroolm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bwasextg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ciiyosho.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2fvazzspw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xejecobk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2kpffjznv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sxnblpgy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2xjpiyutj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yiwrgnzn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fcykofja.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nbzpnkup.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qooctkio.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jyaxzlxm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2shmrdupk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2emrezawo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2eympbpdj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ydcoroky.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uworqfky.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lvpbzrli.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qcgcfpua.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2poghknah.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ozbfwqwq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ftjeucpb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hxmgxyyn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pgshibbj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2huxgyldt.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2riosiuik.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cnuemcvh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xbwncpbq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2evsivuqe.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vtjgwfws.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2dmnhpbem.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mmsovxso.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2gilqgljt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2dfhcvlux.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dipkmdog.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bvidpudg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdufithv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2othaajdb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qqdiipae.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqpawvlx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2zrdkpyip.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2lbnkvtks.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tyyatahb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ujvftnhx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2arloiyho.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jthbzikk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2dqpcwdmo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2vlerzlor.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dbdgbsma.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2oabahoyz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kcwscwbv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vomuekzn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yowwhiaz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nprmjfrc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2bhqjslsm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2towygbfk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tqpxbudv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hqguwicn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fsmstsef.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2myprqzwb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2gcybbwdi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2scqqgshn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tskisdbd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zxemlccc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xhydgelb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2yomziexo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ojrnzadf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2dbikfaob.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ivbxmiou.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lkkuxdre.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqucgujp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aeqqfmdv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2mdljywmq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jpevzucr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2udnnasky.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ttidhdcd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2kypzhpfm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2kuiswtus.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2zrtarsjq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yqimolhc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lyfocsyt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pnenwfgy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ssnrqzga.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2iipnqegj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ruhhobpr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yrgednbi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jswqnlaz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wedharkc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fojsztwj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2geoqdsff.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dijwlgcm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hdgfnnoo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qnqtbwjh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2wpaudpoo.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2rguukwiv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2voccqzyz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2kciftfyl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnhwsvhj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcqdecdq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxzvxiin.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2fdeshfhf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zrjgxzvr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wazotswd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2dxumcdqn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2kgyuqnps.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ttfymife.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hopxlzdq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rduxfeqf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qchoxmek.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2jsslgsha.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kzbluwth.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hsbtwygg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2gecdhcbg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tycbrsvh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ahadgjsh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2emazbine.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2giipbdja.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ptthoohn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2bryyqunl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rjcgyuhe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2epdheyvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skexrtin.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ejnsovit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfmbvhlr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ujlldony.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2zghouksk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xakynykp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2schbhiok.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2injgmjgg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mynszbda.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2dzdrmdaw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2abqxmohb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yunegiwf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrdqvxdw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2vqchynwl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2msowoxzu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rlqavqxc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2diprbpbw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rqcflfun.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gzqynqgm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2uqqwuxgd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2glfbzbqn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2phizvojc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ncddmwqy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2djwzuqoo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2effpixuf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2onqbdwle.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mkgzmiia.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2wvbkpqua.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qxtartec.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jcrnihqb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2wjeroold.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2swxshgjl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2cbekgqrj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2khdoqahs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lqrqtypo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2frpblpqr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dvmqzmlq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lcenmscu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2sfnlhwbn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mkskafhy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jazqtfsv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rijdbpkf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fxberzuv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ydjmaoil.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mmtnqknc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qmiotpju.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mzacgpau.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ygxbgujn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gztzpmek.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2izpgzoko.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ebocqcyb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2otrguboo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2msnnlhtf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hldvhvtp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bdpcsonk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yvobgizv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tqqvvzyr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2aoggrckv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vnulnekb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rkdcgmia.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nlvxnysn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2igpmeiim.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2cqtwdnoj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2vsmotbxy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2tldtzlaf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2fqngwmug.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2qfahunph.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hscejgth.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ahjfxxal.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hpstozqk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2luaozzjp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sfjfjsbb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lfbalqib.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2acvbesiv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xakxnosw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ttgutjow.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2klojwvib.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wsjezdob.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2snkdpvpi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ncegjfzg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ykzaaswn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zgdftljp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbetfawh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2szesqmdd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2swgkkwvf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzgjduit.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mytgunqc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmuvgdll.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pbwqnkyb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2agtdmoqf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skjbzkyn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fwuvqpfn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kgfgdbpv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2xqhsjixk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhfimsce.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tmrobsuh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pdpekabh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hrokwzoj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2prsdhlvp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2baptvldp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ppwganqv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2lerkcqda.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2qjksewum.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2kgwocbya.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2afbawtfh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hadqmvpp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nupernlw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2qbylwate.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2yafbsmxj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2szizvvfx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2dwbsfaoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xufeiepy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2wdjunrpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sankloxf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2mxtornsy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ymcpgtnk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2jjaqsmlc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cofkxyhk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvpkyebw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ylgentui.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ahfpxspa.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gzfuuvxo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ecflcvnx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2srkjjiig.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qrmywkvf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2msaiyssb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wwddxycd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2dlyveyjn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiifprrf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2gchcymtn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qitnhmzb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpbtcoqg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2otumkfrp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2klmvvjsp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jctoglpq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rbwgwnln.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2sivzpehf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2uceghmlf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2scknojze.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kheicxor.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rwlpktxc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2oejthuzz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hbzkdqmf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2libuvexp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2huppftzk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ixycsjbw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2acwjyeue.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ubsodvoi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ozzqigle.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pdsiefwt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2oqiprvyt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gsybbjgw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ayztkhik.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tcbvqyvk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvgjbmkc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbwolmkj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2gqsurjrb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ptonstkz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2aobqnhuh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xwzsvtyl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2nonzrzpf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2awmzbrlj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2baszsuys.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vwmwfsbs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrgomliq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2frhbjyvw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zhmocyef.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2lyezwlxm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2phgdfxuh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2wspvgwcw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2azxlskmy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bdamtzxf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2chauqfvn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bdebgfhe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2zrjfxhdu.html


<!-- 参考信息 -->