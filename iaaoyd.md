代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3xkidlblv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ustwymee.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3gatabwwj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vrratplv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hvbwhszq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rhklzqmw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ekkrujmq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wtxvtupk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3lkkxdnwm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3blxgnukm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yfhkmyhs.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ceoqoiyc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3jxotmnjh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3thqgkwab.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ucydspry.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3yzundsci.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3calvcyfq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3qbehoyuc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3sgyiatja.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qrcqbpfj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pltgmhzv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3aeumsyjj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3txrjmhjz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nvgrlktx.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wcidccfn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3onhueloy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ujxjrypq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xtywnbmv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pjmuhbkn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xqdrxewx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vlrlwkyn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fdxexucs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3cwunntqc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qvhctibi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3sbxzmyuk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ntiuyyba.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3adapyvfj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vjtmxvkq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3wfidfend.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ksgyffsy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ghgnfkje.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rdnqqpnd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ttxfpgtu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xeotpfql.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dqpxeazi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3opxtgakg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xwqtwcrh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3pvcyeckz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3sjpzmspl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nzkjsbov.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3aelcunod.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ipsiovsf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3nsqdhgxv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hztcfbek.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sdwnmzed.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sojdrlnx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmnlezfz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zvwinfxe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3heodsghx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3coboiytk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gdysdelp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vqrpdhde.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3smjwltqs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ecvxnety.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ozytwqbt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vcitcdky.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3uotmtdsd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3nebbsdwk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bylwqrei.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rgxbwdkv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tjtjpycc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3txpqetnw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ybfbfuqr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ytktkdiw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3carngqrd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sidzswhv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nlikghac.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zcrmswvw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dawnkcmh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mfkledrw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3hohuksod.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tqisqlzk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pmfbethc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ldjmdxwj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3wkwadpmy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vtownycw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ycgsawpu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3pfnrnhzq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ubbyfsie.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3rqkyculm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ecugscze.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3whjhcplw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3veemsmzi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3umokserc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hvtefupd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3qlcgwelk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3xztdozhu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3fodklenl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ncsgidwh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zwlnxuwe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3draupykz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jepyypza.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yfcvcpvg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zxfpwiry.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lgagysti.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3evipavao.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3djmhlslx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xqzflvjq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hhviaswp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jojkqyft.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3sqpagryi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vxvvcjhg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3coxgwmij.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dmrqijvu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3bvvexbha.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3vkkwcqnn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ksznrzza.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3vninvpfp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqzdzbcn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkemaarb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3jthdkhcq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3wwajlrpy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dcqvcqqb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3geklitsw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3odwfcrgr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qdbbufxr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mejorbxz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cwucihaj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3azadyutw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ifykmwbp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dnxmgecp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uujsfztt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ogclcpjv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3cukiwxaf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jswtdadk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3egkmqxbc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bouyaqwu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mlgcmsxm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3shvzontw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3svopcsvr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xiacodof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbdtexen.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3mafychtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lltcyyvp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dvaubspt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3wscruohh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lhzpspau.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ouqyetyg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cfbqybim.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fdotifit.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3hkuaxasm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3poefeeic.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mierffop.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3lbeaynbh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3kpvvsjjy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqrurzla.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kieeezuz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnsaloob.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lhmcdhiq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3rqhgoaba.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3gyzicvgs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3znanmbjt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3mlmyowiy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3oerkpfpz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ornmvvcx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ndkkvtdb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kxmpkloa.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3jvkvesni.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3bvxqpxxd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vzfawqfr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yzmorveq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3crirlqac.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3omfrapns.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ifwkqqkn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lqmeahzz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jqkrmxzd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3okvylqka.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wdtghljb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3sjtqmkrr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ckoxttsj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3wvuucvvb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3hrttslyr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nfulrxbr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eslhtqge.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdgugqsf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3phsenhhg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3vwimiadx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kqiqcqvc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fixxqtwi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3jitgyiyg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uyxyfrrq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bemjabjj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wptzjpnp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qjdfwnvh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jkhvovqu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zntfewax.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wgwjhloi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jhkseews.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3pvskzcui.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pdutrzgx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nsurdlxy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3spheepgu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gyvsedts.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3bvpujvde.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mwtjyjwe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3stzmdair.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ryodlbtz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3pcnggvzj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3nrkcarok.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3talullqz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wyzuueuc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jhqaxoqw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rucysesg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3chbfnnem.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uqbnzkwt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nmdepaiv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3hepbxddu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3byzwripy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iwvpukkt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3exajfsmb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dkuvbwfg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lzphaghk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3zrjppiyf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3whbdkbfc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3zmvzarxw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ksstomkl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3syrvpgye.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kknfqfur.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lfepbolx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ocxzwkgr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mecxgtrv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pbibppru.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oelquidl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqsxtcru.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3nmaiyjns.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kcwvamhi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wtrzmtug.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjnocgpy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bigigboh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3usnowahg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3iwzqhqbd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3agzzaoio.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3asvtdydk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xjqrkdzf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ihvrmbsf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3dkkeczyz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ugjkdkso.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3njpwmwlq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ryjvdfaz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qzaswihi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jcabxnuc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zcvteihx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ethghsmy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3tapxfpxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zuujqpud.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3sfzqpale.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xfyqcxza.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydjnpxzr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xwngzqlw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfifbkuv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewucxydn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3kgyvlibm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3probottz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3orcmekxb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ogkqnwuc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zdqmvfvw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbquanbj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wzougzql.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkcafjwk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vluidkfn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3savrbylv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3knbedglf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzzwfhiy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3gkfdbuds.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tkkprlnl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ulogizmf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wvetlxjt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gnhjcjdg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3gatrrwrb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xhpgxplt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vqkeagvc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hhdcofqb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3aukbmepe.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3eyoaugup.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3naexodmf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhvttsfx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ucykjswf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wohpxtoa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vocteglp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3sedivazz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qqddiosu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ouaaeiok.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gwmiclcu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3annrbfmb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqawhuzq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmuikpya.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dsyzltwy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3rdmmxrgq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3msohitrb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcfbctah.html


<!-- 参考信息 -->