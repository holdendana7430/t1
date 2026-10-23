代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bazufctl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3guihpwdn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kkanoquu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kqtcvurp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vpwuiatr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3gadfbuvh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3rrltbmqn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3weoziocx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3azdecclt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3liishbvo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ndcwdeod.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vapreiwt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3qdyauexo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3chhlfspz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3yzbmiehr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3riwvgprd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3gkwyyuzv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3eiyqazbw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kvytfdof.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lzftmmxk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hbqzwtmg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qnllaeip.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vrkocejt.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3yyoxedtt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3omrjvyoz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zckvokgb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hdoeomzg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wdbdvmar.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3eykwjrhn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3fgylhgry.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fvluzgsn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wfvcbfmn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3elrhcmzt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kiiyhfza.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jtblefmh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hlqadand.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rljiahtr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zeaigagp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jfixzaql.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cqgpstdw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ohptyfoy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3fujsbzxj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rkhgueuw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xeklwzkx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xzebaegm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pllcwyop.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3gznqgqmc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3yvovxoee.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uvnjpvve.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3njmhxbkl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bgbnlmrs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vvxxmmjo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ylipsadp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zntmvtxc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3iziwrrcq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3mouvljgu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3kopfyziz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3umguasxf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3zxqaktxm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3srgpnyis.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3typzabvj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hyoekqjs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltzfvplm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nedhhjtq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hwwdzdzq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lkdtrnms.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3tqfzsqak.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucpmgqvt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3bjxbytnl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3elljvaka.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ckojsilm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3necdvodp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3qrrpubyk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mpcclpbc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3bsymsuic.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3smpstfjq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3blvqcjqv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xgtcpena.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3dfsxphzu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3hzgsrswi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cxrvwhoh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rthxqphi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3fjqoboto.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ulvhbafy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3atelviop.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3hqnwpexy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3tpltesya.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mesopqhk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vswhuhps.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fupgsmhf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ohulycos.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rbvjiznc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3pucsqakp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3cdqlruat.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3sybqneaa.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3tudemtde.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zbppnclk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ntadboej.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eylcukau.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cbgejtmf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3sfjuiswd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3azvjhofe.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qwddbpvw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dhqudwro.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3yhljeptd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3jwznujwt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wwxnxrkr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xcglmaso.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3omuuexsc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ickiljad.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jqewzpjy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rztegtxt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3yfdoskci.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3oczsmspx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3muevgfuf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dpczisxe.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vmxsvjly.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3giqsoref.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3txzbgvbb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kcwbrgdz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3glnmlqyj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3dbrkqqqb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3cndrlivh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ugqwtxnp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3yksflahu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3brgukblw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ysmztfdt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3clqgiclz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyfzncdx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3sghbojlc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oddzwcpi.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3qzypvoad.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3hpjwjepi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nmpyodrh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3voxbjnuj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3begvsgbr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dbylxhtk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3lmgiapxi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gncbysif.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ixmpfgyl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3mkjrgzsn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3njllzhlm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3norjbagw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kcjeidxb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jyokkavg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mvxkdkfd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tfanssls.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fuurhrkf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vzreizft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olhxrgza.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3gfizjzfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pthyazva.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nradefea.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mxypriff.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rumprmbl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ejkbqeuz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3efuoixix.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3scxvkkxt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qbkhngse.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kqvhpqce.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3edivzsov.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3omybebrw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3aerianqo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vpndqvqd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3epixsiit.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jkvagntj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nzdrkyjz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3uunjdssf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3tinwckkv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3utxicaxm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3lzpmgcfh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3oregmguq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gjjhgjta.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kmyfsgpw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3andmesit.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3wfqyxlsr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3sescmpqr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3etfstyld.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3otuutmog.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3gfawjjkr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hejqpvvv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ulvsdxrl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ehsqvkdq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fjyhtckd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jahrppej.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jhkpdgpr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3sjbluwwv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3fjuygqbe.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ptmlbbla.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hdupxxtl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wwpqenbb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iovuyuqx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hsvchksi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zdbmdzbw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3fuwwomhl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cznjiioa.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uwcucatm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdnkrkzf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ogjoxuda.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dmlibuph.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3islrhirn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ygwetltu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lvireqkd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zqxfkmfj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pbhfioxi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ordnpciy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ifvxfroz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jhiaggza.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cvlqtqrq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lxmwfukb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ckwmroyg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qsgapzwo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3uwprnmnt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zkmtaqks.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3rvmkbpwz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ivuhtlec.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3kvmolxdd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwfbzfma.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iatmpzeq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3krmogfox.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gofbrprb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3huiurbqv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vbjpnlbc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3xbkbpjnt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3jfmmdcup.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xkjienby.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vijerzli.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vqcpmqsw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3keopzyhv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3khzbpyei.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wuhensyw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yposxzmr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ilsltfdd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jzzwoikn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zdhbwyba.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vgfxzhte.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kzwantxk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yeumsowg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3bgsafkqy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkhqqxdp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwxiklkx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xpehhxbs.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3jgqdjuoi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iomeeqyt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3hzgjldqc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rlpxzjsx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gqvzjggh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3aeiolbdp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3lusgzkmv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mnwycbuz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3tnraihvw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ylcxzqcm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wocxmski.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3havzecmi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ybwehtah.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rjfmtfml.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3efyntjvk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kmlqkvim.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3kdsetuvh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ambmishn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kodwsjlo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3csidskbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wojouvhp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3gvmbdtfd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3piditnxi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gojyvjkd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ugsvuoli.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gqlilqzz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aahocinm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3lreccjln.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3uyorihyq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jltoanjb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3onfzlmdm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3libvwkrb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ldiixttb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rsajaumw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bteqjkir.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bznwlnld.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vjeuapcf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3eikuttxg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3odksjqdd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3uagovymv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3faxuvkfe.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3byykfdwj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wrcdrerx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3gmvoletc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3yybqlzhn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3jxbrgjej.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vdedewhf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wndoruaj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3gfslrbvh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3njnfafqy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvpvhanj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eakzyrjm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qyznynrz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iplkkono.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xfxmhopz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3alupimyf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ghskrcgn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3wcqepgdd.html


<!-- 参考信息 -->