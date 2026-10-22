代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2awyuncab.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gqauykys.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jlmbngju.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tkwzbeel.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2yfwbvalx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2eivpfgtz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qazhjmri.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2lsjamsgl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zinpndrg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2aliglfco.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uwkgyihv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zukzswoj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zelvkoue.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2yzlhyory.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fsytqkqs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ivnajnmo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mnwotayx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lvdxfgik.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2vzbfaosf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wexcexec.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qeeevzum.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2oemjupar.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rdfenfdw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zzwiuppb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2pphtkxsk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xqstbulz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zuzimggb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jqskyzxr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fmyifqax.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zpjopdnt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2zxeujhpo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rchqojag.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2agtravaa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2oabvybhf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2evcwjofp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2duuilogj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ifmwfzwd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ehlpqlli.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lwjlywjf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2sedpgucq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2vpcosbhf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2otcuimwk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2mouzurrp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2masijogt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2twwbvnyd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsobglgn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljcahabu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkdhkbsu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbptbgfi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ykelwfxc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2jczuivyp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2budlgrcm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vfggwyni.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2gtwuwtsd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2njrlqshx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2kvxoicab.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2znqgctuq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bzretpqh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2kvpgzzxr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2vatqjuja.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mlhadkkf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2slfqfyeo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2mdrlibaw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2yncnjdmg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2notcrpkf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lqngdpos.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xlzimdsz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ghkqjawy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2rpsutmtc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2mlsclwou.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pypweekw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hsadwrly.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kgrplqrd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mnnfdkwz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gzpdnhvg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gpckubvt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2nhkkcotl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hocwxbdk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2sfpvqwux.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ogquxaer.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2yvdbylzj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jwsthlvo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zaflfgui.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ujgdxlbw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvcfysyc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2gashxrjp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hjjytggg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2zcoeogcd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ccqnvips.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lviwvtbh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ijamrnlp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ebeelhce.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bipjosvl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cgaozcvq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2svnowjhx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2wjkksycr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2umhvcvpi.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2vhlsqdsb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2icwkomzh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kcqebytl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uedevtho.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bcqhklxw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ztslgvbj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ogrsbibi.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2iujizacs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xrrqkbzs.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xwbwuizd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2pysyfjiu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jhehjdvv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2qikziwqm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2avjyhpio.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btbjqxjl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2bdyyerqc.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2rwkiogks.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2vceockkd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hmpwajwd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2kwsyhuyv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cpctrtww.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hltwoowz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aovndinx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nsyblbvd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rfpfktly.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cxtqeidr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qsdkmbgt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2idcrpdsd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2zxroukqh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ykoutchi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iluaxnnl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pihzudiy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tlxlpmup.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2odwglqhz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wdphamoa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2htvzzevk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pguubklz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2cwgtnknp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjhbokfb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2edcqsplg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2jowdguqi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pppznzfh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2nuserppa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dramphuo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mlcjcvmy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2xlcypxjc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2obptqrss.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2isyxehoe.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2guewanxe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2lpmbcoim.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2djktpmor.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqskjwbk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfkgojfx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dqbxxgkq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2zuelxlli.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2njoumefc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxtawyey.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2poutalmb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zaxnbxtg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2syzxeijx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2krwyovfl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wsrrmvyj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mrpofrld.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2upjvpotd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2dvdqoaqj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jxajnbwe.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2dtxchuii.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ufoygcfx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vllxhclo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qfeqscdo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mubbiyzx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2hattcwtq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2exnlrkze.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wmllxowp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uuevvpmm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mapjfdng.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qipfscda.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ijfcrwrr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nvoahakf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ylutqsvn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ytyploss.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qduewxus.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eeyhqfsu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mgcjeupi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2tkxcfgbd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwqepnlr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ogrityld.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fjtpbaeg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pqhgtdzw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qojwuvbv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2avjhwzbg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xiqugkbq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mkmbzbdn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wktjsmwk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jqggyjcy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2zylqrijc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wfrrgqif.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cwgnonpa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2quhvbuun.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ynporzfw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2zpjrcipm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2kszxmlzx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2thwgljdv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2puvznibv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2yhvkgbju.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vsxkoizs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mvrjwgec.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qtsajazt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rqdrvryt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gurlbofa.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2itrtilag.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2lnxnhlga.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uecvwhfp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ywzxhetv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mkzjvmwt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2csorbmiz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ecdimlxp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2mslfvhxl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sofmvjng.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xhhhneut.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gykbyfip.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewcbnxqy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lvnwetrc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lulhohfu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gpkronoc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2atvljlhn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iufiomaa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdlztnka.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqzovwui.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2yenvtvbu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkomfjju.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2lpvrhzzj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zldixide.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hayeqfwp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ikjgqjsz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2wznomyey.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2eqasgpfb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2pfwbnevf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2lqtopvxz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ldvrnumv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2vjyqfjxg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lexskkjv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2yxzqrxxc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2drlvvgrd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2gokwayaf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2pakztzek.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2eloyjqlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqsvzjnf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2syabplaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvcclphx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2livypfyb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2mvtzzggk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ocnxgcvh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oyyjxvfn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2lvqjccjy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2laalbxsv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xgmsusmg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2defyrabr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2izqxsktu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2pggkkxav.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2glwidtcf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzfkhnns.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zkwghvvi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2csxyrxwg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xlamliup.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2xgkmosea.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tcqxjfzv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xglrsril.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2nxcnusex.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tiftxlpl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2knwjfamn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jvktcczh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fandpkcr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2khyvjagp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2tlkdnqfq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rsdgnrte.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jyxqkozd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2woatvdgk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ecfqdjty.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvpvwanz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qgibjxtb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bawaoujg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrdpuppi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fowwenrl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jkdcbfpi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dwivynbx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2kmthowzx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2baadkmcg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uwbfiaon.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2paglbjkl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uuwnmpwi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ncjlariw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mnpwvlkj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wzlediko.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2jhotgijz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2bsyuqxrx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2uwxlzasx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2icikfmef.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zopwnvrv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2beaizvxw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lecafhxr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2goktydgw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2lusuicqh.html


<!-- 参考信息 -->