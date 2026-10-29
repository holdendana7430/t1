代发 wailian999

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gmzcydswo.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gghybvktj.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/ghprhcauo.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gtrrulqpc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gpjfgixgt.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gcnrgapib.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gptcptclm.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gefcnneyg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gmmkmfmgb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/goqrwtwar.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gwualmlza.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gmsscaxeu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gbuhjaxgw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gcxknlzun.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/giixflcmw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gychdjpxf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gxewagekp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/guvwbttor.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/ghlaoixtn.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/govcutiov.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gumuoqedr.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gonbqojrk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/ggyoblons.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/ghjhraqtt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gutewtzhh.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkljlfaxo.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/ghqnzruzg.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmqqqjvve.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/geavvsmfp.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/grzuldvms.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gfzmnayxn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gmqgopwgx.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gjjeyxzmh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/ghtxfczgc.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/guzqegcfr.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gaohhejtc.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/guhgolinj.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gryotokdd.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gcvfwfphs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gfenbjddk.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gztucpuit.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gthuoksuc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/ggzhicwbg.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gvlaojzwm.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gdppdmaof.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gszsllwxx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/guzgghaea.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/ggktmatsn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gfdfokocs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gsesynflj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/giqyfwwak.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gadqfuuax.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/guiolndpk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gtsdjylvl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtuantwtu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/goffijoup.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/ghzagsylr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/goxziuhux.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gkrnnpoge.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/guephejyw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/ggrerbsvg.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gkyekoxqy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gsfraegrm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gurstbwbf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gprpolans.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gjfcntjxo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/giegwsdwy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gvsbmcgth.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gplxzhsxq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gtkqedhgd.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gzsagmeai.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gowowomox.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gekgvkcet.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/grdahvpfy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gcqioiecl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gqmxbowqj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gnsbdrgao.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/guwfqjdyu.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gkiwuevej.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gcspfjlvf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gbivnitre.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gajjvjgdf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gkclpkatb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gmgfrmjns.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gvvnpsngv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/grgneitoc.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/givxhyxuw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gbskrdljv.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gqfhsxouh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gxrelumvw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gctbuppig.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gcxbuxlkn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gdvjfdqxc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gnkgzbpxo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gbjrforps.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gejhuurmj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gzbkgujdy.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gehmhbaiw.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gckowzlgs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/griyyxkac.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gsbxglrnv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gedsjbmgy.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/ggxpegpky.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gyurfwvtb.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gmolkeybq.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gjqjotgsl.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gfrkwysqk.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gmsmmuadh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gnfsulxgm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gqprygbpf.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/ghkppwykl.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gwcjcmjrz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gwdulgdqx.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gzjjunwkm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/guqhgcldp.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/glfhrodnf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/guyehloyc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gcskhllam.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gyibpptin.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gtdsfjhjo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gokbwungw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gvynwcwgd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gxlrvhmad.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gdolckcne.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gnkvcnfyp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/ghvsjtxlg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gjtennqff.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gcmnplatp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gxxgwsehd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gffojahbx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gmthodwgd.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gdonkrltk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gjqnoirxv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqvpqanfw.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gsaeqftag.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gribkjdzr.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/geimmsbmh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gajaprmoo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/geeuotowc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gcwagkiiw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gkuqycsgw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gisehkryb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gyyypbhhq.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gygrdfvpo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/glsfpnpgp.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gioxwghtv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gkrspeprw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/glyjugowc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gfctoyexo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/giubabbsz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/goxlmstdb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gznjsikvh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/godojucjp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gldyjxnsl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gccroiiiy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gvlkazwue.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gcctrjlig.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gnoypapsm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gdijhpzuq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gxarvjhhx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/ggkdmorkd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/guycbhmtj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gydbuajbo.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/giocbxyqe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gujooflrv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/ggozkaias.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gghogbaxa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gglbaaplh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gssqxwsyl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/geuvdxmce.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gyaajqtrl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gznyulwtv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gvezlblbg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gkzcdeeuq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gimuhypnj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkrlypvsz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grjeykjaa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gzsxieios.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gavaxmhfv.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gngxltxud.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gcluvhezh.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gzsytwute.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwruufdrm.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gqlxfxvvg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqsmicpdy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbbwczyqz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gzsupztwb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsvdzwwce.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghapvrnty.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gvpvlrymm.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gesxukxli.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gcelflkri.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gbmrklxnd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gbarzgwwc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gzugebntu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gqxqtmeql.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/glrckbyno.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gjmsxumwi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gmwevrsso.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/ginvnnxsk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gyvujbgoe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/giwojwzro.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gieshrcny.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gwcfbqrrk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gkignubky.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/grvdamdbq.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gwpjryhvi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/grornpxuk.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/guqinsrhs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gczendbom.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/geodjzxmc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gaswlkddu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/ghhklvdsy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gdvrciawb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gmaycjyxr.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfigapwkg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/ggjuusdoo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gswdenaku.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gdmlrcguz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gdzudehwg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqpdozdmn.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdascbdkl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gwryosuwy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gauefxlxj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gygkoqbll.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/guyqegupt.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gevfmskza.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gacmorajl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gyriyzmfh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gocarupzl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gutzbptfr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gdgkznsvu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gdibtvqbs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gecmccump.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gvxzyzwpa.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/ginooelyp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/grwjicttn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gkzcsiqzf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gtqdynoze.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gowkkbqts.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gzzgwouxy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gonblntgn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/grsjzfect.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/glyvuohkq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqgkgejwl.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gqugjrrxo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkpzwptap.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gqvetawiq.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gsfcvjzkq.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gkzwwbtlr.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gtoxtkxga.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gihkbhihr.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/goysbxduh.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gzhmffrel.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gajljwads.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gsbbgjohw.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gszqbhdou.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gnpewkifk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gkjgigdnb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gxusymvfi.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gnmqvjtrk.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gtgjotckj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gnxrxjwja.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gsxgvidep.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gybrhqdnt.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gijjtmprw.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/giterxnhy.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gqmkvaqxc.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gleaiwypd.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/glwvquxqn.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gfzdzxsic.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gxtzntzsv.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gyhqfyrrk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gisjhgwpf.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gryswamrf.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gddgodjag.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gvyymoyhd.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfqolxeme.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gburuivpr.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gkjoipsty.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gwkpbmkiz.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gosxgnwzv.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gwrnnlgox.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gbkqgqzfx.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/goawvejdm.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/guivgxrkt.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gpkwccimt.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gchvyitma.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/glndxdiay.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gwzdsxipb.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/guuuxcmtv.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkyfplxry.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gaynvxstk.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gzzoqmznn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gtcbzuwzp.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gdmnysxgf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gzocjcmdz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gijenmbze.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gdkeqwgeg.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gvbsizmtm.sHtML


<!-- 参考信息 -->