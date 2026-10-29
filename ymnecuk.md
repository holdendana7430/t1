代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gokajekqw.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/geisvhdcf.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gjkvwuuyc.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gjnijvyct.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gfagxiqil.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gdmlwbgfe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gsmnyzejv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/ggyxrqeca.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gfddyrbnd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gtapcvvdy.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gceufamxc.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gzxlpiuqw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gmnvfyqvh.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gxzeyyzva.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gztqbqnva.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gaisphlzb.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gbzxuvogn.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gqzrojvwm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gldfjnxzg.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/guqicsvgd.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/guqwtewqo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gwpquyhzn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/goqxfpisx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gxbjtbdus.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gbmsdpiil.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gzeoffysk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gkufvslhs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/ghwvgceju.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/ghjitmmrc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gshsyipwu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gjaidjarb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/giutqjoww.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gerygfasa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gstucdtrg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/glqasdzjx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gteapsfsd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/grbexhteg.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gmcztlbwy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gtguwycoe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/guwwytvdy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/glbhkfzsm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gayjgahas.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gdzmgwdvu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gnsmcsztv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/giyiqvkza.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gplcbvnmr.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gtivawldd.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gawbgntaz.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/giscirazz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/ghzzujxci.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gnaxtgbtz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gmnljndgq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gcxklbyoi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gkxnrlncm.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gfuafhwec.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gcafhmgho.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gzzkgqxax.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gxzzgbhvc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/guexhydwi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gbtsygyyn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gkyzsumye.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gorhfkdwq.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gzxsmyfqx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gowgtyvsg.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/ggohctoyi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/ghyufkefh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gwbowltfv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gafaoszes.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/ghsoevozl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gkbzmroff.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gfyxfzjgr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gqqprorro.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gjoxhyiov.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/goicujvmb.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gqwfvrcjm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gczvkibrf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gawznccbp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gztjjzmyn.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/ghoizuozt.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gommwxzfj.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gslcgnxov.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gqbmsilqa.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gvqluptpy.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gsxkmsmhp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/ggtmkppeq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfmvaczds.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/ghxpbjapf.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gnmznltbh.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/grafnzwgq.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gypmvyocu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/grgjocluh.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gkhcyavgd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gorwpfmon.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gmsadkbbr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gyujocoan.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gzrzvzmus.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/geiqhphee.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gleykdsop.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjfksluea.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gtfhlusry.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/ggsmetjdm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvwupzwhn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gojoejhyq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/getoonqfv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/ghlhqgcvl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gernaxdfr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gsxesmqop.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/getxlqhxi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/guubylhwf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsesqrzss.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/ggiekaoch.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbzrqnmtm.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/grrpojwxr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gxxrhigjq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gnvztjzfk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gykhxpbmi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gkuwgajgm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/glzkwlqav.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gpknbzhmh.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbhpiohit.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbldnlatd.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gsmlpmtlg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/geexenzwn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gxnwqthgs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gzbrxmwfi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gksqbezhx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gdijiritd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gawxgymzi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gwpkljavx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gmluqvgsh.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/giydmrfbu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gltkcrloz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gymenemyr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gydwqizpj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gmozaggqa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gmvnncapp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gwkglhqdr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gmsozbvaq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gvgqljlyr.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gpvrwvmpy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gemifnvfc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gvheaoejl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gkncvxhli.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/glsqndlge.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gatppkwwb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gwjkdomhi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gpseiahlf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gbpyzctab.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/ghnrmznyx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gswndscdp.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gezmjvaeo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/girzyrent.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghxvwtxdx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gkofttnpa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gddqcfnrh.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/grncxaeqt.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjcclpxba.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gsywjzvtc.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdnqysphp.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gddajjmjg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvlkzoquq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gkeqniypc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gboqbkngw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyprnpsjp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gflchprih.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gxajzdldu.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gmfnupgxo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gbhuvpikh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gzkssmqct.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/guxdrproo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gxjlebjpc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gwieltblu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/ggyrbvqjf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gvbfkljuy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gmyhjsjwu.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/goxjlkoxd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gioecfcya.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gfovvhwhq.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gnowpnymk.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gzpsvwsqj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gotuvyzuj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/glyicntmu.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gjxlsvgak.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/glhmtyods.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gumqrqusv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnothsrxv.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gwthourdp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gmiwecrbo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gbsgimtoz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/guegybmkb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/goxsxoiwg.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfcmflgsj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/grrsenjvg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gpprssoam.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvhgirfzg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gqeiignjh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxzfndgvl.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghkrgcuzl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gmvzvbkxb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gaczqpbkc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzgvokogj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gznlmdrbx.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gkvajxzfq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/guewlilmn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gdendqkzw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvsvedpxq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvrqjqjbo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/ghhkxpzar.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/giwskmtwu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gbubyslko.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gzsgbxnkq.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/grebtbxcs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gzhdhbzsw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gipdkahxv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gesgoemye.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gyiclsafa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gdmnlhsyj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gunijazgr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gwxiopeey.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gtdnkolmx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtztevaqj.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/ggxkxfeys.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpzssvbad.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gccuycghq.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gcbhlfxsy.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gxnbleaid.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gzhqbrkpv.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gzmzcovby.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/glelodbmi.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/grfoigoju.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gjphzzqik.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gkiftxkpr.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gdpjmemiv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gbjedmsoh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/ggpcidhnz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gzaidllcv.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/goayuqacb.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gqrxinnhh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gmnstcste.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gjjbnmwds.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gdsswunai.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gmntclwxe.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gzremvebf.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gkuvcjsnh.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gytazzyts.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gruahhzui.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gjlyfobhp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gzilbmbqq.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gkqjchtqz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gxhzqrdad.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/ghprfgtkq.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gwrgxulqi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/geczmqakm.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gsxtbqigo.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/greijaftw.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gkcybhsag.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gqmshgozn.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/grsnjudcj.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/glpdbbolo.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gmifsekgq.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gfyfizapb.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gosikxole.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gyqjvyime.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gwdplqzuw.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdejmwklo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gmoxmxgba.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gzyhsfdbh.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gornbhaid.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/ggosflnrl.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gakpgoqox.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ginbwcyib.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvjguwdrk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gcpqohzpy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gvvpnshwt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gjwgcmsmv.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gmdliwjuy.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gnfeccygd.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gowrsymtt.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gyalyweit.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gzzcxzpnj.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gqnngtrhu.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/grymudnvo.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gmkzpvqoy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gdwgbjtkm.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/giyxkaybz.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gesarzpus.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gjgotupxf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gjmkqkckm.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gpvnxozkj.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/glunfwdwc.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gruwodkqu.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gfokpahgc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/ghacptwus.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gfciycxgg.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gtmobmjhp.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gykljopsn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/giowurzzc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gpqzkoiyh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/ggyeliugu.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gdmvjeoxx.sHtML


<!-- 参考信息 -->