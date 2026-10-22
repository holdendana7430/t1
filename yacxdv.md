代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ahmkuwuf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rmbvzcmr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bjpaztyg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jysenkcr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hbvcdabi.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tqxwudmg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2acwvkllc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yykehmqw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2wojvbaou.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2demzomas.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2texvauia.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tzxbdyyn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2hhiriiid.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2odisktzq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2dyycsvir.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2songzmck.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gvznkzek.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fnxlohia.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iktilxxk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rorxborl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2yygeugpb.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2chmdlytk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bhvjvmbw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2iwphjbqp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2vrgstnpu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hfczhjwa.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ubyrryks.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qfugiann.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zqcgxsob.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2uocrfnza.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wrcizmox.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ohtshaya.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2kmnpmsxq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2byacwhuz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2suwryotf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qtmrqbep.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2httqrvsn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2potiakpx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ziakyoqs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2druckodo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2flndixqw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rnnhnqzt.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xwmsmnuw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2atymwgei.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cgodgnbm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pnmafxbm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qiizvqyf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2behwtbzs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zpsypecd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2yqkaaxvm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2czxwwgor.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wqckjhdb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2gxommnhu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hdrltqxg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fofgcifx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ioctjaaq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kmipmmao.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hglfirtg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2huglotva.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2obwpxsmy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2jljdpapo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvflobdn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbjhistx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ksqpvecx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2htsdfmht.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ismiuond.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2xdtmowls.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wrlfwmxj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vtlplfsr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2yincqfuy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2sumaonop.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2jiqhptlg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2pdpwppeu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2opghoell.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2unaczxva.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2kebwfqer.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2icdhaqat.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2cxoxriau.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eqylraiv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2jynbuvjj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ksjbqfod.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ysmitahn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xozuodxz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnwxhmjw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2kahcilhk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fvgoyqwt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2crxcvilb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xcbxmjka.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gvdlcdlk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vziswisc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2finntfhl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xjvrdfpc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2lvlqnkox.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pbmcpfqt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2sfjzbckj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ohiqdzmi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fqepczgh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2uaxbwjfj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gbhzptly.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rcqczraw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fpfdqzcy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fymvwuyp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2prvjojsn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2yzmrmfqb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2xpgkwtlt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2eytknwnd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nmzuerkb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2skepjemt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xoiasbpr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bvdruqrg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pyihwtoh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2taonooan.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2kasldtvl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2glszilfp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2syqkcpub.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zcbhzkzm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ofzbpliz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rttyvpta.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xevfnrxa.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dqplprey.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2zehzwmdp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tbkyltno.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2uavyelbp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2wayevrfa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lvxviegk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2veswfbyx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2whlpknpi.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rctctwbm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ieluxujs.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2pkpvrbqh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqtiomtv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2qvcamydr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2hpzmbujm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tezlrmpe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2njqwokpf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hpzhemts.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bsojxnlh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2lolkigxr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qluypwfe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tnqivxoq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2lqdbzurg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2wambmtrb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vjxubyba.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dtvcxlot.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xvirwsql.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wffukvxo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2bvqixeya.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ruyfngoy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qwtmeofh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2foebnmeh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2nzwnlbkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwlqwvdp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2jxvkuerf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2mervtrgc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dzwpfldf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xxglocfd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vljggibs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qqnkdoxd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vpzxrhsr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sgrvouxd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zuqtodsp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ncjykklw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2lmuzbrxb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2penfspea.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fahncwvj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wcrcvqxj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2cmvmstyf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2iyrfvidu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2pqklbccl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2itoobsui.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2etyzhjhi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mpfurbbe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xvwynafx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cabfxwxe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uqgssetc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2omkhuuix.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2thucnusm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gmlcgwlb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tjquthll.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qwxyrmps.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2shscpooq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2xqrzorwf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2cxtgmpuz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pmiqdhiv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2uaftbgtu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ddkjndov.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2hwyjwbgx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uxrirmki.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2clddrbub.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nwjhqlmu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fzjbbxdu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eiroficu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkjxldhh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2boozfbup.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2hbyllxwy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vlaueazk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmmbzked.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2aktkxwsr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tmkdbgdv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rnihvgxx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kuykxobu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kqlunljy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ciuggrvj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2soeskwhp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ucyvrbie.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kdtxykuo.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ubdmlsbt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rbpxomyw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2epzpjtqk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rzwqsedm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2njaeemtw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2zcugyjeb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2yxdvsjwk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mdcvosoz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2adakmolz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fuvvdlhw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zfmwzncd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvxpeymq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2suajllsu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iargzajo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wzyhjplj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jrpmmtck.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2sjmcoexu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wgxccitp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2zdiubgns.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ukvjcydr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cjjzrmcc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bbaraefw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2aefguxqt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2txtcgmtk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2cgbspoyt.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqxycdtf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2cfyrgacg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2xonbmwua.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2romkeakc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kcbyqpjj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmgqpidp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvsemwqa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2rrxkutec.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bzttpuam.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ypjhntdx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lduijenb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ebwuwdqg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sewdzruq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wlrlpsva.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ytlfjxxq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2eamcllqo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zqcnwalz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jmtjbsrm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xvtsypaq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zyzhhuwt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2mhifgbyr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ldsnlaal.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tvdpoavr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2phkqyhol.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ngjpkbjv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2jyfzopbi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2sifoxeqs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2optfcugb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vzdjepnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvvcbdrk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tbwwnfih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxzehjhw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zmsxriut.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2qdfdvujf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vztvmjqp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzrbdchh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bbiojqop.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ktlpvvny.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mrdwmxsb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jgfvseqc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjwixstq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pwkkgstx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2jpevapbs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtlwbcln.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tbjvbiop.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2qqhgqzsp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jwgbccyd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2cvvhuinz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tuopcbqn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pmxagogf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2tkmrkozv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lxiflrjt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tzxtugiz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2klcoyihs.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2sawwmmnd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2lvbcimpi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vwrzqfbz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2bwymzeup.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wtcplgns.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2snijcmlg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wriaxlfj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2skjnqcsh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2akntcpvz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhubpoue.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnonzvsw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hhqcjudl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qyvxocjr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jzpmcitp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2fxwzrkmc.html


<!-- 参考信息 -->