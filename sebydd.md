代发 wailian999

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hoxmixdi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2stbupnig.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2njbrwvjz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2imhawbao.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2spmrbstn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bsmvnnpi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zoanzinh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ptvfuwox.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uswnjxvc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sfjmgpij.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2zugkmsau.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vknkezfb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jkskukvv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2mvjdqtbr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2slnzlbos.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ppetxrbu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2dfxtmxml.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2tkeomrlc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2nzfiikpw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2bkypuqts.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2krbyfkcm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rhophlph.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qilbgbny.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rjnvinbm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2tvkzrrze.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nrcgvwuv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zblohpnu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2znbdqdyo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2uacklmom.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2barzvgfx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xsrugpri.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wxlqqfwz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hxptybuo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ttsgpuba.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2axukezjp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cjmjdsli.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2fdwokboa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xablozgb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2dpxtklrg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cqtstyam.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lbwsbbwt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ijeexfxa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qvawykaf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qarurrvd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vxqgfvfl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qfsngqlt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zfxkqgal.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hhoaaiwa.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pdnyrojh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ayzuukce.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tcanxvsh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tgyvconl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2raqgytnh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2yrlrdwbu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ckeoeafp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2spqvuntf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2sefgurki.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cwqdrjcd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mgwjnams.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2tvqjkvxb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2pmvompvp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ximbvaio.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2olyylmdc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ebzniktl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2qufidast.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2jttehiqq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jvmfgupx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ujkovrnw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlgfpbri.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ibmmacrn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2jxnooedo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xstbjdsj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2bjsdycec.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2uqmtgggd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jqmsxere.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2wswbdtpp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2qjsxjylh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2woonoxeq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2zezttbns.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2sinautuo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lnganwrj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2nfnitzhu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xlidtkzu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2awlsaczb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2jazkwffc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kwdoyjpz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2hsctcztc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zwtnwreq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qassyvuy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2kcdqkppn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hkffgzkx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2dasgwhxt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2cpszvntk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tahammkh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2anspnkrk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cdzfvvsr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2xdtrcpbr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2iapnhkuq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2iqlrtsqr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2dmjsgggl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qolfddpi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2qqqeqsew.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vssjmdsq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cshseljm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ycvwiztb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2wxzdafev.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2iqfksxfx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2qcefernf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2rtkzakcw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lkudygvy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2idjzdsix.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lgdatgfk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dabmigkr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ohkztupm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2imscfebg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wahrkslr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hcbvvhcq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wtyjyqpm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2yerjpkoz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cowzatzk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wlrnyniv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2srnbzgax.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2atzwuwta.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pjfwjbyb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2sdjjungg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ktmrebhh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2hftpnuec.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rpcesblb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2gchwdjei.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2uetnteor.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wribahrb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vbuhivel.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqxakdyo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2vjjyzdae.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2wwuajora.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2hqvahekf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ngrrzvmd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mdfrozel.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wjxzecmg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dxdibfcr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lemvvlob.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2urqsjiug.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2axtqexaa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zccbptrn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2xvgnfvum.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hzmlnqto.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wyrvsgas.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gagapoxy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bpiiiddt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lspkhfrf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2istmxpha.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pvhcmaoy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2apboctoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmibnedx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2utwrutdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjwjsqys.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ymovxotf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2htyebssk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cgzazbds.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qzfmtunf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2itjzqexm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ycjoarng.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2eknyrwdo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wzvuruiu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hbhiejef.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2kkbalmhm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2lcgjgttm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebqohfnx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zrmleotx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttlfsstv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qbcwtqas.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qlfmytqs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ogcvktyy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2gdurypwf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ogzbcmqm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jckcpnpw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vhfjkvhc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iazayczc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bpyzzrmm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2uzuvjxzx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2bykhqkfm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2aofzsczh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kqcpopdc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2vtkrlwgt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2scpjnayu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ofhebdsv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vdgdeyfv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2iqqfhhne.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2eldfeoeq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ekxusgpp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lqyznndr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nuxahncc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2owcljbmw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2uphmiitr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fodgultj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rpeiuidt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vfckcwoy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fnbxgplr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fwpnhitx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fpafqfib.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pemgbiab.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2iqzfcpen.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqgrdakk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zfydkkiv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2whfczjde.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2penwrtut.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gfgzisnr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gpippktx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2otuzhtvb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fnchgdnr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2drxdfqjv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dmcltmuy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2orsnxrdp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2edibvxpx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pjugcitq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2iznioryu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2yugwjhzz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ttyepphb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ugvymezp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zvrthqwz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dwhbottb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2rulcxfrn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wivdwqxu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cbqatoxu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2numryhsj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hsepcvyx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mzytmfcl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2hkhwzutd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ognidpqa.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2txshisfd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hamxchpz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yvlhbnbf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jaytpxio.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vahiszyj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ktilmnyx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mrniqaji.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2xfubkqgo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2cfpvlhmm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2svfjhwrm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2elyaulpf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lkmijprh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oyfiuwls.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2obxinvrg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pltosyct.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2glwladxj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eknjkihq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vyfjyjja.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2okismrma.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2evedoeed.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vznxabey.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ufmpaljd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tzhtukyb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2tpyjnhjk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2godxfqen.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2pnebgnfx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2mowaobgs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vvfvwbde.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2nkgrgbot.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2jabplroh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pmqbczcq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2lqvsjzve.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2tnkydzmx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2eqeidlzk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2utpyzjoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omivvter.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2kyavhgnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwumbcvy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2rziijzlq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2okauhkwy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2juojdiij.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2icsqutwq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyezybnz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2tbqcseil.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2avupwpea.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2xtetrgtu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucafpgiv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gpzyevhk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2iivpuoiy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qmioniuq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnoikzba.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2glwgifls.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pqrzvbia.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2diltmszu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zcagivst.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zywuybey.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ythfywoz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2khrmjdul.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mbqptbuv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2limihsnh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2nkzqyqzr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lxfyvndh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2knpzujrz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ncpuujly.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2fnqfeqql.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2pobcigri.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2djenhleg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qfvimrde.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkxiqghl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnrvxhbg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qstwruyt.html


<!-- 参考信息 -->