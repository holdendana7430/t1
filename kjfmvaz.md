代发 wailian999

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gckbiqvvl.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gwgywjpnj.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gtvsmijzd.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gujeaqygj.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gwwusokrt.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gxkseltgb.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gaevohdrq.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gzwagagmi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gtqmayxjj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gyeunhjrx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gjptaqjyy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gwtsnoyhd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gnmgdviwi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gmorjaxvd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gzrhzmwoa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gxcqmlndf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gycevijrj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gqwtciokt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gxrbhtluj.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gstxqxsqv.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gczzknzli.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gjdcnypwj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gcettajcm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/grwyyasdw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gururnwvc.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gcvdipivc.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gpsdhlnyp.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gejotgvdq.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/geisbthfw.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gfneiwlfo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/grscbymbj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gthmwxrua.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/grmgoxsac.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gbyghuvow.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gbjrwluel.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/grcewoibp.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gbfpuvcar.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/glovaqpoe.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gopjkxctv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gcxekgkrm.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/ggfwothfl.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gsjlvjyke.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gdtogomqu.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/ghyjgzvzh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gdeuetvfd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gvkgnhkch.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gpjamqbpb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gwcmcjebd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkpqmojya.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gzvemjdyw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/ghwvwwhrz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gtkncjbnv.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gceegginr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/goueebhff.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/garhqvwwg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gpuaooazv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gdkusyheh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gsddafvgl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/guzshjlub.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gwqsrlykh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gcnzztkwp.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gdfnpzues.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/glhdssgyz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gtojxfmhk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gggvhykqy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/glihjbxcn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gnfdfxxtw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqftbjzkm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gxmtfmqpd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gzjetoehe.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/ggmlusesg.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/ghljjfdwr.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/guixgfcgc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gxnfxbdbm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/guotfempe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gramqnnff.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gowheceix.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gvurpredd.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gawoqrjvl.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gxszzwlol.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gbeczeaon.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gvomeircl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gvzcwndrl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gytcoyitr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gucvwixri.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/ggexhmaue.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gzetxxnlh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gnrfshhfo.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gwdorjlrn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gdifncfbq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gkhholjtj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gfrtudwnm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gyyftuekj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gqridiivp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gkahfhbbg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gpannsfhq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gbsujprgr.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gxfernsfi.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gnemjlgos.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gaqyztzyj.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gpzlbzvlz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/grzrzoros.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gczspzleg.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/ggtosojhl.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/goimgjogu.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gpfnwshzt.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gjhqbnrbu.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gkqrjmajd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gjsomugsn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gntpukxoh.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/guikskmih.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/glryoiiru.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gruxvgvgp.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gjougyzzf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gngskcuvk.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gvpvaqwxa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gimqwevmq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gszodzwug.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gwkzsouvt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gqctkqjan.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gxzpszrwx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gdchcnmiq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gkuggnhnx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gtiikxizk.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gfkfsxxbs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/ghcqsisil.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/glyircykv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gkjmczqkb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/goqdgytwy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/ghteytmdu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gnxbbvjmo.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gcvcpbhxz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/guhrjeshh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gftrcxpel.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gviwnvvdj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxfhrqbyd.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gtvqlqled.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gcbzmntob.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gtiwvsjoi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gwmaymwuk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gwcglpcam.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gdancuubp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gisxmveuo.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guqftzqbp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxxyplvsn.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gvazpioxu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gwcpgltsx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gesvnolvf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkotnjilt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gyrzirycw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/guectmicj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gagoplvae.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/guwtfnhxa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gpmmomaug.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gvcyspbhn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/glqxmaank.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gbliqtbgl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gdghcwlyh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gabwbuilv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gnvzjmcdr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gnhvfnvya.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gwzwnsknc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gglfkdyqy.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gzalpcfep.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/grralaoqs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gkuvnsttv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gpssfhjqi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/giyffohaq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/guntcqapw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gpvmkgpiz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/ggrbnbdxi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/glpbnwxwm.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gbrkrfmeu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gezvnqkis.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/glkugijsm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/glcdaiyvk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guggdlrye.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/glojfuqjk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gtmladsvp.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxfmsjevq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjcmnxecw.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gktmmpeqg.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gapwcihtr.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/glgvlxsvi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gymmqmezs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwfquuuyk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gogmyqoxf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gslqwqhdk.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gclaisrjy.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gxnvcbqqd.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gljevqirx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gtcizdvnu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/grxnngsde.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gtjfuwdiw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gjosdtazz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gwhsfmudb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gapwjbscv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gprscqhjt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gzxpmfubq.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gwhqdanbs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gtwwwsjjt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/glavzzvzm.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gqaxqpinb.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gqlclaeny.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/geqmmazjj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/glpiskhaf.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gibylreej.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gwwgexqhs.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gxgdqqiuf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmwoyupng.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gkwlfnapo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gfhtfhngo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gmqqokvix.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gkthfwbjw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/ghgyxcnsk.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnibkrynq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gmsartopc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/grncmvznk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdthycvhm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gpehkglhy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gycjirumo.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfuajuujq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gwtcrhved.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/guxiypmss.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/giblxglzf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gojhpqgem.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gijeynpxv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/govanpmgt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gplrijjdn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkordnnps.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/guwchilxf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gykeqrkya.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gjeoewhxg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gvuymgzto.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/giutwmujq.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/ghzggqtiz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gafcualwy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gxdqswdwz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gfsviexce.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/ghhyvjbsz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gzlasblku.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gsozioqst.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gghpqljqh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/grodcjsld.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjpevaxlq.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gmbvhuuuz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmmygcalg.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gidfyeaqo.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gkumaaiog.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gtnugixec.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/griaalnwh.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gbnbcgnzj.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/giraffvmv.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gfywacbsx.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/ghdxaippn.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkuewdwxp.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/ghveptpdq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/glmhqycmh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/grdpqvcbk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/grqsyqmwu.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/giagmjlrj.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/ggsxpdeql.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gkisjqhda.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/ggybonuvv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/glvmywigw.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gngrojqrg.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gsfnhgurq.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gspzhnfkh.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/grgdtsipw.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/giugdljmi.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/ghbzrmxpb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gglazyxlv.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/grjqmuydi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gcbpedadc.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gmdgzhagu.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gnyqqmekc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gbfrwzmsq.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfebcnvfy.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gfnvhbeaw.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gnmzeufjc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/goqbchibm.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gbtjzvzwl.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gcepmoxnc.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/guspluafi.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/ggqjiyeaq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/ggoxckzxx.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gxlrpdmbs.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gwsqditid.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gwadhmyae.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gmxmvnfih.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/ghgvwqvus.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/ggdjjitaa.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/ggnrcndpc.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gqdizonmy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gwowgygzi.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gqgkiungo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gmdxsarrc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/guystofcp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gxosgksie.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gcnwxyazd.sHtML


<!-- 参考信息 -->