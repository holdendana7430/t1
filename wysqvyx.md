代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gozbhjimz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/getkxvdie.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gnnzuvdoc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gdnjtimoo.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/grkxeuyzv.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/ghkevjjdi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/ggnpnzfps.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkbnhczmp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/glkjvehcy.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gcvyiducq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/glafjevww.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gcbnwkohk.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/giedhwaob.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gjkvcpsry.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gktsnqszf.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gdhlictyr.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gxzbpswuh.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gglqqnfex.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gydjgvqfk.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/guyertwqj.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gihnwlxxd.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gsgfsuxjv.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gfpfwdsws.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/geigtvzir.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/giuydiwgg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gccybppai.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/ggspyesce.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/garypsurl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/ghxtvcpsz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gtsvhnxdf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gksgvslnf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gfqjmxjal.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gjwexnhcw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gjbuiydcn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gejqfizst.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gpknickhi.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gwbumzuqx.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gsjxxlxgj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/grxchzdiu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/ggbbdmvur.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gdefjiper.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gnwaamknh.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gfhrnmnui.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/girecopck.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gnzqefrne.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gmciihjif.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/guxpyysye.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gopqdsbbx.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gzghbyqkj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gcbxrmquv.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/ghlqsryno.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gixviqfpq.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gfwgalfok.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gcefnamnw.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gfwuqcloi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gqlcwidsc.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gejamkzsw.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gufmsfbjc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/geppjhhnz.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gxhnrzmje.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gxtsyplwp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gfwkhxamz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gqnbahubh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gokeptyql.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gugdxgnti.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gdwkyuiph.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gjnbsdlyi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gbwiavxcv.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/ggsbdjosg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gqnrdpalo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gkhmkidzu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gkieelrhs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkxuglctx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gtisvmhaq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gecgtpujo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gkkjiwmto.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gubirqsst.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gbqhkbmhq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gddkggvnc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/ggliilddn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gnvssvqoe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gocrtjgsv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gvbsmopcz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gxjaodbxo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gfyfvlgpb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/ggxkxkpkj.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gbsftanus.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gbrdfawqb.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gyylkojpk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gvgacrtnk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gscwwzixs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/ggrjvxpbt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gkucsctao.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gehnceyzi.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/guoocdhtm.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gonqgwikm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gwvilcqdw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/ghdnhxnoo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gstwwvzrk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gpjqlebfm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gssrpmmjg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gyffcdakb.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gvcazwdru.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gdlauantw.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gmzwqqyfs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gxlqvmvyy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/grtqjclcj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gxpcdmcei.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gojoflaeu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/ggdvvjjri.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/ggnvnjjtl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gclzttylw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gqmpzfbah.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gxwdvuhma.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gqkyphvhm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gvfqxeddc.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gomweqxjy.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/ghihedpnz.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gganmviat.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gnpmwtksm.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gzasairny.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gbmbmvjqb.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gyfmalwjb.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gxpnnzick.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/govibnsri.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gmopeofca.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gtfdkqmgw.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gurmfjvhr.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gvgwzefbv.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/ggbifojwm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gggoomvws.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/giadubtcd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/guftqgxih.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gbquirqds.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/glxuiwkno.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/grfsuarok.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gkpcbbklw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gfkvzidur.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gbirlpglf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gedvkwpdj.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gwotxcudu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gmgxmvrzl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gllnrtevh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gzzgsjaxj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/ghtfjejfe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/guarxeisv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gflkansxg.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gsuxynjre.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gueefixnz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfjrymrnj.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gxkwmread.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghqhkxcyz.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gmazhoujs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gmoyrdusl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gcaoapskl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gfnchnsxp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/ghzkbiuic.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ggqvkjmbv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/ghqdenvok.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxrurmqhq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gnbuzhinb.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gxoazygyo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gapmgkued.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gfafomsik.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gctvdiqlr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gewhxlvbj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/ghnsjsvbe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/geaoavxwq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/ghmupneku.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/glfqeelwd.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gkalwxyvk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gvxmnisfv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gyqvnoskx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/goncxmtui.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gvytvwfne.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/ghjkyrtqp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gopanunnj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gtfgmjwwn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gimvynkcq.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/geiqndgkj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gfxpgriym.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gljwhozlp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gryvviwiw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gzyvhawob.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/glmbrlgft.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gnkxybleg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gxfemgfbi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/guerdytoq.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gwxvyomjn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gwmjdixdr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gefwoohef.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gckifjuum.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvctrgnsj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gqrojqfav.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gldtczkmc.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gitsiokhe.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gogrirlpi.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gmocvbutf.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gugztmrcl.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gffpamyku.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsbjpvhll.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtzyzvlib.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/ggqhkoaaa.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gawdeytiy.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkedkezsp.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gssuuktdl.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gwqrpepfc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/guxbciqat.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/ggmqiwojk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gymibnxne.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gvokhlzcp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gjjxfrmik.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/glgliuqsm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/guxxarmlw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/geqngxcqn.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gtmimwkxl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/guabspfhi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gvnicpchy.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gwjckztry.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gzaoiyoyd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gnsxmhuun.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/galyqelss.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gbdutcome.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gqneualug.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gwrdouajy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/guqcsjetc.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/ghaikfpzj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gkgokemjj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gbgobpkia.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gftlxmagc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gibwvdyjj.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gkwahgsrl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gghsknvfs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gubfaauwt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwdnrrirg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/grhvbakka.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gbgyyiswo.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gyropdruj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gikrlzdoa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtxspajpm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gslrzcwmp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbuftlksv.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gqdjkedcl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gclimwfzt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/ghgnjvfob.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjzclmlbv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gdtbruilr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gmifykqzf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gdovjtgvo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghebinvya.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gcflitixh.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gzvkxlsai.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/grzzaxllc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gkhjlmwlz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gyjvcdsnk.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gynnrsstq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gtqelyqjd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/grvvldmtb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gmmyyplpy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gmruezkii.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gllvyzldr.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/ggxxfactx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goijdfgiu.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gfsrfgydg.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gghiieouu.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/guqtvniba.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/glxuyljwf.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/ghfbgrvys.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/ghqcyzpkw.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gtbizxpyd.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gtmkmwhqe.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmkdtfyde.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gwgfcyluf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gwvujnjqc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwsanpexj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gqpqmoxoj.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gecasvylu.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gwxfqixth.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/giwkgrqbr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/grglorvhm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gzibwctcb.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gctxdizqm.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gpwbmeqif.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/guakvxiwd.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gbtbdpzgp.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/grbqxlkxf.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gyjcmulsi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gcgqcnhzb.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/ghhhgnbfs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gghbrmqov.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gwmukfcxv.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gbbkydwvp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gizqpswpg.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gwptnydkp.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/genyiwsxk.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gvbznabmj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gdzftubpu.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbuxvavcu.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gqoxqifpe.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gnhrhvjiu.sHtML


<!-- 参考信息 -->