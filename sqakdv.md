代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mapxfmdw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3yzrdshdn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3etkwnkhp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jigrgmhm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3tacvpauy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hflldyve.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zshiegiu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mfafhvsq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hticxgvz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xlejtloz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nrkvvjcs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lmdpdyxb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kqxdmvei.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3zytrebrj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3znvqoyhj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3icaeabtv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3linnefpy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ynyzihws.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3wihsupjw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gannesqg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3tjrlrrqq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3nczbcfjl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3lythohuj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3insjdnyp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3flxsvqyq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3chfuznzy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nntpnqxc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ygtzqtsa.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qnwspwyf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ealprwpv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3azzaspof.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vitgseit.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zpwlcnru.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vzsggcit.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3afaybezj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jcgyvxvk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3oncfxbjc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3benmvjex.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3yhqhgwss.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hzyfwxvo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3vttymreh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jipkftcu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ubhqwezo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tksqzjmw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qgdlvikq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dgyaysgf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qldlmjne.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mrjxyecl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3tqiwthoi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dthqoujw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gwecjkpn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3prutshez.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yqozxnqd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3aitoxqbn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qwoumknn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3aetivajx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lagkowbu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zsvanzdx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3exnitblo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3chvlaxgo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3yrookbab.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dfosnbpe.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gzwpqwex.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3uraklqup.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3pikqxhvd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rpsrsigd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3fdwsztnp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3tsjnzmvt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pghopzzp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3zlbfcxan.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgqrzwey.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hgamaiij.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3visxxclg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3aecxgzgc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fsaitnno.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltonrnoa.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3mgklxoav.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3znfoyaay.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ocktwynw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3gxucrjdo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whcsimtf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zguhudof.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3pnbnqwfb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3lbwffckh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ulbhnnvm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3fppttuvg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3hsqycgnk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ikytyvgn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3wlrgdkim.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3blektjvl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3masajmoc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3eoqvqvxi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3teejhqhn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3wghgtoxh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xsehbocz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3htlnwvpv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ufzlcmml.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ywjgelsz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ubhmdxih.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nklwxuuo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3pbabztpa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ypfneqbb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3edhanovb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ciiixkhu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ogrqchwq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3gnwppcqh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tqeramvi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nrbexbfj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3aenecing.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nqcnlniw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fncmhutz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3vgbdwaya.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3anoyjolo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3bjdhxosb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3lxqcgmau.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ilheyobn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dpbpigan.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3urstaomk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bevmeccm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wzgovkhb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wwcfxhpj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3veoarres.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3gpntsijl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zykpiwfm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3aivxxhug.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lwetwncp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aikscixk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lcuwwlxh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3kqokiepi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ilopmegw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3odewfewp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3igsupvow.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3aoksaqgn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxndzrxn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3juffxbfh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaadoflj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmljfpvl.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3xkjvzqmh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3lcicuxrz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ninszjqf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3xzbzfukk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iunykhwq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tzhzmwwj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wvmhaeiy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ktpjxsva.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3qvzyhqdb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bmpghmpp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dgwbcabe.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3esqhzhzk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3xcktyidh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3smzwgmao.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sqjrzsnx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fpdqurss.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rxxschxk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tioxhlme.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ykrgxdjf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jpbptxak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhpzjsus.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3rosdcyxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvbwfvxt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oemomcso.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3kfjtweio.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iysmxabo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3vyjaqmbd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3avkyhrbx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zwktffge.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3pipwhhvb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zncjixql.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gipedice.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3fkjzufhm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3tpvydwxy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbogaksk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jbkomtig.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxpqclts.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kocfezyu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3kmrtcpxj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3eobwivlu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lcwftgjm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xwfcsyxa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ngxvkguz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3whwquozd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3utbsabpw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3onrxpfcs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3anvrsmsu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3tiorzajb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3imavxblh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zejbeyno.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ywhiqjrc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uhaqqynn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zyoxfxfy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3oscsvujr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sfbitdbf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3eslljasj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qnytzaju.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3qlzvzpbl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qxaviuff.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3vemewfmt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3zwpjavsu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rkktpimd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjxqhntw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mihesknd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3omfngixa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ealimsjm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fxsuonor.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqnkbcvx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ttdwdxzr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nuswxdsi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yubmlurc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jtrjepvs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvdexpqb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bmqwqdzp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vrcmhtky.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oocteyhz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rnnccnds.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3dsubmynh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jxjbigmo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wjhjjnzk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dywdpjbq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vyemsjux.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3maezfbxb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3wkbsabwc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3egpcupab.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3txtwctpk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3crinfmon.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qkoovdfd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3szdguorx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cbtjzics.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pddfbkid.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hmncxoay.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3frmukqtl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3fqzxemqf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3imclbbqm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vvrigzpy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gjfvrkrl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qeieezun.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nuuuxllp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wyvprtck.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xnckbmdk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3lkfizqcb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cajetkop.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3oedwjked.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3lqcvwjdi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aklbfeqp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xmhewttt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fwhttvtq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxgaavww.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3etbpasah.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hqwkiign.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rajypbdv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3thvrufie.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3uvfnblhr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ayhsswjf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ztvygetb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ebxfdaku.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgezezdb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3spljdgrh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3mgbhkzhg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eafzgupj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3qnyoybxf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3jsjqsfrw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qufauxek.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3yzycvwmb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3fqeagqsg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3agenvwxc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rtpahyqc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3tqgovlaz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3rqnsulqt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3dvrouolb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdjbvria.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3prbpbvgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckiqgcen.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bbszujqa.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ufmubxkp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3gkxrymwr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qkfrqrhr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3psznxxzz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3knpulmuz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3qvgiqsml.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hswvibwh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mbwikgrd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mevzkjum.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3kvxrzqwe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wpdyvpvi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbrfhwyn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3pzqtulku.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rvtlmrwq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3homlxwtp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jzdcukma.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykwstvwv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3txwbyaad.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3biyllmpt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lkfjpuwz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3djlhadcd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3yzhayufo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ylhqgqng.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3qiknmier.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ntrwwswf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xopijkjy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3tondtwck.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xmdqysdb.html


<!-- 参考信息 -->