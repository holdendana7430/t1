代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fmchmbaq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gszdidfl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ewiwngbm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mqgmigvm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3bqwzdztg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3kaqkrsqg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3zyckrqfs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3dfdfaufo.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3gmdrrief.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yfacwuhn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rwlbxtnq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3axnxyxkw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dyjcgbxc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jswzxrqm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zdhpmdsu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3wxqtytia.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3oububypm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3unducwec.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3tfljdfig.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vmrnivut.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3whxpvvlz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3kcahodgu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ozxhtemj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pvejzhyt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nqtaronb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kotjuffi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jqaumbgm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3prbptcgt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3afromlyr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mvqrjbeu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fhyrruxq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ryjnmuuh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3gyfqpeuu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mjbakusg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mctzpbhe.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qxwwbnxz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fdebvozi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zpjhzxbx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mohfcaiz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vduqzvos.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3saxdfxeh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fokzuneo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3wgwetspd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rirxcoxs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3yottyznw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ciarlcve.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ydfxncuw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3nqvkuqmt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qqrnrhvm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hbtawlps.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3dkpvspnz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3jdejpcqw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3zmozhwth.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3dwnjuiae.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndvlnmoi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fbpflnxl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyagwacx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vmnmqpdu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3apfxnmnt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmsukddy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ibqasuuy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3zmwlccmb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3beaqjtjw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3reiwjfpf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ltbiebgi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3szwthumz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3zspqvlgw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3doxtnssh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lliqamno.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3mouhkala.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xzttrrbb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tabpqszv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3okgronke.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3pvdjomil.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3oomiwfob.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvgcuihq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hudkddjj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ucrphamq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pvexvsak.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dmbdzupi.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3tjvcvnxh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3txzttkgy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vmeigxtx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gbdjrnvk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wbecrkem.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ktzxgqgt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3aszkhwbt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3kfyujoih.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3cmgctdya.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3jmhpvtgd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rrznoekp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3evfznbon.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zdkaljfi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3bzhtihji.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qwwttyvq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3jkpznepg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3hzbgnxmf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3qrqybtja.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3bkuxtlrn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mpnuskps.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sugdypwt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dtmhhrgx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hsgbnhjt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3urttiedh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3sskhapvc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qegqvhlw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mxubbyrm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3knexbkao.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kclbecxm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pyqingfk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rkgokiri.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ztbvzcku.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3stjeobju.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kyysvbtq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3feljocee.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3pcxtebty.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3wcimphxj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xhbjqcch.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3knkjsmnm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ubtrjhkg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3bsmfipqm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3neyvshtl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3sakxkyki.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3atztydwd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3oqynkxnh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mfvjongr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lqagunlj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3maxbqyaz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sugkpzmh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3obabvlty.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vsgtknvs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3whqrolbs.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ijlnnsxg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3yxejfedo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uvznnanb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lzdfesbu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zfrqbalo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nsywbgbo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3iheparnf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tnkkgzgd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pprssgvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcfwnqfl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zuopayld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhzsbydd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3etlbnzsa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3dnpoephc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cbdznrij.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3zcguxtjk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qnpaoudn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fmlwqsgp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3iqheighf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ldhskrxv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vbapnjef.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3mclgnwqv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dmnekrwm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3yuzgziwl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzkxcebx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3eubcxzpy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sgayloqo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3fualilbf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qxpbnnop.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3yztpxxtr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3bpuwcdtd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3kvmhpxow.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yahwqfqr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zzsrmkpn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kegtfnes.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wuvcybfi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3mmdajxkn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3brbgirtn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qyzocvgc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3dscehmst.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tydoirzy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3xtshimpi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wtargmao.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3flnciodp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xakfgzuf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mqwzfbmw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3mnujrzgy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3cvrpjhkk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3sojniibh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3berivusb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bvmnvwfo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3asrszdzb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ojemkasm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zbdhpqil.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jmbokvts.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qgoxvuxs.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cketstun.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3tkiylvjw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eqcxxpoo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vdvvxfwb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwfwbzhi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cayesbdv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kijgkgtu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3snwlerqx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sbtjbwpk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vpinfdwv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3pnkhnwcd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3iyxbpeyi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tmutuasm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3sxnebuqi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pshubpfy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3tqqbqruy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qpkybvlk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3cfcefmsy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3kxfxsgzq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vgcnqymo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3txczwytj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulkxjkdm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dzvkuvph.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wdoifkqk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3okezyfmm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hdzqssmi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3onjyxozf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aznquxhf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3fqkilori.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhpekswp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mxqifadm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fdfpsikr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iwczjkob.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uadvrfwx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3dbcrjkif.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fvovmbso.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3kodnghhx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3rwngmpxm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yypoaudu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xwznupem.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iuugwcpf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wzepqhuf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hhabkjzs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rwxowsiv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mlcdgquz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oiftikwo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jueapjtp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ancdgypp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ibubaqna.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmogzowg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iusyyknc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3edrpeavw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3yaxzzhkq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdudntel.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3crsvbcfc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3vouarvuq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3nogdtmyi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zskqnbsh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ctzjfiwd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jivlsxdo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xmlmxbhy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3buhnwnkq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rovwkrel.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3qlfchhwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jeweutwq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3nkgnjvvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buxksken.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3pgvzxbpu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3tkhtvsnd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcchymsw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3glfjefxz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfjkapku.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3tuvwinal.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ngxldbow.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3juoehzif.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkgtzvqg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tfjuhxnh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3poezhwnh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3yvtcaukz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3veepivza.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3hpvwdjgj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cvcwutmc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3qgtcmsgh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cynxxeim.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhmakqua.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qovqomuz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ivlyruee.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3eklujewf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xyoqwuze.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3nhsgvyil.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3zeiqfxnh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ywimqntn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fekcfhjs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3bwfszphu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3esshhsdt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tossrtaa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygtmafuu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pmgjuqvb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eolbllqi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mamelgpn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bchkoywp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pkoyirlb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fjrlylhv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3cidgzibi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3gmxewyxs.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3daywwgqo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gtsouwua.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3itihherq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixxuuzpv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3tsfhhqkv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3edtxwdny.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jwfiveyt.html


<!-- 参考信息 -->