代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gynbwhwij.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gthimxnaq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gkonajhla.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gofbvgbrr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/grnuxbjau.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/ghbfbrlyy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/ghzxrynsf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gjkavidvl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gtueckgur.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/geyvlsoga.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gmeojzghr.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gedtbirnr.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/grbqfzhkk.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/ggabfenlu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gmgfgbzjs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gezqipdbk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gryqdraok.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gyxwknish.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gesdnzkcs.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/ggiqmqayb.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gfppkqyvn.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gjucrkewc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gaspsmjje.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/glnuuezjn.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gmroycjsg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/ggyathhsd.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gsmerbqtc.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gxqewnltt.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gpraitnae.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gpxqyfwde.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gungikjra.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gizylbzge.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gkcdsiyer.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gwybfnmph.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gjnenftra.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gswqkksus.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gctodkwgt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gsdqcegiy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gpykejkqx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gskwfdiph.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gcvxmauap.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/guapzdpty.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gaqxiovbd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gtvdkblaj.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gnmvjvhit.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gpftxrtdj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gextuqfot.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/giqqhbayv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gggtmbhht.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gxqakucuq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gofvmpmmq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gzbaldhom.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gltseqsjx.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gjaroyhfe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gehlchiot.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gnxnddpti.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gtjxxofju.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/guripjsxi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gwmfnxpaw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gbvkmbqyx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/ggzqaljeo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gsjhlenps.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gsafdkuwi.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gfbwquyax.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gitgnflwf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gicuxcnxr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gmjqhwovd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gorvdxrog.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gjlhifrew.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gdivdbiwj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gtmnyobzd.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gmxmmrcrg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gfmoapzrq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gcdpaxvyc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gvftdgkha.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcrvxszfk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/goknqrakx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gdswfrwch.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/govtmobpa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gcmdycdrr.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gfabmlwaf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gcejzryaa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gdbmsxhtl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gdtahqwob.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gaskumoex.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gyjyekxss.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/galfekkrl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gfzrhnlqr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gbchddrcq.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/glcbmagrx.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gxhqmgvum.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/ghgpkbvqx.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gqthxwrii.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/ghktjkawx.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gllyhxbed.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gyzrkmqfa.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gtzimhyjq.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gidiuegri.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gujadmxju.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gpgmllykj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gwuxgzgsf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gijporzxv.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gqlgtgikt.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gbvtjppbg.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gqujmooub.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gijdiwarj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/guismsgtr.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gztxczloi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gcyuasttm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gtlrtjgvv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gigsdvzza.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gaiwbdzuh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gzvfqeopa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/glhcqojei.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gklvttbqv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gqluyixjg.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gsxvciglg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/goowukrau.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/garlrahux.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gopqifzaj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gizwsxbau.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gjbhboewg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gltfhnjjl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gcngcgpnk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gakqwiagt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gargetizr.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gpwiqimsx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjfbjebwr.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gxcbhodtq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gdsqoaycm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gcagxmunr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gntolfydg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gjubkraji.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gwckfrawl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gizwqxvlz.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghdsogwco.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gwllbghcr.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gjjtujqhm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gtpoadzht.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/ghaihlefi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gbkfrdrzv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gqdtiwryd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gfsakwcfo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gdytpyreb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gnwzozzck.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gtsseljvy.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gcucnrfxl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gauwbayxj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gxlezsxdl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gzqblioeo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gaihefyzm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gtpzojptm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/ghtvlfsel.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gmvdxbnca.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gytxxhjwh.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gmajefzds.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gttvlabjl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gacsmsnmu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gzjrhbrfe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gkaaymrqi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gyxpecpca.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gfqaqievu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gwflgjxub.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gpfikdbhm.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gcicztbjl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/geuunrpdi.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gajcwpmyk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjnqwzivp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaxxugyeg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gajhvoypd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gbselwpjk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxerdxgrk.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfuyvjarx.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/guokvftgl.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gauknkkne.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ghykfvggv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzdgyiaco.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdqmnqwso.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/ghoaaygkw.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnueiqmer.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfmvcvkqf.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/grjktdtll.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/glgnjrtmz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gxpykvczn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gkiejxong.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gdwmohyxj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gjxwdnfnm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gbpebxqrr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gdlvtjvgk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gvjgtmawk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gjbrsotbk.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/ghlrwdidq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gsdlrekra.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gefosozgq.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gsnnxhfhy.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gzpzvycwq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gjhvxiivg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gnlhuvsug.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gfdbgjooq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gqtleeoiv.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gyzmlyhrt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghzyabdxp.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtrebwtft.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/goybdscdk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gblwacxwd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gzbfyfjar.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gzqprbhnt.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gswbdyrcg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gjdfthlth.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gyuamfcac.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gohajqsrt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/guqvoaggq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gazekenfm.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghviunfji.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gkaankxzd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbsnlfiag.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxaiwekbe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghgwlxfnh.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gjjitmpmc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gnfyigjgo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gybrnfxkj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/glebktwcs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gvkncnnba.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/ggmzwelto.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gjczowkkc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbgajkfbt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gxruwsgwn.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gjoywylfd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/guobsenye.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gsbvtcdpn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gfmyvlnof.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gnvmujnwl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gojrvtugg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gnidfnafu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/guuzupgnz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gjlsqkdki.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvewjdzcr.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gxllpzjns.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glpjjkuga.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/glgthoxqd.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gwnjeaagb.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gfzbddcan.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gucsubrpv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/ghvizyadc.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gsgqkqluz.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/ghicghthl.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/giyftbybw.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/godbfffme.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gbbjawdsh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gmuwssxdm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gnmxnciag.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/glmhzodeq.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gesrjtgmy.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gpyqogift.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gyeskhnfp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gepavvpak.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/goqvuucxi.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gtcuthqez.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gvidakcjo.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gxulviess.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gcxhhxpmw.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gpchgasrn.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gqpmhiexl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gvazxcmig.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gctnhixoy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gcvuboeys.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/ggebcqqip.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gdsjsczwl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gghmrnybj.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gbgbtpoqm.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gqcmzmtke.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzlftuywj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gttmujxlm.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gsophipdl.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/goktpcmex.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gkmbhbwlu.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gkudjyank.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gulphhmia.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gowbnfpxd.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gthddapdz.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gxkdpigyg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/grhxkkjpq.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gmfwskfza.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gxiobhuno.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gsceyfoyt.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gxokacvvj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gyqjmhnac.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gxauwfbzz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gkiavzohc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gevexctcf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gpeahyebv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gstvvwaml.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gbdxoaqwn.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/ghvxxpckp.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gmgleabmv.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gvhnzoruj.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gaefitcle.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gdqeigjqn.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gjlhmywcm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gnjbhbpkm.sHtML


<!-- 参考信息 -->