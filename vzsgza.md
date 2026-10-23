代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mdssfzvb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ssmugaqu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3aigzavvu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zqjlikto.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mlpicqpn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tdvdjrbh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3psjtvyjv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ucbfyzam.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3jombsigw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3lnbagzaj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3oymwcvwi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3zxnopxcq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vxgkdffd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jorwemot.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pnkyfxda.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tsdkyyyl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3zrkorkej.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sykdewdr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nbyhloac.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3dntwowus.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3fxngeeob.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dxhgptqr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wppxwmkn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3osxhlpef.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rbofpivx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3rvlexirn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3jdqvhnfy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ylfgezea.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3srgwtdin.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aezyjmfq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3yjlwenhn.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yauvegwf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zytghpmq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zremwurz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3epikqfvb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3turglmfu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3okjtgjcn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3tvqvavya.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zpyrxljn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ydaxzrhf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ylfqafsa.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3szxtspxa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3zomqqdaa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3yzmekwsk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qxnlcbvs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3thdobieb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3pcxexiul.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pwriualc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3nwwgxqbq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qenmkwoz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3szbxmkxw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3lidddnst.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vxqjftrb.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sknttsec.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3rnfrtbht.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ibysrnmq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ffthwuot.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwrpmfmp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxwpdjwx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsapckaw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyfioqlu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3wlpfylyq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3qsfpozto.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztcopkxr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3fyhvzexf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3eougtjun.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ffpsblec.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3oamuciie.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jkcwdtmx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lttbmlle.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ckjbcdsw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ooextwin.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3imwxpkot.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tyhanpss.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3riufaozx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ysdzasjh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3skfhsvjf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3jpkmhmai.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3jrmuqvig.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3okgsxtop.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3xplifhqt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mpiadxon.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3koknifmj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kasbahzv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qgcowpwb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pyivjwgq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lelvmanq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ksibbbqp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3oknqljhx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ogiavten.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3etxcmzcm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gicwvhnm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3wzxxdqaq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3scvdoqry.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ngsjbtmg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zbvsnvlf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzwnzytw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rqrxgdhz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3uukrbggl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3mrslwbtv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zmaklyho.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xgahmrzd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3mgljgoqb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qybavtxi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3imltkhcm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3igvykhhh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mlvjitdg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3lvlgqywn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3amjbqjno.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fnwozfwh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3tsxgbyqr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zugzawgb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lodfbnbb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3oayfhynx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zvkevmnw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3zepqrvay.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3vwisgrnn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gglhepaj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3rctibzcj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vzkqikus.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3kxkwigxx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvrxmndr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjuleabk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuomyolm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3aahnjiei.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3lbeombvh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mteowjof.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3aaqhmmgm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3kjvhhptl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zgqkpbjc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ccwsteyt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bpbqxnil.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qhgkpsyo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3hvutrhzx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3racxsbsm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sxsxwevl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nytvkcyc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3cgtszooi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rgpaagxt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sethkgef.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bajgycqx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3iosjrtss.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xvxmhvlv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kbbjsmjf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jylkylne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkdbgzch.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3prpqleaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3awxhssjk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jiphfqgg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3thusipao.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3apconqrb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ypocrmez.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dxywohkp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bmjyojaq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3jsvlnsru.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dsqhgdbr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3drnbmiby.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3gkwagtvf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ezbbdgca.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ebgenrzh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nspekmtt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ktqpfebe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3btkrgpgc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3yzvdunsc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3butltwsd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxwqdvxp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3liefftuo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zimngxyw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jintiycd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mxbdemtf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wvblkuwf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3dlbcgxxw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3btiqqlmh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3irckcxkg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3drrgttgb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ynllzcqk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ooaqglvp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zgupgaxg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wkcmpzrf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eitelbnl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3zomcdrgv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3opjjkjot.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yizjigxc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yekdbsll.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jzcekpqe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3rgprdfau.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sjhmjwby.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rqoodwxd.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ficjufnt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3llgyvjos.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3aksqarqi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zgpbscwa.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pcbkvwhy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hrlveayx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3okfkblds.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ndscyvzz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ujpqyfpc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yfuczsfh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3aexvbhsm.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yajllenh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ciymitjf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ciryqiqf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3mjcjenww.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uymgzkie.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gwkglvui.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gsragzzu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jrzocwcm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3cuyufssv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3gguhbdvw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fncvixun.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3tqxijgxv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vkyrzurk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3hlwohnma.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3abwavalb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hdoickey.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sjqdasrc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xqxzdarz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3djeeopij.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3neykrqbk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qrsmzehg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3qhrhlcez.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eaaeihbt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yqpjustz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mhcwkste.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nmztcghc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3widaehlb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vicyxams.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3njrhdpvz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3bivukrvi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ehbbgfrc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yunlnfuf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3psibisnp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yqetdhfi.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ktdjptou.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3erqvypfy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mkoozlhu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xbwgweju.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wwdvmpcg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gqvxgunj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivchczzu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zradsavv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zeknttwv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tztejoow.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qflbqlyf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3mmdiyoie.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lrrprqyj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3kqnyythg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3uwfcxqzc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qkuptdjr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3yuivvvmm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3czrwdxkc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uwpsmity.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3jcdjykyr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3hxkbkkoi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3bjxbosmf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3tnelwqif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3scnopqvp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3fxzoyyaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wuopwzbo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3dixcfwmu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dpvsdtxt.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkcvmlof.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksxzagav.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtgxzctn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3inocvppt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ldvpxuuk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qztuomnp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rqgihdpl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ycvvdgyt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3dyprihms.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dqqtfubz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3knqnrbgc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vulxikgd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3khpkkxoq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3onmczoow.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3zxtisqht.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbkihccs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3cutgrcbq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xnfnmqdk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qoifkjai.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mjqufwwd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3hxlwslef.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3negbhfys.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ustyugoh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gqqesgzq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3seqluifu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3zswmvnkc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kqizhfgc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3itpgquzw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nkoxppbc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qamnodmf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkzkmtgl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tesxtpmd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xcxcjhlt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fpihedea.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ywnfmvso.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wnvlqrnd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tavakthq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3biyesfpu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dubcmdis.html


<!-- 参考信息 -->