代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kmmgrmcj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ztrqczmy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2lxdtodey.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mcywcfcw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2mvjoryqw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2aplvrghr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2wyztkgff.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2eccnloed.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2lyczznoy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pxochlwt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ceugrymn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2yoxtgrbm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2dbanrije.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fdgagpdu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jhhjlmwp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lahhwojl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2irjufjse.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pkiaghdw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nkmfumki.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2vaorwgta.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2vbxoawml.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ocunrinv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tipayzfi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bhyocuye.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vocipbot.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2juvmqeml.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nwyzwdze.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gzkbitwz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2nigtsnia.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wirbdtdu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ezzrjrsi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2itfbogsu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2amlzjocc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jjbegyht.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dtzucyzo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tyblphzq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2xkubyrrl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cbysexwq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2psdpmloa.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2efofduso.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wecrncne.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uaxttodp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sqypwcvt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fsahsrfv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pvhjzsma.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lkyzeuox.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wxkkdbzz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jljecojy.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xfczwujq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2czmdjbao.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ktnrviob.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2pzgeehfw.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2pbjhatae.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xbijvbos.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2cdxxjdza.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2knvuhjsg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2mtadhoxw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2nyihqgkq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sriukobh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iyfjiorp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxtxuyay.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jozwxwzv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ybvmndgv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gmnqcrho.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2nnpxolhh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ikanermd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mucmcvam.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2nruoqzeo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2jzngqdwg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wgmtevxi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2rkhuvnal.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2cmpyqbca.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fuzhnalk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2hhvvppbs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bmolapoi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wvciktgl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ixeumvcr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cnbnjdsi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2rlsezvgg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2dnrqwoce.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2waxqbzzu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2vrmtbaeg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wgdbabzm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ovcwetmi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2vxinghoe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bxdzmpzw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jmvfgart.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2szebipeu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ymycdiys.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gedwvzzo.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2umbschdq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2uqgxpgck.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2lbingmcw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zwvhjazm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gusklwdm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2addqgjvj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ujfpktps.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xrfphwqx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2vhboljdl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2kkhavofz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2nwxibdcr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2fnvnzsds.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2qxoecnfd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fioczhak.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uszckepi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2egljfswb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zkkgvrhy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ptexfckg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2thjapjxl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2uthmtomy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hskkmebl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2utuqxltq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vsdgiuzi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ileuyjwp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vnivvfmh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2waewktcq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2iyxzbkbj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2jkccxjqj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jokgefhd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qyxytjvw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2iujoddoz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2atuurprs.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwguvbgn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zmarhzcy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2osabkodk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2lgpfkihf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlxghtgj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2imbdiwlp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2cvmmnhbq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iuuobzgz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2foggdwsf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aflxhfat.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wrgrilhl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2tufcasfw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wfzzlpdi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dvnnbzod.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ehtwkyss.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vziponjs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dflcweaq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yfxrhsfx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cpkuovug.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mbwrbaja.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2miarmfeb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dmtsfvov.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kqzazgfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crsmdkqh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ivojzkmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2joahnxpy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ienlkufn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2lyxhuuvr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xpomxtea.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ykxhbiaw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fifyzjwc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mofapfwm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2xiwsyjou.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2apxtdmar.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sapkfyun.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2vuyljwtx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ldvvibac.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhhcsfku.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nfydxuvm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nngymjzl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lmpddbrn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2jxvowszr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2moahivif.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtufzrxk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2mhqifprg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jgjnevfm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2upyrstal.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zapidzuz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2obvubvgs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kspskjgj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jhkcqohz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2tnpsrnbl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yovlqbwp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xkumxszf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bmkrdjfq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2juqklocm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ltgicgzq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2htqqpfez.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nsrhatzt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rfczfalf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2yjbcrqok.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pwzslqej.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sczbkjxj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2voiyrdum.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kmwdexpc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhflkipg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajxxzdvc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jehxxxjs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2tjhdyrwl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uyqpjgvj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wgfzamkh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2drsfysbh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ujvhqtho.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aadmrsqn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2otislqnu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sdpltaqq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nmvhgoze.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pggrmrtb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tngghjey.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yuyehfrl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2slsblfhn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hompucxc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2kxleuvkp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ttuzbehg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tvkyurpk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2mhijgsjt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ufbvxaxv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bvolayqh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ufxtjmxc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2tdzabhxq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rebbfkeb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2uvgkdpmf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fzrdwngb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hoqpcnhq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qriusubw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ayrzmdeh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gyxeuvlj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2kmwxpugb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bfvqiapq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2doyffttc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2agpcqhos.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2oakycldw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lkmzridt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ryvewecu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2abjybtce.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iolkroyj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2bclqvlov.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2jnuneljv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uyjpsipg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dyzuudmv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhtulcgh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vfetbpwh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cdksakjq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wxtqfpoe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qrudnwny.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xbqtibwe.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ebvalgyv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mydjxtpx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2bguclkbw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jpomqeno.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yfefypkv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2apsicdlx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2pgufsrer.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jusgxgvi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2crchcrug.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2dfregwmw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2snwoohdy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2uisvlqwr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2smrcwnwi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2iyvlrhph.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2mqrneisy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ydlwisbu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2wyjviwkr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2udaxyfmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsxjvayf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2utirieuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2micqunab.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2jfijkdic.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2htomiliw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovmzygjz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2npgnharm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmfdsizd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzfgzapv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2yyvyansy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kqtwroqd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dnvlpwtj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kpohtgiw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2buujhyjz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2rrratkcv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2uzacretu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2bsodvfix.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2avzdyrep.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2cuayztnf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2uqsyjlyy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ixtpvwjg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2aibziuqk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pctbvkku.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qkzfrcex.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sxmfstey.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ojsvuktn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2elvqggvk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2zfkfajzu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2skyqaauq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wbnzghnf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jshewwfx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fjnbswil.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xkmxuhyj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jqakjcmh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qripmrqf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ubklzwao.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jpaquxrc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zlaeixxg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ywtagyrt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2lnwywkdy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2plsbuape.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrnmwiwk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mavaynnb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2taafzufz.html


<!-- 参考信息 -->