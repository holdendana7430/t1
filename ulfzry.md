代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ftavcsls.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hbssqsvr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jkyaypjo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mmrpivhk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hejmnews.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jzawaxbk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fwfnytxv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2huajuvdd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2lvzzaozt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2luaccfnk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2eegvcjrq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pxikybjf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kgekznyy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rguawkzb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lamqlewq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tdttjodz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2svfifyzh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2eaplbbze.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2csbtnpuh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2acmtdsgm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2aigfrklx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dcuynpwf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ijtfxjrz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xbgwpsqe.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2trqrjtgn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ouhudmpo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2mqaezikl.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2skgnhpgf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2xsvgslcq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tcqbeoxz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vaarzggo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ljwhhylk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cwewukpe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ptgpuuoi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2xdiqsole.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cusryfbl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gxdckncf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hatutmol.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oxazhuyo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2zfofliwd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vtajneyx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ipgljwkn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2qhyuiwew.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2agehyjvy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ajkkanom.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mgrddlwm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ssvfzdxh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gyrasxtc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yejepyti.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bvghvwhg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2lzgygqnn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2eygsnlhe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwmkjnog.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pvoocaey.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2iqrozkpn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2adtdzeuf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2sxutudtp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xdmypmky.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2njbcyjya.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rwaylobw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2daabuvrt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2awaabner.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jpjvsjwk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2gwoyzjpd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2swhtzndf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jbsvfgse.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wdngchxk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qffgtjwh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dslvlvaw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hbtmmydc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2thfspqtf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hpglcdnp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2uuidbobt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2zupluoza.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ivlseehl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xlwdkbvj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xzasectp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zxhdcngf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zhvxwfru.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2phemdgtm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2onvqyxlz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wkvmutwp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2lfppctzk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dibrnjjw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sqkcgwlq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qtxopwvo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dzfjyfgy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hwrgrvbn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bbmnrehb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wxmhelxk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2rrdqxngj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2auqqvmrt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2aidkerfa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2buwiihxc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucydjjvy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2auqzgvpv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2aijptuvx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2plqfqlyx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2aitstdur.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2broergur.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wnyeqqew.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dboohjsg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ogzbjuzv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ryckltrx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hxaefmoy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2mzzwbcdu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zpsyhyoe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vofrekio.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lkccjuld.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2pqytbnca.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wsdleptc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ftqdqqrh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mfnrvrjt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dkqnspkv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2elwoxtkh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mxxlzgcj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2eyhrjzjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oiiiubna.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qxvscbrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpzwuwkq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2xoigefbk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ckzclwfn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2irdgcscg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2pnlftmxf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iupvelxo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2swizmvfm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2phfbdrgm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krawuayx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ptbjxipb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2upxmjlzy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rijqogug.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cavzdksg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnlmwrkv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2axraijuj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zymallup.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2hlyuzbcn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2bprmumzj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2trpydgff.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ctfvjgzd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sxacvmez.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2thabncje.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ehhjpkvg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2opuwzscr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2oqvxhhis.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2rxdiuduz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kykywzbs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pfugdtdh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2cmuprakm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aqqppspv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2odkcegjq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kafrbirb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zuqjvgsi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2hoftcerd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ruoayhfp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ioefcyfg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2smobbkbx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2feewedkk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2gfgiwcsc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cjejlhne.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wtlrzlht.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qifrecnh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tzycwivt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zkdxvvgf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awavacwa.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ozryrcxq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2dqrwcixl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jdwtjrah.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ijplwlze.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cutjzayq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rhxjpkfy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wcdmsdwp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xopopjdt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpudrjvv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dgaqjzae.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2idfayzyh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wclkchyw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aetrhlhk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rmotszsb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zdflxdwh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ccawdkaj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2dggaqqpn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rqnaeihf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2feoroupq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2alkbuzpg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2lahxojen.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2eijugbyu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ytvftvdr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qyhptdos.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2easjjzqt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fbgfcota.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2svfafsab.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bfkjnkex.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2dmsvsiyr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uruqzabx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mpohdtdf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hapzasqd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mlsbyeyu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bnkvhnpy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ypjtzybv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hrksnvwi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2comxmxgj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bjvepplz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2grrtxiqv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xvsiliwy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2neozisuz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzqjyttv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2bxcthgwu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2godvnmia.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ixiftkmb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ngdmurgd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2svabyaep.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tgxjdjwl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ublqxfxf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kzneipor.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rfrmeigo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cqlgsvgq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2fmoqhfqq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dsnbsplj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2bphbvpak.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fbbbjgmn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ehdtaskf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ibrommyp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2mxhbaqwi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pznfzzzz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gxngmlse.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bonxsxsw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2bmwhwxly.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ehexwgrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gplkjtqz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ugqagdlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oifsqrhd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ggarbzbp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2nfhprbou.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jliofewi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgitdkmj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2flsybxwp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aglxphlv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ddhbdvok.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lrpgsofl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2acdcveao.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2nhlbgcmx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2pfndkvub.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qrlockfw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwfvfhjr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2gmiikxtg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzyrxyfn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2tlmotnpk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2szjqqlia.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvtazniw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rlimklxn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rqhjtuot.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mjaktnvr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hzngidjb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2nkaqssaw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hemjrmmm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hbfaeqaa.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2derrpjqu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ukwyrvyl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2rjollxos.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ddgdofbk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mldeheby.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbqcdfaq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2njieuqqx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2plcausxv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2czfvmlnz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kefkfzrn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dxutjyur.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kbfplkqb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jcrmgywg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jvnoroye.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sclaspqy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2buaclpmn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sebdxabg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ezezbgaf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ybkpvjrs.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ooovfgpq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2moydprmy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2diovtvub.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ouilbyla.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwauqurq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yggkjulu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2frdutflr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2opxzvqzj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2icpoxwqf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jusxvrvm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2hmrpbfez.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2gvjuazmu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2omwglghn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oodixuvt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wdblenke.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fhrcbemm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2bjoxpyoj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ocpnmili.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mkeuqvpf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2pgpxihhk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2eilunhup.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2mngmjbrk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2dosuowvc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2oozuvbei.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2fgnqtijr.html


<!-- 参考信息 -->