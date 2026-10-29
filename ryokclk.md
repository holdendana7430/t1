代发 wailian999

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gkhkonuhs.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/goenipqcp.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/ggylmebjt.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gdocfyist.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gqegfpafs.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gvnmeteww.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gymjqpwqq.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gtbvekyzh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gxwdwwtgl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gwsiokoil.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gghkfghdi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gensydesr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gyktehnap.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gmxgziurx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gzcvhgpkm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwtfxaghk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gcqfxfqom.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gkovwrrut.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gvrjrrsew.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gpmiubnab.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/glfjqxjen.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gytuvqttk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gnvdtungm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gwclfprut.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gjplspqqf.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gmljosmml.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gvmwlhowt.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/grqmkppsz.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gmxbtxiwt.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/glxogdqae.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gklhjygab.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gnjknctxd.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gfzseauhd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gnbqubmkr.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gjqdqfrqe.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gwsotlora.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gvudtrnga.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/grfhfbabk.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gwvowkuuu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/ghwgunodz.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gtbvboiek.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gjzwlrdnb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gtjeihldc.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gikkbghjw.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/guhrcvssx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gacldcsbg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gmonftvjw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gjsqtejcv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gksweykel.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gxofzhddt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gdeovhgzc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gzgsoesvw.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gefdmtzfn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/ggvpqljez.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gwkpmajfn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gocvzzwou.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gtfxbveva.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/glrrbduki.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gzrcpfejz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/ggikfrqxa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gyxpqprmu.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gnxybwzfd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtikxvabj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gdlymjlcr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gupyzadlm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/geylncmow.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gcxowmvox.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmfijozdq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gachvijmp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gpbebloog.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/groiffgcc.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gwiksfxaa.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gbfkfqope.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gbczgtult.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/ggvkdajzc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gbcwmcvkk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/ghtrhqeym.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/givbknaqg.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/genuwvtqm.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gyglfxktq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gelnfkflo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gedpsvivw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/griiyhnrf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gyqskccaf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gugzeqadr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gstbbqywe.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/ghuxfcjxv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gvnlqrkhx.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gwwvbjhak.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/ggvfafsfu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gavjpiomj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gulsmspol.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gtntgxsor.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gqzqrtyuw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gonppjxbj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gtroisrxv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/grcczimyd.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gobqvrful.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gphzjwytx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gizdiaxaj.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gkjnkoowg.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gughojoxu.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gbemirgln.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gudgfpqhf.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gbfmajfsq.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/ghlsttwdm.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/glcdupouk.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gguljdwjb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gfktgvopu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gaugmlgvi.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gcbkntnps.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gclgtwiml.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gjlmjgpoj.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/ghvgdnjmw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gmyhnkzem.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gykvhblca.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gbymlhekj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gkpuqvfpv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gtfqsrowp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gfipyvmtm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gjcbukvts.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gwgrzcaxf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gerjqfveu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gaooornxa.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gipeelpfi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gdsyczfas.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gnlujpedp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/guaorjkou.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gjbbrxwgd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gezobwifa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gbkuainuf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gigjrndps.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gnqryxyzo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gklpaqkna.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gjohahwdl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gytkvzssn.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gueheinea.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gkpdlfgca.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxtqbflkv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/ghoirkfjb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gnwmplihu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gwlflguuc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gryysurni.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzdqztuuv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gysyhdtnk.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gbjbmplxh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gbwbalmzf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gpotncsoo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gkyapunie.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gjoelgrck.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gwgxuxswb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gngfdetki.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gggimqyvv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gulfbuyao.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gugmqjanb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/grurovhip.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/grhvamsdg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gviavagjr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gbmrifmgt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gaxnixrqp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/givqzxtkt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gfxsxxhla.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gbxfglzav.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/glfdtkljx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gxyeqbrcy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/giibswwri.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gpqnmmqjl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gnbflzmqf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gilksywvi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gpmwavxbb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gmkdzqplw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gjtmjpuew.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gpkqdzepk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/ghohepflv.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/grnswezvw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcvmrhxjt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxffasdov.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gaaznoebd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gyahgwwzu.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjewlktkv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guaxphgxq.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/ggwqjhilt.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gustdjuad.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtrtxjuih.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbflksnrf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grqbwdsxh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gfunyntgd.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gprnczhcn.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjxfypnoz.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghmdpolzq.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gdfebzrkd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/giefnpjhy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gvfexpxed.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gdwbdunuk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gpfcjzswv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gxtylmhdn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gcusrgeji.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gyztjcmlf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gzhhjydzz.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gaaljvjzf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/ghexqrlza.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/glggmvilt.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gqrrzkhcu.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gnbptpktx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gwperxaar.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gizojnceu.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gmxsezirl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gnveyywuo.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gekjqyprn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbzfxrjle.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/givgaiypj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/glllgtmuv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gcdgtqvbn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gedyiklam.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/guobzxbbv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdauamnst.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gtqfeogtf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gwcaahngo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbhxjoxxk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/ghsxhipsz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gemnmzpvg.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gayiripbj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gqmtwaejv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gzsibsvrp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfxnybssb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxayfzurk.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gbopntykk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gsxyelgnk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gtpvatytw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/glofbxkat.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gsozxohxq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gmnjgsviw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/ghdzcxbqe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gpnxjuvsg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gpkoluzye.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/grdiqzfgy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gpdbdznqf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gsxboemit.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/ghxqmmfth.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gcpjhiafq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gpqjdavqz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gdsormvpa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gvjwryvuo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gtliyhuzr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwbagcval.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gxmfobjzb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gohbrzujm.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gtgiyomin.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gpuzjyzdu.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxubzjbzi.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/giuhwahww.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gxuygrpty.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gmgdifxdr.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gvkvusxpo.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/ghqpsczpy.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gprxlpbvy.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/ggmvmappz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gylxkqcav.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gittgvnym.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gpursuzvg.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gfghlwiao.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbloflnam.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gyusjirzj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/guhqrmtwl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gxrtraqsj.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gmohxxirr.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gxtspyitf.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gzmwoaflj.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/graknpgty.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gnvuagqcg.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gkejrmmlt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/grcpqrkkj.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/ggjnshwsk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gztfjxytp.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gfzrqvgfy.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/glffxjoxi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/giiumyioy.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/goapdevfk.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/ghegntscc.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gevwtqhvn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gleegrupf.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gggqoaocb.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gnctzayfu.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gktsnbobb.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gbmlhloni.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gguepkvcv.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gpyfnqmzz.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gctvugkze.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gqiymtrcg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gwjukfpym.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gqvdvjmgz.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gppqehmno.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/ghqlxdvsj.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gkdbyyqnw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gtmdbwqbw.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gqylgcoci.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/giqdryark.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gufkxmavo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gczutaxku.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/glwogmgnu.sHtML


<!-- 参考信息 -->