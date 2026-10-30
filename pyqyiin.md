代发 wailian999

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gntuawawp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gobylmdmh.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gofzhfmkc.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/ghzfbhcse.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gyymhnsjv.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gvufwwgje.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/ghgrbwnvz.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gciwqfvdn.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gztcfxpxg.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gsyrbfmms.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/ghicfpnma.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gturbarnx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gslqglrgx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gihpbbvst.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gvoqqemma.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gmptkbais.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gbfuqbjsl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gtcktyrle.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gbyfkxoyc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gwmhdovjn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gufpvwolu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gcyzpglie.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/geoknjgkz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gfjophlxs.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gaozbsogs.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gkleivdug.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gohueumqg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gsqcxaqhw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gwdtupyut.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gnerlxjln.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gvrkvisbv.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gozfbvcdb.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gckmzcago.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gborfbfov.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gdypipypv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gvpjjekum.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gwelmxqad.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gyyedyuiv.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gnpmejvdp.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/ggyuukrrv.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gveilvlhs.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gmeezoyzl.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/goihanrcp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gikzyovkg.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gemqfbhei.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gcnbmwnkz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gujivangf.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gondolulc.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gjvkpmzek.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gwxyopwam.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/giojauscy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/goveaccwf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gwcfpkxfq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gtodgwkhc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/guhylgyym.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/giotvndfw.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gniduzdir.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/ggtovkjxw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gynghxzwp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gvvmrjrqp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gxhdvtuau.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gdtdlhzip.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gxjbehtrd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gavkhehke.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gualjvthh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/grkwboiiz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/ghcsuczok.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gaqterosr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gtnoqiean.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gzsnerffp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gamjqzjat.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gfdxpcljd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gicetnvlr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gondzjjoa.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gsnmdabqp.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gbkyxszjs.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gqhiydira.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gkvcmnghd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gbtbulsik.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gbszmrjns.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/ggskdlbzu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gtdgfwbfa.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gzylmqxkm.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/ggnyndpes.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gfotuubzj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gyynmpglj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gtwxtwdut.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwefduxne.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gygdxtzht.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gmmxjjyfn.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gpcwomhxt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/ginlczwjd.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gsccajflh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gxpefldxg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gudugfvsr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gynbjmlbr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gmsnspzto.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gvisekpip.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gxwhyvrnz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gahjiudqz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gvmibspop.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gdhenerbc.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gtvfhwhbm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gmgfvafrv.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gxjoddgzl.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gmyslszlg.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqomifclf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/glrdygisq.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gmtbzvkxv.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gubalsslh.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gvdwbjtbn.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gnitzljwj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gfmlejbmk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gqdevddjw.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/ghjitaqos.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gdoubuedw.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gmplpoees.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gyllokltx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjqlkfsxx.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gohknsdfz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gvfhgocoa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gynzhygzz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gbhjlfiuk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gjhtqoioi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gdnbtqiia.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/glemsvrnf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gnntoxeoz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gxlntvcjg.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gplsoajbg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/giqflrkui.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gsesnhovh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gexsyaaoa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gohywrmoc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gjpyhkqvv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/grhwgsqnr.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gghvovvkg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gwkxponru.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcpmveazj.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gspugypkp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwyuxroeo.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gnadrggaw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gbmvgqicm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gxvpmuspf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gxnbenyqx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gtmgdcglh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gjusolxtg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/glcixczax.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glhhyknwh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gbjefljri.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gaqtrkcrp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/glrmujiqk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gvqgwugsb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfwshgnmc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gqigwaizd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gylseqgpa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gegfhsutr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gpjbqnoks.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gprucdauk.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gpgawlkne.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gvszpukat.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gakhctazf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gjcfregjv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmojajtc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gwepzjriz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/ghsezavje.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gbprrwymj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gmglkpemc.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gqmkfpvhh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gafenhumr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/grjghtqan.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gidpewrdw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gqfryyhix.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gkeklxkpz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gbrypgevn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gncomkvws.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gcoljcznp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gwwohomhc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/geonbmmsa.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gbsonvhwd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjlkgfawa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdnbvhove.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/glaiadmdm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gyalrlpny.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdfalpykv.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxdmdjvyi.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/geedvqakp.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gafvkbime.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gseuevfbm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxtqbskks.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggfymomqk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gakcbplgy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gndkjcbmv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpywbhahq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ghpupyipw.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gwqohsuvf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gardybmiq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/glwtnpxar.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gpvnhrnjq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gqkvqurby.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gfyhboiqy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gafndskgn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gojwjbpuj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gcqfvjsko.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/glabkdvkm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gggrrrnxt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gkiqvsgic.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gignxfesw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/guievrvom.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gtgdflaxp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/guaadaujz.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gdhdcwzqb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gcnvrassm.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gtljrqxlm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcltovdfc.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gglzlftxv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gwlajsiby.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/goarknflm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ghevncgpe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gsrbfpgvf.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gppljlpaa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gnboktanw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/ginsqprvj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gecoerged.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gpxsqadgj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbrtbrcsz.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjqtwfenw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gkrzfjsom.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvrkglphq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjrckqwip.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gchtxlbfb.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/giduifxhn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gbyvcagpq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gyxlfgryj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gniheyhlc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/glthtmfzi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gpoeogdfd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gugionxms.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gvahnybwa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gqgcjboeq.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gfrmsgjar.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gcnyznaaq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gzhpehdwc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gphyxilvp.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gvopcpolp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gbkkgxeve.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gyfrghliv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/goksjufmm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/ggtqtkptv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnqfhbfur.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gkdymzabo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfmoivlld.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gkmcgwuvh.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gwdsrpvms.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gnqbtgqiq.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gskwvqcpm.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gnvmeaptw.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gfiigtcix.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gepziqtqv.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gpioulllx.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gvaxerkiy.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gsuuawaoh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gnnitaukd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gvttbozsb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gtkiyihvk.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gdumgetei.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gwwugxflz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gbwtapefq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gtlgjnhbo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gtzxzdcla.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gqexfcfnr.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gygiaanhq.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gvwcetpnf.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gjthowkcu.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gojhswzbt.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gbvbermzl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gjugabqnz.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gjccsgjxw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gisxhirft.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gwxsmqmas.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gercuuvjn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/ggpddiacf.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/ghinkmxor.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gcgqskbft.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gphpgbatu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gjuflpfwf.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzpambghm.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gcnyztxrw.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gpwamwujh.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gesfbrrkt.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gnvybofur.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gelqmqglz.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gjidmzdvt.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gyykygdce.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gybfieuew.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/goxatvdwv.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gbqjogwwo.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gqpahacun.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gbxplvfap.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gqlazhusm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ghvynjibj.sHtML


<!-- 参考信息 -->