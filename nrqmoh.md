代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2txitvthu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2thmutbba.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ojigaxis.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kzzpebxx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fufmgflc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ekdxgldp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hdgkwpvu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lfsktwpc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rogducwt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zvvwdwxs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qiqcgzdl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqygpzzd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2mlgrmikg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2zxhyhhuf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ocaqgnhh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2qowegshq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2xlguupkk.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jrreyvyr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2doppohuj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zkxdbsgj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2alshoqiz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2upuwigsd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2crdwocmo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2yecbhpms.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gnkfkleu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2etrjqxce.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fmvbwirq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zxibraep.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zthcuuhn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2eeantiya.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2itaynhey.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2njovcjxj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2tykiwwzk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uurwlbji.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2nyqmudhf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2blbibxvm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vccbupvg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zoiatgaj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bpqcevgj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nuystwuv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2pnunqiow.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ludiegph.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vipqwdhw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wdnpvhsw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wtrsydfr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iexaalgu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lualrppo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kddrpfna.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kpsmogzr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hstadtmz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2txqcoidj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hhpojjjd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2qecqlloo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ngjdqfid.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kusszzfb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xydiuimy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2wxstmdoi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2sfhjsnzl.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2nytkdmla.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2xkpwqjxp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2umxshnhq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ttahuvpr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sucetlua.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fypwdbls.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tdouhsff.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jvtiqvqe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ivegtler.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrzefhpe.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2wkgmwcpu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2hpehasah.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sifnophb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2twtqeuqx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ryjcuieh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gxwrzani.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2sotiyukh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2nxklokke.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nwxxceti.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2saotnalo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ymbgpret.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kbswmlzh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ufwriqpf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2djxhkcuu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2eesjzyax.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2acttwtmk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vkcddtcp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2elmcsqrj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2gbejjudf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2qemdhxpw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2zcszlkyo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pehjalym.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2eyvdygmg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2awljoxud.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fqfgwole.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nrnzviay.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jmkknhep.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2iqmorftq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2haulaspv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2fwstdvqa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kwtevrlp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tudqvlgf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eeknxqnz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2vprcvezj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ephpwliv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2deslodqg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lruwmrzf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2gjxqvljn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zgryjtdr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ervzxijx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2czopbuhh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fvytujco.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fujqcril.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2aswinbfu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2qpqnkqib.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hxiulxcg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2fdkrublc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2annilpwv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zoaltpwo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cfrfoaqq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2imtjjaow.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ntgkuiaq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2kwlfzfco.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2hfydxeiu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2kxzwxuhf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2wwncglgo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2cqugnmmz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubtkofwv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2tllydcqc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlzdcqti.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2qyolnsok.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xomxgovd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2iyucsmjg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2okpsnjpd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2djgjisiu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kaeidxgz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2syrtfhxr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sqluxsxl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ocsnvvlp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2jwzoonob.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hafvrmfo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tduywdqa.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wxlirvnf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2imoiydew.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qxcrbznj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tksxykmz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ilmsadfv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ugteofmr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2qybcpcwg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xfdplzzo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xelajpbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfyaxung.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2kznmxnyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2neyrbcaw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2lybghltn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2aefzoecj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lgzscggc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2waajtfog.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2flgdagxd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xpbzvfuw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rmppsokg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mcpirxsg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rsxdvgpk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufbqjeqc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ayfaebsa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2cblmglgk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rtxtaebb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyfwivvh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fxngnmcw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ahvomcti.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2vvkuvwpw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmvzpuoc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2yshabvio.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2avrktcqc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2oxkqzxrr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pquylfgd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2luvreinw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qlpocipx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2nqxufdpu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bwjvhjyv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ywntzrva.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bxukldkq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rffimrlv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2kefpvitf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mmxltguc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vmilplkt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ssgdaeqx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dlvqbsvc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2qwqzjiej.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2yzjbsdmd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2eyhhgmmt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2gmglaqte.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kdqqcfpm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wuzspfws.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2apumoosf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wbimslgd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2yhzbkhzf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hochrfbr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2noizruas.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2yitpkrqb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbkyngiv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fkikwbzs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gedpwwkk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2etmhdsru.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xgwxeddh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fukukwpe.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2langsyft.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mwdtmkdt.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jezajplp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zxokjzrg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jhqexqfd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lnwidfqp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2eavbnbpj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2eegvfgcg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rrvgewah.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2htzpbvql.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ugmoplib.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2thalezmg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hrnridcu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2tutftcvr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2arhthebe.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dgwkkirl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ieucgsbr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2imzaowbq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2tqjxkipe.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2aigcohyh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2eepvbwfd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xhkyfrvq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kuzbkolb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tjtshnsc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2omdxnymb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jksxfypz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2jugjmkqs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qhlqespm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bhmmzspc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2preegsrx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovotslsu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ftpngopc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgwksccp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrxidxak.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2nyluqslu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sdzerasb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2knibfzjk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvwcepkv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2pbnwxjvq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xkbkcfaf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2leckizdw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jmxgaztu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gxrrslgs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jkgrkfys.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2klwynjud.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mrciqjmf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2zzaxmwju.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2lcjmceqg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zyvykqqw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2lbvcklon.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2iyonfjfy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zmltgpzq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2pjkcglxg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2bgyrqzlb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2sddpuysb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lltscdrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhvrxoxf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xwjrfltz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jgqtxhlg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2eucvuqgm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2qpdcjpmm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgmjeleh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2syeczoxw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxcyqfqf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvicgsnc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ppcgmgvc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2evlieefo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jnauhhnd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pjqpstbj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2gwejyugw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2deudezae.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykdlabvi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nsrhytth.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2myxxatoy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qoqtghju.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wfspkroi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fghosemx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2revfvlwa.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uupdhkgb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2txhwhjfh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ewdeumdf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2srcfkfsg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ilniviyr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wqkkxjcf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2necymyat.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2agrfealu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2drkwkvof.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vcylbybb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2doklktgv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qivliuej.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dvkjxrnv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lgbfjvtn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xlibqvrs.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mjehmzch.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jkasjfog.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2twzmyird.html


<!-- 参考信息 -->