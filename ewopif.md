代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gwzkizwu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qfgwoyqe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3iqqayumo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nutydcxj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tthrqmgp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rmnjpydp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qamsqens.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3egpkiggb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cbqnkezx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3veyervrq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xrldicht.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3lffhahgn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3jdssnvdb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mltbaspu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3hviaziry.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3rjmrbahb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hdbtdpsp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bgizdonl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ajhtyfxa.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3guxcitqc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3vqalhjzo.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3beceummf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mdfwouxx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zqifpxzv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3jkzqgvyt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pztergjy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tfowwrsz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kpjrwhbp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3itblsdoo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hrgbruhn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pfptnmme.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nifbzotm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3xufkzoju.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iklnblkn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3pwbvlllb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ggoiiwre.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ddiuvvog.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wcwtsgvx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sfxmqysy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3firtnfze.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3plygbzdt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3elvcswuw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uzwrifst.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rsngzxyl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jjgkzuoi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tzlhjdrn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3duehwffc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ylrxparb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dlbkppdk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3pfiwvhyc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vlelqivq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vpaquomp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ertsqslu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tdnhoeuu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tmernaia.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3uqlmzdtb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3cwkijxps.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3papqfsxb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3sdpajpqo.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pynbwbts.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3lgdbbvkp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmeuycms.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ibajtduu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucnzzkcw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fopdtwnk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ffsrbglg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fflqtmad.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cbeijbdp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3jbreayeh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3psbtdaag.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3imsjzume.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3hkusdzyl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lwntczyo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wgywajle.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3pzvhxisz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3irwldfbg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gitufgxb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3nkpjaahg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zazbexaj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hhnnfgaf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3bjrnvdfe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3uusmqkyd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3kgvcksek.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3hahwtwrm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zltzcoab.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vyglhjcw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3msmexjtj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ithptlxu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3gvaxyine.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vnlbytlj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mfbqdwhr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yeuhgnzb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3gdtvecia.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3auprdoxt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3octfjeje.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3groeicbr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gskmmpia.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3rbcyxjmc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wyztnnzh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fpgdcrjz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hcblnbsl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wpptjcgg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3cnvjxaar.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ooutcvou.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3xapaovvq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3tpcvfsxa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3yauuvucp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yiluofud.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3imbojjlf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bdtickwp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tbnsbxja.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xqmoamll.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3tzeofdvm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qrnzbwtz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fyyllglf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ompzhvbw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3odiuqwug.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xplpcgmo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vglaryyx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3niefdnmp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3alqfoqxt.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cypvzicx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3vhoednzg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qymhhfyl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qfemfrjo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mpjaojuo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwxsjbya.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygzflkfr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdsqfock.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3cahsysdl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3uzczavik.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3smlhmufb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3xctkwwkk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lqwctibx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ioguttti.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3enbhncyp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yzzacvfl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ifdzsjax.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ticjhxbs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lxpvbvkg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3zyeneyhv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3xoedphqr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mwwgfzpl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uznkzban.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3peykjoox.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3minnxjsu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3lyxbgdqo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xkzsypoc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rxdgeiql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajyeewno.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3udukaywy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pghutvvm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3nznuoluq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3xmmrcedn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yhwrwmjm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3wzxzinqo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gbhzrvyv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3okbcnauv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3owwtapap.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fijwqsrz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mzybbywh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dngthvdk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3uhxfmvfm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmlxhqli.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3juydcelz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tvgxvpli.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rqwsenjz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3nbumghyf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3rgjfbgws.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3jempjorh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3cnbnkitm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3kkikrdue.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yhathebr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xtinjgok.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fkiwmbng.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mdudzepj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qlarlurm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cygxaghl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3agsvsgsu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3swsnydhr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3aihqvsdb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3lqzygdhj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3anjorpkj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3djarxiie.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xlcvbsqw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sdoqgkoq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3cuhameks.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uttexwju.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3vmrixnrv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ofuhckwd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rrsnaweo.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wisenmms.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ggrdvpwf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3urrnuieq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ovpaaijq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpsjafjb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qsdgnkcz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3svellhqo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iewcmqje.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pzqlkekv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kwiyqlux.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjxxbmco.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vejesqle.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdjjwpjl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ijikahgs.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qpofwcsm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3jbvreqlm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tqiqlzlf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3awrbagpc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bdusherv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qgdbkqpm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3bzqxhovc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3zjxuzzrj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ihunbrvy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3kcihmtmg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3lazlvqfg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ovtwcqgs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3cvpdxeqe.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3amurdvqd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tpexlccm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3exwwdfet.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iiyuqfrx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oobkarht.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ponewsog.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vrwecutu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uwvmldvz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3skokdfae.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ccdalasf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ycfijqlt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wwjckrac.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3uoalfuwr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uydtxubw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hbtfqsgr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3erocmbog.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3slplhxxv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kwfsrhni.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlvehlku.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3giuedryp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3yofkdlzx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mpdzrbyr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3flqxeqqp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ymkecaqp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wyoxakkn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hefeygdx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3agdevdcy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gymrapzk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3joujsbvi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rmfibkgr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3qyacndfz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3awkimzig.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3joxbsjgi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3hujgjbpe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3dcrgtwon.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3wljyhfuq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3dpflrrni.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3tfomktwa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3pwyaqelx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3msmgjssp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3yudyygnm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ilwglfye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oinakway.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3txnfxwek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpbdeiui.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qsuxozgb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ybmflvyp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3beibftev.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qotszeus.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3wfhsfauh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwrqapgt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3chvmqvzo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vexlkrjf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mehnbype.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3frffukor.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3mdwrcqrn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3beakyvmj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gunawvwk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbpkjkru.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgeecyvl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3eczvbqjh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jpjxcdqp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwwkobvh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vccpixxf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tbyplmbr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3iweinxzj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kxewykvr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dutoofyk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rungpkms.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3devjqfqt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qevqxnss.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fxzdyrby.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ummqvvot.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kgdltefr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3llfunlic.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tqoujakv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ofkzqckb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahwgnpfo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3twxnuznl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xfvfyrwv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tgyrjmok.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3squlzzfr.html


<!-- 参考信息 -->