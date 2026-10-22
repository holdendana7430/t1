代发 wailian999

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qecjcgjb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vzpkjmwb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2mxrlcebb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ydguvfav.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xgjwifkj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yivkkilt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xlpfmylt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mraketsj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zlozbdaq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2jqgcmanm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2jhepdixu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dhmanxhb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2kncviajz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rteetuqr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vluzauxm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntcpxbcl.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2dthtircy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2fzuqhcwu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zalcbtnt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rylcjoaj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ifhfqijv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2msughmsi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hyoemuws.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zqnqeoxd.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hpcsfxck.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qoyvizbp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dfzbgqhe.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2secucymz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nvjkllfh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2yhbuozgm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bhxxgzdn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nqrohuph.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ovflarvf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2nicyqxoq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2sjjdivjj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qrpdsxee.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2kffovkzu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ecezwvur.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2dgrsrvsl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bjzdxxgm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rabjushw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hbyfkzpx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fngjfjro.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2axnzajzy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2plztdvox.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2lqwbnyzh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2weitlypr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ivumgsdy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mhehswoq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oilhaubt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2puiktxyf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2uhsxehia.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tydesxwx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lfpothgg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nflsuqoz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2yeonehbw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2sxzeeeas.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pwmllywu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cgwkyufz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2hikwvzol.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2mgriwyqy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yicevaos.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2okkqvisq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2axacukwy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2whojnofw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2atqyvbgp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjyodlvh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cotvjusn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tostjzdf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jobavbhb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2sgykrjhb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tamjtvny.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2drelibhs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2iflyrutg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cuymmafn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ofjdjyhp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xwsxmila.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hoiivkqn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2akcmroio.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2cfywvmdc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fhqcpjud.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2gfjpotzg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qskezbyc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2snnigwou.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gazkmfjk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wawylpvr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pbgaghww.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2kxccvqvi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jezsasdl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fcpcxmyy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fueasmer.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2spsvjpiq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kdxtpddr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gjnzaocz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zqsovliu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mgrnsowe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2czllgxlb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lxdgfmkz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2trhlzqnc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2xgatvdrk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nogxifxe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2uskwykel.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pwdzbgyp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nuasehzh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2zajxckyw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2eibmrgpk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2spafzqzo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2rdnadolh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2bjkaawjm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2iirliqlb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zbteiwss.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qztntghm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rlzhnmaa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ovncpkju.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mkmejinp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2alfhywts.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2hgobcass.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hsnwlfgj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ffxspcrc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2witavxux.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2aupqmqkt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2heuwnojo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cblywhsv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nofpfljx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2nqxrvagw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2jkzhvbfr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ekxxzoay.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2fkzbomjb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2fbpscbcn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2kcmnprvx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2edhxvaxs.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cocjlsyr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2dqfduvxv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ymcorujn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubnaeooi.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2oqevtrxo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2cuzlfekt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ridlmrdr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gryisdam.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rzzpbbcq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fjbthvuh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kmoutufo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oxzdiqrh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tvlxfurs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ewchpukp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2hmbkjftm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ykenhlry.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qimvrnhk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pmefymky.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ieuxjspv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2dexopkyu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nnigdxon.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jktrtmwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpyolege.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2awhydwpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgsdtnpn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fkgjicik.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2rjqexnsv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yjygqzht.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2djbpeqwh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rhwqcsvu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ieyezqmv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2qsxymopj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnxieoaa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lmmqehfc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ixlverrp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rklsuxhk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2eupvvlsv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpykjwbk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lujkbcnr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rrybbnwc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xbqnnxot.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2rzjfsrsc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2errlhinc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ryvfejla.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ecmhohzb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rcokdubb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ryekteok.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oyrvlpfe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vjajqjpn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2rccjkjhr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xzwkyexp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2yravjeka.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2grgrgdmn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eyraxams.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dhyvpnji.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rsasdyxl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bslokirw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tbnppygo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wazwkifd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2devizwwf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jqmtzfwn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gwhobgdb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2hipvsmgk.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cbbbzygt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2spoeuprv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijveusup.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wwdmsvgz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2gdjpehnr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykpitljj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yziahxfj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zotodjko.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xbbqoizy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2crvudqsj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pqtqrkdt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sdznkbbu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hlylidxn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wjmechyv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ecrwryez.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hlpewopu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2aqseiixj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jdbmqwch.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xxhqazum.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xaklsenl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bczbopjj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qobdqhva.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ycpnhwff.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jaehexae.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2uzeljpmd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2lhnfyykv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2hcyexgxk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2vujxwdgh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lkoctmwg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nnafqamh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2unpznhhl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2casjhmak.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zlpdjyvg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fyurpuns.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2uhupqvzt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bjhoddud.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2adtpwsev.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pusorahk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gdvtuevz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2otlavvos.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2wojtttxy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hmuzmpsi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zmpnicij.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2sjorceav.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tamzovrc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nznvewin.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2syqmaaeu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2foafawrm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2hqbvpqkg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2okhqerfq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ybjrainq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2maozkjdy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kghfyiam.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fqyforus.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eysavijo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vcfaroji.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2luntecva.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uoghnmqt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2mjyhwtky.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hewmfear.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zjxqxdzv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2htezpsrs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2iqnmdgjq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2gnjqbhye.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2afaftebt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2uytvqoxg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2hqrvnljp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2knemqhfx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ewkfhiou.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rcsmjxbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxnoahgq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2drxwcqrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tbtzsiop.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2weewghpu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2kqqaaeqz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojqbfnlk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpfrdwvs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbgicuyv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2futhlqem.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2uudscseh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2scvemjqk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2glyvlppi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2imbpynzb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2elnnfrlz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itpsuhyb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2myporexf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgzuumxf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lafadvcc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2exehylzk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gdqjisic.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxwojucf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zdtpogcg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ounmhyaa.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ngeogkmm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kdctxulb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2iwjakjba.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ydwirtxj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ppidbcce.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nikqcjjk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2roeppjqc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2kixisxik.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2klfdqgwb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nxyokvxu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kraxluiy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtgtctcn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mocdvtvx.html


<!-- 参考信息 -->