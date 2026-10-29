代发 wailian999

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gxvxhpmqz.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gxulemxwg.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gbymxoepp.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gjldrprur.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gxbxkkqsg.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/ghzqyfbjz.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gxalrhekq.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gxcqpsbtq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gjkqnoigs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gjrcrdurz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gppbzjese.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gjibyahyr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gfofrutjt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gpaojfxax.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/grkiphqkt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gwvfvyzhi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/glgxrgoaw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gznpfqrfm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/ghzeosuwm.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/ganhwbcga.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gqpkzucip.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gnnqvraoo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/grezdylfh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gcvyvawzr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gwwepsbhy.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gaovvwkhl.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gjxtrlylr.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gjxxnjdct.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gpgghavib.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/ghzlnfdww.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gfgjoevgi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gwhowzjse.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gsuamxlsw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gxzlnwqrd.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/ggdsyerwl.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gidophpxa.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/grinnvovx.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gljlqwhys.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gkzhmkniw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/guropodzp.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gggnsbyzu.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gktpwnpjv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gmushwqap.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gdisolofm.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gewxiicqi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gqrleuili.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gvgducnwk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/glgzfozld.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gajgxltht.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/guuisqdjr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gizpskmuc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gveqotzto.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gmbpamvvx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gggnxqtrq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gpkxwqldy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gudwitcgl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gzjipvfaz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gzvgkrmnd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gzytjeiqs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gltqdclzb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gaoancysl.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gjqjqvqba.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gaajgaotu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gjyleghpt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gfexftauh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gdaswfudh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gfncajttb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gmkroumiu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gqkbrrosi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/golcfvvtr.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gkukqngmh.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gjjasjrcj.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gzqvomoms.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gdqtaefmp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/grjzybyzw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/ggbildxym.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gpgidktoi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/ginruasly.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gwdqchctq.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gfqlwvdkk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gflahtuoc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gkqeyypqo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gqpspglmo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gmqcvnniy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gxqhfisot.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gboshlchd.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gcyvtufaj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gzxqdcirh.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gdfamefyz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gnhwkwmxx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gpegmtgdi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqzhvhvb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gshqrtanu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gmqvzezjj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gnfhadnkd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gmouuqfuh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gkzhlhkzl.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gmavxlmml.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gmhpalxbg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gbxpzvppf.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gqvyvedsl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/ggghywqyw.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gxixrubui.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gagzotdov.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/grmzwjcpm.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gzpnedjcj.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gggxrcooh.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gvhwmnfqb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gjaswllnz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gnnexggew.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gyjztefye.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gfltsjpto.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gtskbunab.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gkdnkudjj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gahmdqsqs.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gmvplfdjk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gipopflnh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gdfbswdmh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gfjtcocxn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gklifmdfn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gvfkswvdx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gjucsjfit.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gmhycuedc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gecczikrj.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/glzybxrqf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkmuvdzdl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gahjozjnr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gpyfivkmf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/ggqoxxmhv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gwqdfatmv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/goggubgfb.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/goczumzgb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gupkvrdaz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvlyckkai.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gzmpldgdg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmqzdygyp.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gpuanztpr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gydosgsik.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gfpsmseeo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/goobytfqp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gbgslwssj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwbgrfxcm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/getmaqaeh.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsageiesd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjwfdnlkv.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gpxubcxgf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gxakcxevw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/ggtpvfxvt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gamtoslkl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggpaddekf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/geimelscl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gdeydmjzq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gdjijesjt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gtphqcwsv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gofhohyqz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gnbmjklqc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gtkbggisu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gnwwzsdou.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gmajdysbg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gcvmwfpkt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gryffdbwz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gfllxxohs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gjstujucy.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/ggadfvced.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gmowwlbhb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gpfqggzsh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gcrrwwjam.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gsiigxkgs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gwigzglow.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gkbvhworf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gajwzwiew.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gyevolqus.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gvjnnyscm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gctdwjrcl.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gjmbtlogj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtotgtjut.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkpkhwuzm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/giarxjsma.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/garfqaxgo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnjnivygn.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdwecyzvu.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/goihwtxzy.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjzgcwtsl.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjjpkusju.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzlvfxxwx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbadkdejm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/groydlynq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwbbzfwgt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guyrskzln.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gripgdfwz.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gpjskmaye.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/ghssbrwvh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gakoofgip.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gapzwlwwv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gxuykoyco.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gwrnfhvse.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/ghnpsllbd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gdxptxgup.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/geclryuoe.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/grglgleyv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gxduwcmwr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gkjzbzlkk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gxsqcvatd.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gpgburuuv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gbyrixswz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/guwxoneyh.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gsuxmpgvs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gshawfkga.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gptlekutx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gftmykuts.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gsvjkupth.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gqablxzwb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gknrtpbke.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ggpirqgak.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gywqeckpx.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnxuslbqz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gqaxkpotl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gaeceiwqj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwaxmqzef.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gypjsirgg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gumoikgjj.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwljxyyqs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/getgkycsy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gfrqkovpo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/glaisajbp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gerbaaprw.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/golqajjjk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ggvpzkaeu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/ggqvpztma.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gafxglitk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gnsgbnljl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/ggkydvimm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gxkjlohnd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/guokogcwr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/guerliecm.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/ggglkklwk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gfquayuyp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gdrafgzuv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/glfryhszs.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gixntregl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gcwrmierl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gmwwhqqua.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gyyjulrcw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gyszfihby.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkgvvkrta.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gccefxxzn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmojtjzcp.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/guetlpecz.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gkmutjdzg.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gpfqqncwc.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gkozrsehr.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gpdufginb.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gvuaolglw.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/ghppfsexm.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gjuhxdfcu.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gihlcukap.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gxudugben.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gxrqpyjpe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gdhugaeac.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghphkhdzm.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gfwsezsmz.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gztutbonk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gjhnylvod.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/grjjiznyn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/glctcbawh.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gybtyyrsh.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gwnkajqtz.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gwuvifwrm.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gwvdrakyn.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gexbekepy.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gveefzcsv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/ggrjvpswc.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gzlhtigcg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gxkgcpijf.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gmhvuzutd.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/ggoywvwef.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gazucuuhu.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcrnxygxl.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gqgmobzzv.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gihnrgrqk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gcamkpoyu.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gtwmadfab.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gfhbuqhis.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gctwitpdn.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gwpavijln.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gzayurrgp.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gbzllfkiq.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/grrkqbtij.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ggqxohvsd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gzfbwtpsl.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gqukjwrbj.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gnkmndiso.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gsfpsmrru.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gzryvowfm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gugjzdzmd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gegcqkfeo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/glavfkfhy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/ggpcrfzox.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gzyqwfjow.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/goqwngtzh.sHtML


<!-- 参考信息 -->