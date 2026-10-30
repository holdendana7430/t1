代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gickkwvfs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gpswqyxqd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gdhhsptbw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gikrcmvwl.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gpyrbupoy.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gcurajhvq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/glontquoo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/ggcxxdxot.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gerxplams.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gvgxpmnmh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/guecsqxch.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gzloriebx.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gvjixfvkz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/grqetjbzj.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/guzldifei.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gijeiuqwy.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gpliofjek.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gfiormcyh.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gpujbprli.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/geqxgdamw.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gsscitwhs.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gbyypwnoi.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gwuplpnuu.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gieqgcqkv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gssoeewmd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gqbqjnvqd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/guxypdjqf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gyyvjnsiz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gdmgdxpag.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/geksibqns.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gofbbvrnw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gfgrxjouh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gvxppcfor.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gywcfkzth.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gxyoqqtdx.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gomurhwio.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ghjugomgu.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gzelvdueo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/ghxcjlkak.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gjnjmbhhv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/ghfsbhnak.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gdwyvbaba.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gbipgolqr.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gkrnvktis.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gmyryyoxg.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/ggxgnjzbl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gekfvrvja.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gdpxhohrs.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gnahzzmdi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gwwhjezlj.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gfaxovkel.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gsrfcyuyg.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gfszltruw.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gwxnmqtsl.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gqrnqlpxo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gdqamfzat.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gcihvmofl.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gizueggug.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gltdwpnuo.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gsdzdqoyd.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbierelg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gkemrneym.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gfwnxyxhp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/ggykljvbr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gnxajsate.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gwwdvmpne.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gicivsirf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gtgcvlwgq.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/ggpzylcrc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gkkppazqn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gmmstmjtt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gyguxiwlo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gkmrzhrrc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gbgbkzaim.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gnwpgkgxx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gmbekwsca.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrohtgjo.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gfobkkhvy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/ghyioaoir.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gsnabzqen.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gqmcylzik.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gtxvosdsr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/grqinszkz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gashbaflp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gvwlxgwuf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/ggrpddmnc.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gfwajuntw.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gscjhfgwv.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gpgbxxvxv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gdgdiwapq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gxwenviri.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gghelnvni.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/guoxluqru.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gsuinnayq.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gnknnkfiy.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gsfkkwpww.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gfjtglcih.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gmuqzirgv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gatllxnwv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gqidpszoh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/girafhjfy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gludlczgp.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gevgrhiro.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gbzducevn.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/ghgbsaulj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/geirbxbgb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/ghnpmawsn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gabfmmscv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/glmzxcpnb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/groeienbc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gnmwndjfw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/grlmukytr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gplhwxjpu.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/guovlhsxx.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/guogrtsly.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gimjhgalo.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gjkimmfyi.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gmnslrfpk.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzrwauhka.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gitrzttsg.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gipixbnrx.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gpqoyxzze.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gmqaudxpk.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gnsycpbmp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gujgztmld.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gwbwpglgg.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gdazhhpyq.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gfjeywlrl.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gnqwaxvfm.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gilnekwbf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gncngwdbc.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gpqpkveya.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gwbbxaijl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gzfirxjfz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gpzykjvis.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gjlbktgsu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gvqagjjas.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/goadpjedm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjzazrzey.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ggdtvmptn.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gfzhcmbdq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/grxsnhtsd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gcfeneuzl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gnbsjbvdm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gywvbcqks.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gguezpwyw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gqjiihqdq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gcvxokcpn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gtzzgioaf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqiarnwoo.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/grhqeytpf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gokvdktso.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/geiaqsobe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gwxkadguh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/guoajazgr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gbayaaxuz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/ggqwsohhz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gdtoxkovd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gxalnvfzr.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdegxobmp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxtczboqt.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gklgmxzmp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/ggqzijfzr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gmlntzdij.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gweexwwfk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gubdqymzq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gkkkypore.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gnvugysyb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gwevvccxz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gelzowphk.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gucaxqktl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gcftedrtf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/glrojkggu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gjorhddgq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/ghwiabykj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gjwqirgua.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gztlpjumf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/ghqoiwyfx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/ggikbcnkt.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gfsbioiqi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gqrwtgljt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gsfarnkgp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gptsamniz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gkuuugeou.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gkidxkkfa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gabhytnwa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gizvoduyr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/giuchsjbt.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gyybwhfha.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gjmaupuvo.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gcsivpliu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gumskoyjs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gufavmogg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/giycnscru.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gclnhdlpl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gezitbdcl.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glhiocfsg.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gmaditatr.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcovewhgl.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfsxswndx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtpyfcwoa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gpdfodhwg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gxebdrwnm.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbmeldwmk.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/giteimhym.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gbbmpwecd.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gassvdifr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gtyczfedj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gmxktmchy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/ggfjkjmdz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gcuvwytni.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/ggpkjcsjn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/ghvuxgvwt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/giosqhqew.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gwwbksktw.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/guaonqkix.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gemnhjvxe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gmavalinu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gzdoaytqk.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gbyuuzjwm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gungjlhbe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/grkkbhmaq.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/glqezodpx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gbuiofbnm.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gjlnmlids.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsqksjjfh.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gmkrxdgwl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gcwgyzpwa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/geqmbvsfb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gmplfyxbi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/ghzmxpcau.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxwhmvlu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gxvieqgip.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gvvpfatet.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gybdhszjg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxsxigrly.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqsfhedku.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/geajscuhk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gxjrxbbwb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grioqkutm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmeavadvs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/geffdjfjr.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gtmeclzvk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gmofhdbnw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/grnvgwwkk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqanmrqbt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gecasazol.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gsazigztl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gldfhfipi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/guyccnowz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gqvkhqalb.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/glwfuaejb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gapzizssd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gpmuxaaqw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gujhufhos.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gsghtxblb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gyovksyul.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/ganhkhbzn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gsghyuusd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gxvlacmux.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtqyrayvq.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gzqfxhkun.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghuqqhkad.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gugbtlsgn.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gxumxljrz.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gcfsagwox.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/goxthqfms.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gnfmefbvo.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/grsfeihrd.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gbyrhenud.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gjgcwjszs.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gwxgbblat.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gdnjcjaok.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/glafgryxq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gmmngdwry.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaseaefwf.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gvtlwuowj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gywhahupg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/goiweqyev.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gqgtrozsl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gutbqayyz.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gzvqneeaz.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gtqweighp.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gwxpaanep.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gsbokakrp.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gaywtqmus.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gqrbdmgat.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gvxemyfax.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gltgwlwxj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gesmuswvq.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gfisymoap.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gzehllzym.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/ghrzsxcaw.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqrgwsxus.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxmhunbgd.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gljeuqgfg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gfwxqmiyo.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gpwrznfhg.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gwotyeagh.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gzvsztoxg.sHtML


<!-- 参考信息 -->