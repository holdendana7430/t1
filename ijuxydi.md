代发 wailian999

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gxznjqvhu.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/genjgxqzn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/geniswups.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gcdxygvcy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gdwrvhtyd.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gmhgnifnp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gszedprns.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/goosebvai.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gfygyrhjp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gzggdxmoq.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/guhgsenid.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gzfhwhawd.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/ggwqqgfqj.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gmzzugbtv.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gmilrzywm.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gzgbmatws.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gzlmzyxkz.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/ghkbjesyj.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/ggazvypyp.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gohpwfkvj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gzirvwbdc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gnuxveudi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gqqddhbpy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gkwvyeydd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/grwbuorvr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gqyerhicy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gahcnfeat.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gfmgbyawg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gncmqkwdu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gxgvugwwm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gjcikfkfr.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gbtrvdtjz.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/grjjomekk.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gihlabldg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/grxcokpnr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gqasvgjdd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gxniwndvl.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gngckolpk.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gkyyawoxa.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/giygmxwzr.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/grwudbkqn.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gkcvdmbvm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/guqkuzuzq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gnsemnane.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gcyfqmgfk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gcfjucufy.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gldjmavtc.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gbqitlwci.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gvlvysjek.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gftqkjzwk.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzrhsxcal.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gdpmgnnby.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gazfkwkix.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/giuffurqa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/geerkkvlr.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gzldgdsof.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gdisluryu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gnctjjlns.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gsuizylre.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gjqdxfawn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gplvgmvpn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gtqsutjwm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gtmrdfvfh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gbnpvjltm.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gnlycsoqz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gwsvivzoe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/ghmqcjdwn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gqsgqirpv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/guxurmzsa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/ggjnquezf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gaifzshfq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gnkrjqjit.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gqwasnzwo.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gjatyqjpp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gjrdhntxn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gvjgnzjpy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gfwymtymb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/ggwydrfry.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gooqaqrhc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gdfeqipcp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/geppchxjk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gkehsppkq.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gqcahxqnm.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/ghxmtfltc.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/ggiudblgx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gfxmxfyai.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gboledhhs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gqezpkxbg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/ghlowzqlp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gnpejmtgd.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gikemxwfe.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gehlethxh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/goyyvckhq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gxtfvxakp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/giuqotyee.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gukmtgvdf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/ghedfobrb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gnnrbswra.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/grgadsqoj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gekhiqzua.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gewpxjkng.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gmcyoioqk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gdnrxmyrz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gvhszbwko.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/grspdjxjg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gpvecstcb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/grdkrvmjs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gcfvrobtt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gkfghitwc.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gdbhrutcl.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gulrrpady.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gfajzxxra.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gbsgpabzi.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gyoxncenx.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gpmcdimym.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gjbujjfgb.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gcfpwkkrp.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/grdtgcify.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/galygrxey.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gzfntuehu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gprlugpdr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/guwackzss.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gsgirpsxn.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gtpyeysve.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gdovcqofi.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gczquzaqa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/guqskujem.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gwfjvjcdr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gdyqozzns.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gggmwmmes.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ggsjywbqh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gupmbhhpb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gkzkcsnor.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gehkhagol.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjrkidnfz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gyqkftxia.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gwwlgqrbc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gsrpbqamu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gjhoimrdh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gszefasqz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gumreoyti.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/groftfzvr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gwxlfdjac.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gbqpreghm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gzcyxduao.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjesyxcbe.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/ghpzsdvzg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gockbilul.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/giodtnjoa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gtzzotgvh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ggzgpwohe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gmxjejhgm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gzonnlshr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gkadstmyr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gbliwosfm.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gekcgqmce.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ghwgiagvq.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gzqziisgr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/ggbgoamab.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/govlkylis.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gdjapfspb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gzhxmcucu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gjtvguiqj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gsujbvsjh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gmxsbdbla.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gcdqvftuc.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gjafljtjv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gjkrwvnsu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gzfxdllwf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gcqbixzoa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gjwkcwwlf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gqupqdtdn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gionhsosc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gcjezyrqg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/grfsugukj.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/getvyxgxh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/geyxxyztr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/ghwmunzqo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gwsnfrhap.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/ghyxxthtz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/ggoblhnrp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gnxtdkjwh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gctyescak.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gbzvouvoc.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gsnrbwbgk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gnkwxdjyr.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjeibldkk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/giszirwym.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giimoximf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gzqrellog.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gmrlfngfc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdcazymxf.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdbkuzxxg.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/ggdylpqoj.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gursairob.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gaytexrdz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gervpjtwp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggcbdtlll.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gzonylegb.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxlthanej.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfwkvgcln.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ghkaaahcq.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/ghcjsziov.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gwgaaqwcw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gkssakxgt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gnypdiatf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gblmjpend.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/guwpqyqjs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gtjtxweee.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gdkcmjgpm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gfbdlsqfe.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gsmxtygop.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gcquqgaqp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gsuotcadw.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gckwnnxnd.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gipehyfdb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gztwegmlo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gnkgyokdp.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gupizmbjz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gbinswbbm.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gfsqqtilu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjmtxfljn.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gouqszugf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gpnjaebvn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gdlbkqynx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gorwgvrup.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/grwzjkvvk.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/guhwlzkgj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gegekwrqe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gshowzqap.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtsqvhokt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gindpuzyl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtccrpsir.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcxcerzrf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gtiwxmfrw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gxqhvhldo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjhdenwnv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdbbcrxmf.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gtdlsggqg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/grilaphwp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/glmhcykdx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gcmhcgeim.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gpfycunfp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/grfwhdlcy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gmbshdyhn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gltelnwhr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gdlsjddbq.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/glytjooci.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gethgpvky.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gvqfkdbsf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gnffxcrdy.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/glympnqft.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gxxzswbhc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/ghonnjimc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gywjzuthm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gatdxztbo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gprwuvmkq.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gwhmxggct.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwxqxifnn.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gqennonfg.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gqjyjeesf.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/guxusjqwo.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gobkffukq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gpkybtorw.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gbdmkirqw.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gsioxnusr.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gbvgfcohi.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gumpyzvmz.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gkwdbequk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gbgnhzdbb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/giwdokomx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gbkekoseq.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gwaauwfjh.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gkjxthubz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gcxaeydvc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/givigcael.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gdvksjdcy.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gawyosdsz.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gphfuotoi.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gcttncueo.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gwagnvqfp.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gacndcvzi.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gnesuhkof.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gdgycojvn.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gnmifxmsp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gobwuvrie.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gwqfbpxmk.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gcgdcmchh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gbhsuoysj.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gakfqfazf.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gutbdwbcu.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gwprlvhuh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gcwzphpta.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/glfhbqjeq.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/ggszmglbn.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gpegorhaa.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gqsrzbpri.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gzgrlkzjb.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gwarbugkp.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gzouhszfy.sHtML


<!-- 参考信息 -->