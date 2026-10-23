代发 wailian999

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3olzvsvsi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3udhyrqlv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mntqtqhr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wffpajkw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tqeiuasj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qxwitkru.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mrkephgx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jtdixesy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ocbiwwan.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3xfpremag.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3jxadbicy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dwwuuuei.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3yuhokmks.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3lqcdyvfy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dppfztoe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3lrgsieqf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3jixnlwwh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3nhtjljes.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3atocfvlv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3gyzgbzxw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3msvzspwv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tlhbqehj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yvxrzcfd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3cunjwjpq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3mygdadrq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kstxakua.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3veyvfbtn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3rmxkwqyx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3liscfuhw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3arkfhoel.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jnngfhnn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wiodpkng.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rybxuzxd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3lqojtavo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kssqomqs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ksrznfbs.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3qntasdxk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qyflyfvj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3chnzgchy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ibayvnzy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oeflvdew.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lpsxigiy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lgxufaju.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dxfqrzto.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3hwhdxueh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jutiuyze.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ybiepkbn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pgnvtell.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nwrozlro.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tzlktyml.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3prdozqln.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qshonicp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ogehsfhh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mkluyimo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3eusvrfou.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3eztgnlou.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zakovjvh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3veemhwtn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rtpovedj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3cvvdgtla.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3gssdsiqf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tsedpymz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3hzppxbyg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gqgpfdfx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3vokvwgga.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ymlelylj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qllkhhot.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3maegsaza.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbjcofgp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3onzflqhz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3jnsppndt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bectldku.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ibqkffln.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ctvyqtkn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3cdsthjth.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3peavjyed.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ozjxyiut.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wtemnbtx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3orttoaiu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ihhvwtgl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dpqgifci.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xlqlshth.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3wizzedkw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3usdgtfqh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ybxvgyzm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3guipieel.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3dbsmbaxz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3fxkznlwb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qutmgssk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3bqmhbyhg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lqlajlcm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3lbytbovm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xdipkwuj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bozimglz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ldnvvsxd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bachsptl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ytnwhuhp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ehbesvuo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3jzywwcuh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3lrmcduje.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3gxueubps.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dndizlml.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nfxsoiuh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ppidlhgc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmrjmdgz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3iudovjyz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dcgvcuvc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3useyetvz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3cmxkhpfp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3uvrvyuru.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zscxvldt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sqfceoqd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wiqsdgif.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lsbdbihm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3derwhkkd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wmvojmle.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zjxvafdn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3sekdtpnc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3mkdahbsr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fococepf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ugzfidnu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dwdgsgvt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qegotvcs.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yejzbbud.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3byhiipyy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ceezmvjo.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3cocfonab.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3oydjttya.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3tjmexpuu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jufknjfx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3cchgkqsr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3aywlnzbt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahkfyynu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3yejdfyjt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvqpsnur.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3pxwlajnj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3qbdgudih.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3giadezda.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3khjywgna.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wbvqrkel.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uunstcjx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3hqqxcoga.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3urxtetnh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3leucvsoq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jfgmcyem.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mkwkpxpb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ybfcwlde.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3crvmylaz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vsrehjkt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3frxizjyf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ygucuuzy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fbaetclv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3udixfedh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jhysnzqr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3hvczwwns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvbxveqz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3khllyqku.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3dbtkaiph.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vrfyujwc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3hmlsgfkt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gcmygnwn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rfcocftz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3zjugxtwl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fsxuthjg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rxggtimf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3wcznycjl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3xzkxtuec.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3lnoyazvs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyzbgpbr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gljtrdrn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3buokirez.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3cfioqhwg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3pmiacdrg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3bsxspshf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3efggwhiv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lhnygwhy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bwsgrmdf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xmbthrqp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jiabylcj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rwpxsusv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3dlxfbnjy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zhizfxzo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vbqtqxjm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3oxrcuorq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3clbwbysh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fuxvfpjd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3svmytktf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3esjimylo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3kinbdltt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kyjfzoml.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3rbivpiwv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nmtmipuw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3oyojtjih.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3rctqbgxd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dirrmxuo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehdmbsyc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oizxmvdy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cbknfmhg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3vexpkkjs.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ywwykuyh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ovfwfojh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxjayynv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3opnivnhi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fzigimyo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ytqfegcn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oxczoxpa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iotptcws.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oyopdwra.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dunozhuf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3olygtvlg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3wfvfgzlp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wcjdvlev.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cnuvbein.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jqfcpnyc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ecldqgeg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3eewkauiz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3owwhovnu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fuemkqxi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3kzydxdtf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3cshvcjcu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lwkszlne.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsyzvxqz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3anmnblcv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kmonsfdk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nmymlqqm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pyehguml.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fjcifngy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wnffpiwn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3tgupxjpe.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ralwjzgr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3offzyyfc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3llwxxnmi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fypcicbd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zlktiumx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3neiwnxby.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkbnfrla.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3htwyiweo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3hkcxexqv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3guclhprj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zpkouelw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nahydrej.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fpeknwqo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3rpvwgyvu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djvjtilu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rgtabiwz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nzgqvucp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3vpsjqcff.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ttzuhauo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oclecosm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipzvvcsf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ohhqrmyq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lidsdyee.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3nelquvbo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bfppgsub.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zapuorki.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ixypwdna.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ufewnlbq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3tiaqxhgi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hgigrcby.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wdrfacxa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ulwcnjxp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3pqkhyhxh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3mjgeviho.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3gkhvtxkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ictaxgmz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3wzxquawz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzkdbauz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3cjpythxw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3acnsszka.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qpijwwam.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbghhpmy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rotfgvlp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3txlfbfab.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yuovrjad.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3udaypjjs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3igxjjnhj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qegectwy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3iqdashqg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3bxanahse.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tdihpuru.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kisgkeuw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uefbvefz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3nyvlnxub.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3grlyhmiw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeuudydl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3rcrmhulb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nbhgqdck.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mfkwdcje.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yflbrgyj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xsqyxixo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3niygexed.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hdkjizqa.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3urelhkvc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3qkptatsq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3bamzgxoy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ncsqanni.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mpflcnzs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybrqoddh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ludqaifu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3shklstlp.html


<!-- 参考信息 -->