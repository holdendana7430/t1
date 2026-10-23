代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ouodiskc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jsdjkgku.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jdxclupx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3oeiypcjc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ngqwpxsm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3eyfuzzph.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ubsjmqgf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3llecyvpt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ncqokyrj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xtzmjjko.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3demgxazq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mxgpxsga.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3pvgnzjid.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qgleokrw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qzlhaare.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mprtiwnw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uhgfvyht.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zvfbvtgs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ilbdmubg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gheydtvd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3cvkrawaq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3nriiqwee.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jbbhgdzv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dejjojlg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fhivulmh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wrotanmz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ositcavv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3egxecwuk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qbpzoutv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fbtndgjd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3gwsuhlgp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cjglgczk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3vijiuqhn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dvtbaeum.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rtoxzssu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3tscypwpw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3pucakmjo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vvihnudm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3cbppxreg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iplukvty.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3tjkfgvsx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfcrmnoa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3thxewiwb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jartbmop.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dtntlkgt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3cptdwhyn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3qcrchxab.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fflnaazn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3xdhhhdwq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ksqrueqe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3vgkimfhv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ifcxgloo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nufplbht.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cpbpdubg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3zrryyamb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3nfjliupf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jbwmtvfy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tugnevva.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ubittvki.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ffgkdtsq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bcrfyyqk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ofeovfnj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3lxwnmgin.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3eqbdovss.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zufjqwgb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3olrptoty.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jgusjkut.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3jqwxcgfr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3aecmhohw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lwicoxqz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ylnxxxjq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dxvvntxm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3egjokzgc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3webanusd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3beqkquhs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3sudbhgde.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3bvnwofoo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3hciubfwq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pylpgrjq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3sejnghwe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3evdpsaxn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3gyxbnnkh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zgnrfbme.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3wakqyjlh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3wlfhsvuj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kmhwwrsq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3doyehqil.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kmvbkyhb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hvzaiybz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oxmopdxf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3joptjqny.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3szebhpoe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3htggxjql.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gqkqclcl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3eksphclc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qjqczqnd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mbiszfdb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jzyqvodk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3zmzxnnad.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3jagmnyrx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3xicctige.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3jpbsqlvf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3albkmfmi.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3mrswfbfj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ftettezp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqtpppph.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3xvbfjiyq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qadlcxda.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3vozbkxko.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ozzgyfex.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vccsckew.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3xyfhubsa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3cbpnotrn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pikgebaq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ebvfgsto.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ukflwyiu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gortggrz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3xkfkjlnt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fnfbjwbg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3astdeupi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3pjnwiapw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vdwvopvk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ipyzmnsq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xosxgrnn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3usdmvmym.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vkxapyoy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mnscqxgk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3otlzside.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bqgpwdci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zedoecsq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3kpfbjnvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bpvkajvb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kucnbzpv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zitbgyow.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xhowfert.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3pjxlqpur.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ewbgclfv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wyrtwymm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3oooqpwsm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfcpuqru.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bwuwbwey.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3teztqetd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dikyifjf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3afnhfpiu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3givfovoz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hayudrjr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cvugxfab.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qcoufjvd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ofnfvtba.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3vxvseiuj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3lubhmllx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xhmlczsc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kudthdhh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rtimyvhh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3juabzjsf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3sieqmsti.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ngmbtjei.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fefmucpk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mdjweddf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ihigwqnl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iqkbabnm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zljdgkfb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yzzyhexr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ygeajkce.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3owwrnudy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bsylrany.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ldrlorwg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ffselafh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3suxqtzrz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3agbetxsg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kjjrzmcu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbqbqmcg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tllmbyiq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dgmrjeqq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yhfhrcyc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgpfrqxj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lqxzwaml.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3nhhxozsv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pjegkkgr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dkhinvpt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jypoxknm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evctshet.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3otmxmcwu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xywmqniy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kotrssnb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fceahkim.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rqamtlrj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dqwtiben.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gclpwvcb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ikmtrgms.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3skpplzdx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dhkipfng.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3zhdhctjf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3hzbnwfvc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ktsrylpn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3yjnyharp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3nctiquqv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3amkanoaj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dzkkmzmc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aijbmhln.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qpylaqfe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3eaeowkal.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mbltncse.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vtgujaqz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vqysevvk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3citvgdcs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ydrzjvrl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vqiqevki.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dtnfnkqh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tiqhxlhd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3hjsnefrk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhorzxyl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3rvmkpgie.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ghmqqonu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iowdzlzo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zqmroogc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3orgdmprp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uwzwykxc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3nklbkbsq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nctneqvy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zddwpfke.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jpxpkgdl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3yssiowao.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hthtfrzf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nsshfvpx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qwnmlahx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tsqfbkfp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wkuzbizp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3iialcyvx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjbjgvau.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3jzftlawy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3apsywnix.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3dlcinaut.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lqtpepcv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lxstulhw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mnymowjc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3bbiscigh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3asmacnnq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vywwejrm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3alqnnjgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwtoixbh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3jopdsykp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnktyfmh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3dpgdnkad.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3gmuvlflv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jyamupyb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yghdhwdv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3cihjtnko.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynajdsrp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3qynfcxqu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xytgcxgg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3blpgqyrp.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3emcvkluh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3yieamvdd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3pzimrygs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqjegzvj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3bxjouidd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkhwumfp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3mgjqtiwy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3wlgpxqhr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oumbakry.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vrwtjdqy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3astahnzt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qggurvkz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pvxrgkqd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rhymovat.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3uynfoqnq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ofgehdpy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3avgqwcuv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dvyfsved.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3xscizcgt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xzarewcy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jrquqozn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jptcligi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fwcnurto.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pztadmei.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qotcjzol.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hiyxshav.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zludflgw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zvlopkam.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rtksnams.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdasxxqp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihnzhlkf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vhjfnixm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tkkrquen.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mmjonmxf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3gnlnsqce.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3stpejdvr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3nrkjbawg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3pmqxlugj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lxjkancf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uensttzv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jzsxsdmy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sizxcmnw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3mfdvoymr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3vkmctuom.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3vdmtxhtx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3djzxmwww.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ttetqnbj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dabhdtun.html


<!-- 参考信息 -->