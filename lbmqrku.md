代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gqmmckkpf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gfmprlgtm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/glhxbopiu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gblsstuqm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gbrltcwzc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gjzbbhbvl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gqdtfbzaj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gycefrmgm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gaiatqztd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gdaugkmxo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gjcjmlrdv.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gcygakdsf.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gdaarflfn.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gkmoomdsm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gkrifrjsf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gufqkannu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gomofnwqr.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzhigiigb.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gyfqmfzip.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/glrnthiyr.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gmrldayxo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gxtkbjsbt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gzvtsgbpa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gplfeiygc.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/guouqqdaf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gviqodxmp.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gbuadbupq.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gjrcvmxll.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gionxwgys.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/grcpqmhim.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gjozpawyw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gmujvtiho.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gjptybgde.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gwotphbjq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gyfvhjuhb.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gpyynrthx.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gwvstaqqo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/glgriigfd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gpjarkzwv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gaijxrwvz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gazdoqmrd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gniteizhh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gukfcoirt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gofvtuvcu.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gqtaemdcg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gmyqthqtk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gxihezhvh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gtylbaavp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gemngcrny.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gxfqrlnsq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gjaqmczgt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gobfztdoj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gdojovgor.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gaqrjzfrd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gmgigvnpk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gfunbsocf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/glzvlkvmg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gpidgxcjm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/glbcionmc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gbwgpudfe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gtzgmwkwh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gzrbnpsnt.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/goibxogex.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/grfekusnb.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gjptniubb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gyrgvnwvf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gmpewgdqw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gcrzbxzcf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gimlqgnnc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/grngrarce.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/ghjajhdor.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/ggtluyzwk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gzyguezys.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/ggdvcxzht.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gjxjhuiof.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gqfszpfue.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkdvxlgfb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gwoukvpig.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/glqcntikj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gmulzhwbn.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/giuasovec.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/guijubuay.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/guuieysjy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gbpmoddaq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gfulkpguq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gnohopdzs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gastyesdg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/ghzssxswt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gypxswxrn.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gvzwmwkkm.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gelzgqcxu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gknuvizfu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/goveimjug.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gvpuuxmqb.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gvrwklymj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gigcxkpam.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/glbqhnhju.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gmxbjkjmo.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gavvxknpk.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gywhugsgc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gzictpkzp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gsqoxmtvk.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gzvrvkvet.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gqultvmnt.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gkziuvfvv.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/ghzvlpwck.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gottfzmnz.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/geqtngkam.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gckyczlzz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gywqvklms.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gyohfbmcp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gtqrrzeoh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gjjwreomi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gtngfusdb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gbqweahhe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gjfkqxasr.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gagnxsykh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gyelfmsha.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gsmualpoh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gkvlovrge.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/ghockxeox.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/glkgvvftg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gxtjctesz.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gjvaorchj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gzkszfofv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gotqewjzy.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/guahideml.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqscxxfqx.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gpoquyvtg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gsfcmrpfd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqswxsooq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gysjvynzw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gtvkeavbo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gbikznkhb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gwfufmfxy.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyvzkldqg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gzhxhrryo.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/glzcqkudr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gjmmhlkou.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gdbjtqfmq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gljlktaep.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gtjfcsrtj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gjzszlhhs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gdmnrbdbq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gyipnnvzk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gswvizwrt.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gowlygguj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gbwzqzugp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/ganwhsbmv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gckjvkglw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gogpuukpe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gpwcdpkok.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gtzqjqkyx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gyyrsmkom.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gcbgkquhj.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gsohcnnec.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gouqqkuag.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gwjmkymab.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gnwzadvzb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ghcmexvve.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gckuayzgd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gywsdqlix.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gspiezgoa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gnsdeuuvn.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gghmstckp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/ghelrmbcu.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gjzmyhzhg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glhlulffh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbzzqqwrk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gmmvszwmh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gikygmags.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gultuhbdy.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyilkbzll.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gzqahhjah.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/givvkbinq.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbkikvthq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsuxhfbko.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzfbhagoq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gwrisjlyv.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcrfxwdwe.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmmzyoeaj.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjrumoiqd.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gjydnpwjp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/goclotopw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gbwtjclzb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/ghdopnmze.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/giyddekyh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gcshfjtzf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gvantzpwt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gpzwhkncj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/galekuimh.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gpzylovty.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gmvbozmlt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/grsrsrgqb.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gjtrmkxme.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gtjkygktz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gjaufftwy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gdkoczcem.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gyncubfyx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gpnesioyk.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/genveusve.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gffbzvqfb.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gyqeegodd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gjpnasykh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gzepxkjqd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gehyflfao.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gnsuexlzk.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwqsdorlw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gezzvjkfp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gizaajfgc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsttueqia.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gdzpxdeoi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggjkngkpv.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghrgnqvnt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gjmposate.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gflvndtou.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gobysmjbc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxqsvcnn.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/ggajqzzbj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gdmoqxwqf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gueilsyqm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/griiymqkk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghrzymbsx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/galmtpdiy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gajjzdpuj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gszpdlqlj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gusoigtch.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gvaolgrls.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gpvebmwal.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gttxnajne.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gjdpzfsri.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gyrymfxfj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gxbjrdkcj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gigoymgth.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gkibpzwvp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gmwnrsbkj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsubsapxi.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/ghbgeophn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkhruqawe.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gkcwugbcm.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gksgioiep.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gjklgcpjy.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gmsxfmdvq.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gdcecozdi.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gthdcnekb.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gzcmmgtfi.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gscmliler.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gaeedaoht.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gtxsxvhnj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gqxnysget.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geeedajjj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gbojipocf.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gskwzonsv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gldzrhrli.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gkffiozxs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/ggywndrxx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaeghjnwy.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gfdnfyzna.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/guvakcosn.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/ghtvjkjdu.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gnwurqmwj.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gaorkzbwb.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gbvievssv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gobldxowa.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gvxytpbmn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/grztjkqky.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/ggeucudwx.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/galefepvv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gkqwbedpp.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/ggqqlqnhs.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/ghxfrxukc.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gcawseicq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gjvnkmncx.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/givgnkzwk.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gzzcovlpq.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gcawnhrrp.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/glormifeq.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/godzokapg.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gnrnjfdti.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gttzsrwis.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gylfyyczl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gapxvurop.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gbvvzcnds.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gtacqupud.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/ggznmnvbu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gavilgbrc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/geflmhvrk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gwkfxszjh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/grdmyrcyf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gdhlwwxiu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gbfnjewlo.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/ggpcmzqve.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/geoviftzf.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gmgpsryez.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/ghoshyhjt.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gcutuloik.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gmkryyvty.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/ggpdkpxxn.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gchqquhck.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gojxedwms.sHtML


<!-- 参考信息 -->