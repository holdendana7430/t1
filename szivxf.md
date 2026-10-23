代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bezabxuj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3idwfltsa.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3colgpwhz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3cpmlzrmo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3mqrbheqd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iqtjmdxg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ypnxrsjx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3sgfbpqpm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fwdogkvb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ghbxgmen.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ggbodhfg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3thvpwquh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hrizwbtx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3vsmirmvj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jldvgvxt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tilxkdod.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ppqkgtzx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3inpfsear.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3sgckjdfb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kpgbdves.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3flbnbllq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3onbqcxpv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ztdbbzxr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bctcicwx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3gjcrbili.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3hnzrvqat.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ewtvgitv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3efanffwi.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nfmiznaz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jiowgwug.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xflgycjy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rkjnotmi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vvzubgwh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fnyzggli.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gqhkmduk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hhxqkeqj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wojxfjnz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zxziaoig.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3egypssfh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3zmitncpc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3tycpiszg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zpvrpcgs.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ueeyoste.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rkjkndez.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3udbpkxqv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ynnjfbod.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hyijylhj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqvmpxgw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ixsbnqeu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eimbcaso.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3layfxpxt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ljaffnko.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3motbyvor.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3mmfxileu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3mjdzbquj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3xhqnnyee.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bvrleuvx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mmkmkdzm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3uwdykear.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ukrnawei.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3klfqobge.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3agugcmcm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3jhsoguxy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3mutnreeo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ozvhdvgp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ohthiogy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3umrhcpnd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oebcmunu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3qttqjvzq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3adodcxlg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wbuqiqxk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3govbhdqy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3shktcnyy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yzxcrjnv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xenjpwmd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xwflgnlk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3uvurraso.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3gzagxnxm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rdbuyupb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3csefraao.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3tggeglqp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3hgdjzztv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3khcshodp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dryrlpqh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zlwmwaqw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tafuphws.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mzvjfujw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xyfkqxdn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3qkgghxos.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vfbxsyjn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3tjynddrb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fkixhwwm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zqbakxho.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ujigrtef.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kovjbrde.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3joyczhur.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yjbylnep.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3necospno.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3uvckatti.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zguvgmxf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wmpikeuq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rnzeimzg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zfjhgmhr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3wgrzcyzt.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3njywemvk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ygvhuwju.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ulsdivfa.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qufvdgtc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3vawtpdmc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3awsbfzll.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqbaqvak.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3smfvacwk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3igrgbhez.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3fulvjemw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3afaxmqxx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ldujxzpc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3iqwhstyf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jqfsskqz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yhvpholt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3delgfrsx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ldsgdpve.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3jlkaaygg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fthtgzrf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cofvhnbt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fxkhjgit.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3tsvwxedf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cmqbpmrk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kjrgiqjf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mufasoii.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pvslyzsu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3vadngogn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ibmeznys.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ljqfoxzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxbhrnab.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3kyuyrhdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glnfiwiz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3tvubwhek.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3mgklatug.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kqzxggsw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3yymmqdis.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ygjqraef.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qovzqxww.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3szklmwcd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cswolecj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kebddycm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3cyfqbpmw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3megxphkn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngawkukl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqoyqqdi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qhhrvznz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3smgfhubn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xjyzfath.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3rmwndcuy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpeqquwz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ktfcvpws.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vtymapnx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hlswomjg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tgwpahuq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bkuvkqak.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yqyigsyb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3dprhlkjl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wueetjjr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sdhyuhrb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3upwdrspn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3inntopza.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3plunytvm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vptyjkrm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pvkswnaq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3afttzybx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pekmcisz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3xljqgwzc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3greqjstc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rlxpfglw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ezpamjbo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nfcrtkgk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwodrqmx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cahvjvpd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rhjudped.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3sjrnpule.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cjaqvfxi.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xsorusjg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ttlaoyxq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhkmasyw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bolazuyq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tubczvbb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ebjvzxnf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wkhcnirz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3plvzwayt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jgxgcrmm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rcqyfyiv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3bkitpyef.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lzfddyvb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3znasmfrz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3aolmcxsc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pzlaaxsg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3zfenrkat.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ndlgaayd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3oapuyoxo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wdhblrqq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3dvhdjgqy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tmqaohoa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3agcknfhp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xttmnsej.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xywdssln.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3psiwtigj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3bxcwkbsw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xogsqrvp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ccyefwno.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3jhifykzb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bucrlapb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3czomtrpx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3eiwjtjwl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3amhxmzgk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uwcumjcx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3owseheyj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hawbpibd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3umnficat.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3erxtdaqi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfpvekjv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3efsiqplt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ffjtyjei.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqslxjmw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3wgajrcah.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ztkjeigu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bnypmdpu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3usdpkesf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3onuwnlmz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jfcixxvn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xpszyxpn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjdjszzb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bknrxmcp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ufwqkart.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3eblcsrar.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ugoeoltl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3drvcrxmm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3hituivhs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ynhpscwq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3parmdxoo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ipigoqmy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ygeydsmq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vriltxon.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3sgiylkhn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3plmecnnc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jikxbshj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbadwvhc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3fqmngyos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iirunhoz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3lhuizwsx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3kowifegu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3pkicapyi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jouiyxmo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpcgdqln.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3nexxtzse.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ktxlmwzu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3bncjgdrf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aawmtqva.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vwurszwv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3sovptwdk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utwbmxmd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghfpqcmo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqvrfxpm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3iqrxhwxo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3azmdrlst.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3osbeurld.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ppfrtrsg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3nmfkpxbm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3prjxcydb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3oxqjalky.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3llsuasdd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3icpnnvsc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3fykdmuds.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3uzciekdi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vwzyvamp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zflwxzeb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3tmmmqcet.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3sunezjwm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xftdhnxs.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3agxodutf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpgzsaib.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mxprbtjh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3iqrvepju.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fzrzajho.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hrosmqfk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3yijikqeo.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3qbwvzfpb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3duoflafc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3txdoffcf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfvtqvhn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nbzgitwy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3yfnotgxf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qkshdqsn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3miydbjmf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zqtykjfz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ereunifk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nnqvdyxh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzolpygm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3orakadhl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrboiaus.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3gpuyumdm.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3yxloqiul.html


<!-- 参考信息 -->