代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hdroqqvx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3omemotwg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jmuxedby.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lvswznrr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jgtczrrp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3giharnyz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hmcaifkx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cezkfxvb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3iicdhwcd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pxrnmgvm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3dnodmzwa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3cgvysarp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3pongfgdh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3zxgsbflh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3tikafsyi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3guhcbfnm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qojlvgwv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ceqgyjou.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zexhlytm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vgsctydo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3hbonkamc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hsajfche.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vtljcswb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3wosdydwg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3eomeoyhi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3cfleggwg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qaejfyyk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ihuknbkw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3csfmwjfp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3fymnlsxg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3swtrryyv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3aslavtqs.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3kqgvncnf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3almzmuhe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nboapdrs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fouddrsz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tfxzaapj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cvbvwdxw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qvygwyeo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lmoslgbw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3nttdbaci.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bombalmx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hsloflwd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zetokclp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gwddrxuy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3keikojbv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vbwryqdz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jxyenmmv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ireqsfaf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xxhpcozq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3utaedenf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ndcistqr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3bxwjbpay.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3suouootl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rklpdumv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3pzwkzvgs.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3fjlzxqlx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zzfjixxu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lyuqitum.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3brhlswmx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3mjslfbhc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hqfxtezs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jhmgkonc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cyryhzxm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3djkiwaoc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3sppxrfuk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3gteutirm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3flzkncir.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3aolrrccx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3kbhycaiw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3pcyiagrf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3wlsgziyv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3agklgljq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xodkzgoq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3lakbwzoj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3bglvdjde.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3haqzblkv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ajvzcpaz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dqamqrji.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sasqiyuc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijsbtjmq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3lopnjrge.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3fwqraxtf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dubswjus.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhxzxejz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3anaqtfzk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wqojibyl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3htqvbebq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3edtkqlwz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wvesijks.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3owrpojxm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ztdsaaks.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3fsxxznoz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jxldsmts.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3zmsycwys.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3hcymxbhi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3jowbkcby.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fjotpjao.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmnuopny.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ofwztdkb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3vhtaecbn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tsnylgow.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ugkzigsw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3gajvtwmj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3yyjyjjqp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3qfcasyod.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zujvghbc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qtlicrmj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ffadsybr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3epavqdmu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pcrphmdm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rsdbwfon.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3vzjqegtv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3okwpbnlg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3gyvcopph.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3djjovheq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3btjahlpr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3exgyvmbk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3sjxozkqv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ahbtgeki.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3txzmnixu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qykuvmil.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nphyxicg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qkkreuoc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3hxsvryzy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3blbpqxiu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ngiqzmzz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzipruzi.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbfgwnwr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bxjdjolm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hugljend.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3lhwlvxrt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ugitofia.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gwegrjtp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lvizkzpo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oyzlfqrf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zxgcxwcd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3gsmtrldr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3chfogcbg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yxyghqor.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3zmjvpyaj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3rkyodotx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fviwstoe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jqcczlqt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eurxxvrq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3njjhznlm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3wymeltsb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kpzrrffg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kxkujxuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udbdvoly.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3chlvqegp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swhdjuhq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3itnyjjvw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3fozmyfxk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kxgnaecf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kzmamnfw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rrjykqky.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3evtoqics.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3zoxsceiv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vlnqugtt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cybofmab.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rwntfoel.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3fwzrlecm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvswfcaf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrpgrogj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpjtrxrg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lqoonhay.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qtcesoll.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wrmwsrlq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndjmpfei.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3indjzgni.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3byrtfylx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kyspcjjc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kqotlbko.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3foberceb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hjgewbur.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3nzgnfojo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3twllgnuy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kiwhlbco.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ottpxain.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vztpgorr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3nzsimtpk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ypnnciqy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nclyvnfg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3imqrylzm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xaflyebx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3tvypyego.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qgxwrnkc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qsorrzdb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3hsbqyejg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mrrgzsyy.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vzvgykij.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ilsjmwhd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nkdwgufo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tcdvznlu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qnzdnnhf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wficpqiq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qlfjosrh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3twbqoepm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cssmlsbu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eehylyxi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kzblgtbq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ucoqllzi.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xwlvtcnw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zzfwabtm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qygqkibe.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hdkfnaon.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jmrlndvf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3wthtdlim.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mdcmoqfi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3igmjwnpp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ctqesxng.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3kihywxqe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3bkbhkurt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3lpxcebwy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vcnmvokj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3gwyqetiu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3nufmoqsa.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hqqrimfe.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qilhdigw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3uxzadjey.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3fxvtvcba.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3zekbbyqt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3wmlfnhse.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3kscopiki.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fpzjpwwk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pbvfpedr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kldzqkbt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3chcucfna.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vjnmooyi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3bjjujqss.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3taulqoxb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3pzbtugos.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3sntdtucn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wqkncxif.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jbwulmfk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mnuswxtn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3galqeink.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3xnvfzgjz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nduqhzck.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jeoaltqj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xuebwiux.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3qdombucy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ginrbhxp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zgdlqsnu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dooepsjz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzkkzekv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nbpjcxbd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3oyfhbqfc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3egueqhjz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3yabusuug.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xdxtocju.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3umzbqdnq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3atmvupdf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3efmobxnc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3rheerrui.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3yhuugjno.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wfbmwmto.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zhotpvus.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fvrrutky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjsidvny.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3fskxuzme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvcuwpfk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3vlosefet.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3rxslweyy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wyjaatae.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ffgqoyvy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3xfpbpvcr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3yovfxpie.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3bazxgeix.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3spxygpnj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ijzupphk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3txtvqzsv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3jjkdbawg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vrtrfeei.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rewvzhrt.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfkgcczb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dhlfmkjo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3uoovzqoy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ihrantpk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rwuhtutl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3gvpmobba.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jviwhtib.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3obtyaapg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3looacbnt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wsrqmhcb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ngzxyvgq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3icnbtrch.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cspbcffs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3sqoeoowh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3taktfaze.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zhvphusj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgtlccuk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vezhmfuz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfkennow.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfcsxfzk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dtdtnocj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vdvqxskm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ykszcjha.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3iymalcuo.html


<!-- 参考信息 -->