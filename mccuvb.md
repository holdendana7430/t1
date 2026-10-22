代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2jmxeenxg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jtprbpif.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ehrqwobg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2olokyiic.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2yqofjeri.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2oaekfnth.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2notwomww.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2syacwlht.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2aaiupfue.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wwfajbxc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xtsnubwk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lfatmgby.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kbntjhvs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2yfrbvkjs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hdeugbgn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ndultcnm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ilergoql.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kzwxqspd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wxzbjlne.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tlakusqp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2opkslsgk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xvkieaax.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fimgeetr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ddhodpvj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ymefopwb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2kjeyhpdp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vjutpkuu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tqkkqdhk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2asnckdnq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2shzgtmem.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pmvflcys.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2phubvxdz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2aatubbnk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gufcmvez.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qgmywcxg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ykqpmvwp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2cqhinvva.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rdmfldub.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bahfccuq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2tpbgceyo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2czsnhrou.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zgpwfwjm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2vmfgpnxh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jpqqjuwn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ouzrxykw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2falczfhg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxbwbjbn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrsybiuv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2disubhzs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rqzcrazh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2aonftbzt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2auuwqlmx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ttzmncwz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2rtnfatpz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2evlcvwul.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2hrwkwpzs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2scfuzwxw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2syzeoblr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2cyqnvbmp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2lnlnnrkc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qokubngy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vuqwdfrs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hpppcndx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2rwrsqelm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vfselyer.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2dvrmmgkl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ohpzhbbh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2gbcuqitw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wsbpzohl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2jenrcbnx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yxgkaxcc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rhylylte.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2fvfhqftd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xntcirwh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fsrftzis.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zkyismjc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2thrczrwm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eguuwvpk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2squcjxdz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2gscukvcl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2yxnwjtqn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2dejwbsmv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojvmihpx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jrfnwyat.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzndpcwk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hmhbdxqu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hlyfgkqe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2hlonlsmc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hhwgogfs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vghvxnni.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2snojnjdj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tdrmxzil.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tmxoopzi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iyxypwmy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qbhmwntj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dpvqylzo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2qbabcnhc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ypynfftd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2zmqeqpzx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2iklmbhhm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mieafpak.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mvccfjcy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oragaioj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zlhtarim.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zxobgayr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2wdwohzds.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2iycuweuq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kdfvlhzy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zhhssnxg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2yrwzzfkg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgkegxaa.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqplgbzf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwajcwyl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2eorvwtwi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbbbwlwe.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2cyfiyspv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2juyuiphb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gtoopryi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ctxdoykm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kfyjruot.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ihzibfjj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ssaraqok.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2norxdbtf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dqsfpaxn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2uufnzhuy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2klurzooo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vzutgwzc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jfbbdkpg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cmforrdc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pmhklcuu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2pzweljku.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dngswbns.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dtnobzfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bavmrxcn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2uzcylcua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hyuqdcuf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2puzscwgn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2kixybumf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dtyfhwwp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2fxxmkwqb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lkprhctm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wfvgyoxn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2mswhhqrx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ktmrxbfd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lbvqnrod.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2pmrbtcjd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2qofaydoc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2stgdtmwp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqaocttd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fdvntyeq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xcoppxos.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2kvjboyqo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2wojexlzz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2yxpnqlqn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ttxdfovo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vyfwxhcd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kigtujdu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2agqvxfgj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2piesuhqj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zkasvmbw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2kjutroul.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dbsmoeaq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uaxsfkka.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ebmukzmd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rivxeude.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2zjfhtoqg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vhcjqnys.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lhyqereb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2odnlghtv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cfzkuxrc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2msttjfue.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2mutvxehu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ergdpxpe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rtmqdltr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wqhnmizc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfubtzta.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bandeytw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rtkdvuwl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rtzoahzu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adgomruy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azmzgukn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2buvsmhxo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lgdepmrt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oqbnqvsf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ituupflf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dkeoaawb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qllkmnyz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fkfkubif.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojrrehmk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ubvmunro.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2fwktdgad.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qwwtccej.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yunrnvbo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2aztpqwyv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2thoedoam.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2itjosica.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2xucessra.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2kvicawyg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2vzwmpwxj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2kpjkikmi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2sxwtbgvv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2kjwlnlas.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zdsgudkb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qetoyiwp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hzphdjtb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hwmhskyc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2wjpyrhnq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ezdtjelg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2flbzalrr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hutoecuy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pimtlgmn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tmnmvglw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2htoaalqc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lwqnfaym.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2kysecebp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxavpwgs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xvrdofrc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zielinwe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2difgqpfj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dzhcwbxv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xejqtkys.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ngufflbd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dqyshzqp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2teitvlth.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksruieqg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rmqafvyy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ydrljoti.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2alvywcpr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xxftjxvd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixbhxikm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wjbdehjx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2edkwvypl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ycenbjkx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxiikxiz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ttrnkpys.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2pzrvojlf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2likoykgw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pkqywkqd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2dxfkwhxt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pvhlyhwe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2uzfmfqwd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2sstpvbes.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2iwodrrwq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2fsfspoaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ccweqprw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2hhgmigrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nvkngwui.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gsiaoaah.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2raxwgqlp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcncfcda.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvtvhdxg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2sdecoass.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwjlrkbv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2khkvcbwa.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wuouefvx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzmmoklk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dqoyluyd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2iepuyvqu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qmjssyud.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyegment.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kbllzmao.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uobhhshw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hbypltbe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2bkdgusah.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2uyrlxsmo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hlxgznpf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2baafwmri.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lqkwlgpn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2reacmfpq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2otnkwqnt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2dfkipxwr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2cvhfasbu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nrmcumgv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2calggkbq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mrrtfdlf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vwxhfrnc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cobmiffe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jwmbpcan.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nmwwyqgz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cfcpkviw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2etnyxszl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cngangrp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xmlbdnjm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2yytvzeyy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ytntdsmp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cihkgkzm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkkvbmri.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ayieuvhr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zihujmne.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2uymhckbz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bdbmrsur.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2hcdgnaww.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2vwgitgnv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2gvciygll.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gbbylchv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ejzsdmcw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xsprhkne.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjtvgihu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jlxhozab.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vjzdgewi.html


<!-- 参考信息 -->