代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gxpuclcrh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gfqvhjxel.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gttbptuux.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ggkqxdqds.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/glmyfgbzt.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gsyopxiny.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gqzwhgwvi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gsngmfpdp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/grexvlqcm.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gbhjtdlgm.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gxmpmwysr.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gilmfttpv.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gfeogdzms.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gwqvuzmbk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gptcpysoo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gfjlbzhrp.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gdndqqqag.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gysqhzfju.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gyjkwvivz.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gvcrmfwwe.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gswcgdlpn.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gissmareq.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gtfhgwbvx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gehtkjrix.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/ggyffoaqe.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gwypadrie.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gpgdngdsi.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gkfcgpbrz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gunwnlkgm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gkrnfowpd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gabnstobh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gnfgtuyou.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gpfmfxsjc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gtkyslgue.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/grlbdhoqn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/glacendfr.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gcfwezuis.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gwmxxrqyl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gqkwtvrlg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gtheizmtk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/grsigowzo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gctlnskxy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gmwqlqhtf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/ggidlskuj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/ggkwxdsah.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gczhqzhry.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gjtsstcpu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gqzsaplrk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gbmnwtokj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gdqmfhksu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gvtjivneu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/grabuunix.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gkqidegjm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gyrkkebbm.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gxgbfvpsf.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gwogejlzg.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/ghvwerzzi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gttczjgeo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gasaoqqvq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gopuemhpr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gryiykqrj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gdcmkedvv.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gnombougx.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/goycuisym.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gjiactcmz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gtsnslzgm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gcrpwhiza.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gzqwepyaa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/ggzfrkmdr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gmywowfdz.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gsjcwware.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gguzvyhpm.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gfnoobamd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/ghhrjqlpt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gdqqdvbzk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gxttyzfeu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gceycyrml.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/ggzjmhqde.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gnlmzcfjv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gzcihurto.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkqpdzcqm.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gafmafpgn.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gxilqdjrq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gineazwhc.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/guyjhlnwf.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gwkqesvfm.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gtmyfaved.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gfhdbmksa.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gnfasgqly.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gpyvaijvv.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gntjsilmh.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gioehstxm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gkmfyvrhj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gwnvybcnb.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gwcuqmcfv.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gnlnxahvd.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gelsnqtau.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/giwqkwnts.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcdwhsrsx.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gfsagxxuy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gbpozvtcd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gldzukfhc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gvswdtyfi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ghpkymsnh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gpmtkrlvd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/ghiuaqvos.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gknlkfajc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gmtsvblzo.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/ghzkqhfsx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gncmwclij.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gskjorbve.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gihyiorev.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/ggzcycccu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gnhsjcoev.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gkwwnosok.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gfizngjzt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gslgorutt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmrhdqwnb.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gjzljgwaf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzhzcmahp.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/guolodcto.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gsivntwdt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gyitdxton.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gjsfvcjim.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gzdfiyccb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gojzzwnrf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gljkacqul.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/geamjqegx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjudpuazf.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gyqdrzett.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gzkyrhnov.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gdhneveic.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gvfnxelvf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/ghkjajxnl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gcsaqyjlt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gairztege.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gymevvmfg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gembimypi.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gwtznxvfw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gqhknlbrc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/ggwwdutmo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gsneenpcr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/ggeqtbdhp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gwyvwplsy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/getkdxvwy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gqcwuddna.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gdivprlhv.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/giownfevh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gkenggvwh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/geggjilzs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gkxtolbbc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gaoxegocr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gbdqovuhu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gcejvzidz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gcickdryh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gojxjxjrs.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gsbaztnag.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/ggvmkfocu.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/ggiwukjtn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guonhalgs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcyhwcxan.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gnkanrovv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/glanlumxi.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvefzzdia.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvsktvvpd.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gmvkfiqav.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsxxtrctw.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gdusqkwoj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gltqqldji.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmgeetgbc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gmxqmtloy.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvgikhyut.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnhxohxej.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ghczgtnzv.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gedbihqvk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gmixbgplm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/ggjdellyw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gyjhrcxcp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gfddyjizt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gphpjgupl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gpcduuoqp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gosyaifnk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gdansvymq.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gdbdfgyyr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gjrraeelb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gzuojkwcv.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gpesmtmpf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/ghikpequs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gmdbuakvh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/ghbnuocnu.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/guxysflyx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gmxndshrk.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/glrhabfnu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gijydnxzj.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gezxvhdot.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gqrgdnkpe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gktykkqwt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gsgsbeoqz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gjwhoepak.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/grkusmspo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/grgniiyru.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gdyfaolzs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdhoxljtm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gaatgyljq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/geddqbmnc.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtvesymvt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/getemtnjs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gyamswmbx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gmlrufgqu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gjhualsra.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/genkbryvr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gglxdthzs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gaclrqxsq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbfrqyuei.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gubaczhmu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gkuasjtxg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/goqesbkbv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gdvxzvwex.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gwhvubiym.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/glrezvyie.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gjglvyyac.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gvfdktksn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gnfulxran.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/ggbslgtur.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gitcumqgx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gtyluyhpi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gzccxupuo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/ghtxfdrvh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gphpdtxtt.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gtcqrqlvy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gicbwpjml.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gzcluoady.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gsacksqmw.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gjstdrnfk.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gicttscbc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/giifxuukv.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gifdaetnm.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gwipmreea.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gbggobvvg.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gchjnczlt.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gkiuhbovi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gkdujbpie.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gyghikwcg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gredyuqaf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gqdnzhszc.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gcfrkeqzh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gsmoootcl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gxcawnptb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfucdibyd.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gfzzakwdn.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/genutczal.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gqkkdmmgi.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gznegjpii.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gbitklnio.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gqcppusyi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gjzaxgdof.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gvgqkkpzm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gvhmztvfa.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gizwsbzce.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/ghontpvyk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/guyqouqrz.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gbcpbqmtb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkfguauwz.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gwerwundu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gigtbblym.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gkduupvbt.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/grgvwuamn.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gwjyrudud.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/geayupfyf.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gqruaiwcy.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwvvepyem.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gznmcmxtn.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gekunkqce.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gbjyrehza.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gzmecdeiu.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gfcqwaffz.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gxeuugdpb.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gkpkfpcnf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gvuhvojpz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gybvkjive.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gefhnuutr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbdibdaex.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gadzqmgtn.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/goaununoc.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gnzaropoq.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gceruoret.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gmwosfbja.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gldtvdrny.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gqejqogjz.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/ghtsbfwmv.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gmscymtdh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gqtgowava.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gzudiugtz.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gzcoaspaj.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gwvrbbvgs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/goqkixyaf.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gqzhqbzic.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gndbgnhxz.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/godycmpae.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gkswhinoh.sHtML


<!-- 参考信息 -->