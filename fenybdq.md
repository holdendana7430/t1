代发 wailian999

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gdibnqdng.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gdapnwuoo.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/ggqakbpvm.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gfjuvnvro.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gfsvkrtyb.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/geoosakim.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gkxutesaa.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gfdwaybil.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gicjizwgi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gsytqtred.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gzwrkgzlo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/ggsjrgzpe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/grsooauxw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/glgzvthgf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gfclnyohr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gqmjumfsb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gwzasdori.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gvrhnmmil.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gxaeaahhn.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gyuswghzf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gnrugaqwq.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gngsbvbky.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/geoxjbqea.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gqmpnrcwx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/ggkplabnq.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gzgnyntom.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gsykpytnv.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gmbgyauup.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gqlndrkjk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtpjsdtlr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gnhldnliy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gemhckrnz.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/ghnhcqeez.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/goklokukx.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gnidmcpae.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gtotlxwoc.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gjfoitdff.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gtialiqee.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/ghizexlzj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gaeodbdgp.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gevgmiwhy.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gklultizi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gbvcsokmd.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gmgwzdxhu.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gpaahfzrc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gcbijojop.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gsleyfgcu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/guhgdpbpi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gdxdfxwzp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gwdpnaiza.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gswkutahc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gwtqhyxqq.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gowzknlqe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gjctthycu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/giivwabvm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gvjbantxg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gifqcxtyg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/giekffqti.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gagcaxufi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gxoyyqygz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gjanfztse.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gctamzmst.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/giyjwvwhf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gymqjwmxu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gcupsacyb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gxpevdgrx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gvbeplozh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/govuwibjz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gtqssxfmg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gtauwznrw.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gnnigwqga.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/ggnalyfez.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gjgruvczt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gxbhdffoo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gdyyfpbub.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/geylztvxy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gmedhgirz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gknawrczi.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gbrcboyfq.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/girilognh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gpsdpdzwa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gkozlclub.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gakkqffkm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/goqkxvgjf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gflounepg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gmtepvpln.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gfrmyvxsu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gparlxknt.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gtyagnspl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gpuxuqysg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gssfmoygc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/ghdgsiavm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gpjgzukpf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gnlixqhrs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gcbtxxcyt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gbswuibrn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gntnmcgah.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gdkcisrys.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gygdgeulv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gljiobrtr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gglijxpcg.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/goblplsmg.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gqatltufl.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gjvpqszbc.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gshllcjbo.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gucyerveb.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gkssfhopc.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gbnnziyjz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/guwqzbcne.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/ghmckzltw.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gnwjwqihy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gbsgdlfhb.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gmvaoaeyi.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gxcbdxcxc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gsyyebtqz.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gckeygrfb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gdhbgcwzn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gtfjddrue.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gxlrjboqz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/ggnxungqm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gsqnmcpxd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gnedbwnty.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/guyhwbvtc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gjmdqnsuc.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gzeunvvbb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gtakfdzef.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gbsnfbobi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggkxccaja.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gybttjgqc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gmsmfzepa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gnaviruhg.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/glzlitkag.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gdbkmcugk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gehvbmjye.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gjienhrdx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glbqxowvd.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/glfopjdhf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/grmpfsetr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gswnaeegh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gfarloyvo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gmorfqugn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gckxkbhmf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gxidygfts.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzaxaksij.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gartvxmoc.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gxpaqhmwq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gvgvcpgsv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gdwxcfdoy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gfewtmyci.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/ggxjtbnzy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/ghaimxlhr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gpendjlee.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gtpvlrqzl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gpedulnqo.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gczfpnurc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gkdtxzpic.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gjiufyrph.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gkeqlaurb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gvdqdexhn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gswafpjpf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwhakrpq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gmgihlgqj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/ggsrkehwx.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/ggtcpyinw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gioatiuxm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gnckfcgen.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gpefwivkp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gcmfaahaw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/guoxtbfow.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gjmsrkmmp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gunnvyxik.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gygddbdlb.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gcmofqlzu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gmeuwhbwh.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/glaxanxel.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gphdqwcwt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwcpsrzwb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ggwtsxeip.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gclzsucwx.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzzycjrrp.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gaoidunhl.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gowkqgzst.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gedahqjgt.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gafbqrljp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdoiljgsx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmjmsxnhs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gohujxmhn.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbkdubmtd.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqlrbulyr.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqwyqcayt.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gdffbvqea.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gktpoxbgh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gbcbbzumy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gunbvcmha.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gyujggkor.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gbrbzjvmi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gelqjmsrx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gniegbgyy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gtpzjvagj.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/ggthlhfbd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gbwinsbtt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/ghndjphgi.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gohqckdhd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gucynkrsi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gpwcjajkx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/geqxftska.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gyvdmbqzb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gvjsmvdno.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gqktnkrpz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjictjjru.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzwcebavf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gplvmkwzf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gjqajjerd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gwwpzwkdu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gcjkwocra.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gorwkteec.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gfzugplkq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gmwaltfcy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gvgneweko.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzxfobrxv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guumauqji.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gncujaare.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gpplpilge.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzmlzwida.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ghbucpcyo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/geciywikv.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/grbisouiz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/ggumslfff.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gqedmlzbk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gchikogji.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gvvbuvclj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gqxbxpugy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gxdcamstb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsejujmbv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gcywgvprb.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/glzwjzvaf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gpkturrky.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gxkunywth.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gtsjtrkjx.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gjqwqcjhv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gllmpwitj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gerukvefu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gpfazgjsy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/goapagusc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggitunxzn.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/ggbzkhjhy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghdbmcmit.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gctpkqryg.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gdjjnzxxp.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/ggvxdifva.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/ggxlxqkbb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/glstomvnt.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gyoglfvhb.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/ghdycqwhf.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/giesvyesd.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gazlnymld.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gzfywbmon.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gdimnhxqe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gavcljuyh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gfmsqoefy.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gkfenmqjy.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gixthskqw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gwiaawuyf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gziiraejd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gzupdvwyh.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gbmjahgad.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/guswkcgcy.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/ghfwodrin.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gkvgambuk.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gvrjgdvgx.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gulitvcif.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gzkiaklut.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gucichzay.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gpodppvqc.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/ggdnvmrxq.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gthlgllhk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gllgfidtg.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gnmobxrfy.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gxqjqmplm.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/glsejvbht.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/goqqhpeqb.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gzenyvgxg.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gjrjlunhh.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gtzuuaepw.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gifvghvxg.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gcywmyeov.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxonhocvx.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gbyvuuzpa.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/getkzpoqj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gvqmvzzse.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/guwqydahd.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/ghwswtvag.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gdonijrbb.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gopwemboc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gsmquxzau.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gxgliarhp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gysnhbpqd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gmogfrrfo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gffbidsuc.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gpdjskdzw.sHtML


<!-- 参考信息 -->