代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/ghnisifvx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gkkvkxpni.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gvbhxgaaq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gumwjwehm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gkiqycmaq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/goxcxkntb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gvsapitnl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gzeayguur.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gxgmtlsbv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gybzxpdcd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/grqzskaux.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gjictmcju.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gpsacevzq.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gjkdunqgd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gzfkjjpvc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/grbsicibr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gufqwzeht.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gcaieyhpg.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gvtcokpjn.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gffenkulr.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gnyclwkqi.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gqkovhodw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gxgaaciqv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gwdrtotth.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/guqstkfyl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gqjcbxfvf.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/grvuxbezg.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gedimrzmu.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gzcopvpce.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gmjdmalfr.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/giyfzvhjp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gxttjksrw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gidfshjlp.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/ggyybmjyd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gctzcqvoz.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gddikovva.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/ghhiagfut.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gxgqkcugy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gcjdlavup.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gxapxqgud.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gkhjnqyrm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gkcfejsfr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gvohzhltj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gzxkwqwas.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gbmgooofa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gdcuhyclw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gznkwhxbz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gskhgjlri.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gloukfthv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gmdfgmxqo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gaheamnew.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/ghgsjknej.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/guthtvwdg.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/guamtofsb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gwfjftgqk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/ggfpajpea.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gbjswswxt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gcjyxbvza.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gsrvztapb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/goguilffs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gcliatlrb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/goxyeyokd.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gdzydemia.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gjwergmws.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gmwybbrpf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gygkppcos.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/glljdjsjo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/glcprqecl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gfwvqhbke.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gqdtzgbun.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/genqgqrlk.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gjzyqifoe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gdocptfqn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gngejecwe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gavmhrjac.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gqwbtsljw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gmuzchwzw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gqoxllzjj.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/guybxymxw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gbkmzixiw.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gkfwrlxon.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gzzunqbsf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gfxevjxpv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gxgbmhxvj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/glhplqrwt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gszsnjusn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/goxlwbktt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gwuiurztz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gbarkzbti.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gkhyjupfx.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gvfogmekd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gdzmvpvxu.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gveoscjwr.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gmtmcnffz.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gpmonbhkp.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/ggqvbzjtd.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gzjzojzsz.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gthtegpbr.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gjhrdgdxf.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gbsskddbf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gcazkwuwv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/grizwkkfd.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/glpikqqmp.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gqkiylond.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gkbfsbtjy.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gufplbvsu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gyfthbrhk.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gvrjpkqcr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gnyofobwz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gndqensir.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/ganbmooaa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/ghwbizleq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gyiucfpkz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gieahmikq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gcybplzrv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gcplktbgc.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gyvjdofxm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gtngnipqv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gqglebmns.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gobhypuoo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gfomcmcov.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gykymvcqw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gknrptzhb.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gmmeznmiy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/ghbybhuce.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvjoxvxyi.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gcqcmfcfv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqlaozbac.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gtaozktbx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gleaamspk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghjmbngox.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gwlqwgutv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gcwmonemg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gfxxtmwlc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gfpsfncfw.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnuresato.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggjtztade.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gbduwcccd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gnzhgfqpl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gqoxdfept.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gmdjcktjj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gyhsexjlp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/ggkqemevw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gykpetgzi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/ghlfqvhmn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/grjfsesjf.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/goxlnilyu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/grbaybmod.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gnuqmcmde.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gydsviwbg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ggkmyxymz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/glhywdboz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gzuxbeupm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gzsziynkq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gufugcwhi.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gsxnsrohh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gvlfaklqy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/glbyqygea.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gxwavgkcd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gvljohvbl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gfnxbqdxz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/grsmikakg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gwejcavvz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gsqkumgtw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gmfjyzsct.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gasihtqja.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gloptzrpq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsxmjeogu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpbkbumjr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/glxtgefxx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gwqqpebvg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsfxgajgo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gklixvzjv.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gsgdrbakp.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxthayqkx.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/grdqrvyci.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggcbbzaqc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzhayycub.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gqtwtcskw.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/grtdkhdrp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glhglvswb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/guyxqkbzb.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gpjkpoxyv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/ghhpzqeug.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gjamnsghd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gcqnitpkg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/goxexgode.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gkzhgwgga.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gzvtrhbtb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/ghkgkmpvy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gpmybikkn.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gjqyvmgnf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gagnjsgpb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gfsbzaais.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gjeswzwzh.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gvdihswdn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gbsobtfyb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/goddaobsy.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gcmnlzsiz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/glqzmzyjn.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gpkmguuoa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/goiknokbf.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gfoyfvmcc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gcupvelwf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gbiwldsay.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gjomfpmtp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/guxdhlylw.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gasfimori.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gnueyvqgq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/guikqsnjh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gufdcztqz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gdzrdxdxj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghugpocpc.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdkphlusy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gfgrfceqj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grrpicouw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gddesdvwu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gcxjyehrv.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gmpztajic.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/glzytjqwa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcaevxthk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gkhtrojsy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmuwjghuc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gugdsaewl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gkyyanmyb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmuzhhpug.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gzrsndnlz.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gkrnswxor.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gnqsexxin.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gddnmmgvp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gikerqlfi.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gbkaasija.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gbbaekrhz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gghmlxxec.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gtrlkrchr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gpqzvvthq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzogcpxez.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gacykjjev.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggxwslrww.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gvtowuzoq.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gbybzfual.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gfyjhqvtw.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gtfdjvqyo.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gqkrdvycz.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/glvxhgptx.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gkwkzpntt.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gxefmenth.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/ggfdtfucc.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gyiztdipx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gpqiejdmd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gumcvmbhb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gtnzrjjgc.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gqkxtqudi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/giadekkhe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gthaugesb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbqsuqmkt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gxcclblyz.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gfpsrbdih.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gbkkhupra.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gawtcuxgz.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gapoluowq.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/geujpklvs.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gihmydkmv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gygvmssst.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gotyhingv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gogzucyhf.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gccqtprla.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/guhsgaruu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gopihcgfg.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gfpuchrbw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtphkshcy.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gldmqqmuk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gyrrwfxfz.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/giwfnmvgy.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gowxvkqml.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gsxilqklp.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gjvyqtrvn.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gubvcufvp.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghkwffnjj.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gyhphkfdr.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gjeuafctv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/grfqpljfd.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gdyoidncu.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gvyqsmvwn.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gzuuvzoua.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/guvmhqkuj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gefusemhl.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gpejmwrnb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gthlmolnk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gkojtehds.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gplanqbyv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gtukesrsj.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gvagudceu.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gkpimjthl.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gilxtynvr.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gqnndtoqh.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gmlrskgmk.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/grqjpebcc.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gtmuofyky.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gwajqxmqq.sHtML


<!-- 参考信息 -->