代发 wailian999

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/ghmrkausg.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gbpntfhcp.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gndxkdksh.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gtjwywibw.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gvbpwncad.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gaquovnkt.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/ggyvjbzbj.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gbetkyeei.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gdtlhvtuf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gkfnbmivm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gnpbhbrts.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gcxuyujti.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gsloqnvtv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gkgalvnxo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/ghqbtzpdj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gpeuozper.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gxsolwycr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gqocywjtt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gdkmjghta.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gkmmywnkq.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gihmqngld.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvfohbku.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gmcnxloii.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/griymspoo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gxyxvrtnt.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gauhgdppq.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gbygymdnr.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gapldhpiz.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gclmonlxz.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gwyewxore.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/ghfbpvzcw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gjnqlkvtn.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gobictwaa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/glxrazamc.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gszzukmat.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gadoygbuc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gmfwrusyz.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/guhrelcny.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gxcfmqzeh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gexoiljde.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gpsbdqhud.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gghyrwmud.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gviccasdm.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/ggldpdaie.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/ggdytzdao.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gtktjsrxe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gfcchegcd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gkcafosvi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gjrjnupqi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gaqgnbxzp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gowsuluux.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/ggmzvjejd.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gumqarjkg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gwjprbuth.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gkwixpslw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/grcgzilqj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/grcsbqwlw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gvukxavvv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gwlexixfr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gcseypkgr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gpalllxfo.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gtxsxewbt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gtvuzoqyx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gavdtndje.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/ghmbkaofb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gqmelgkcz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gfdghbqoo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gjvmgiowx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gbvhnlfeg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gnfnuyidt.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gueywnlxl.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gtxcykhal.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gqlzwuafa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gzvaonanu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gglodtvls.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gaesowfda.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/glevkvsbq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gvjfxulqg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gxpxngyum.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gxnhrafuq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gjumguaip.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcwvknmku.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/grwxvqqpl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gktbmbcpw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gczyitxwb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gefwwhxxm.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gtfudeknv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gtaujoqan.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gfryfrobh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gqbfjzzez.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gkfvfnryr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gqtggdzah.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gnbpqtbqk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gxvdftwik.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gsygdpmsa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gjyxydyrw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gsmjlgrtr.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gsmhhtvhn.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/geeihtedu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gaorrmmbh.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gesyipztd.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gtnjhkweq.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gnpivjbbw.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/ggrsjgomd.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gjrakxevl.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gehksdede.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gclibmeqw.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gnjudfxfl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/ggnvlkwnn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxlggswlo.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gkzpbmgyp.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gvxmueeoj.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gqijvwmpp.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/ghwimnnnt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gzuobztex.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gmnycgitm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gxfsgdtxp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gnybbfjlj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gfycwpave.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gzroecmwh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gnvlygbbj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/glgykocge.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gwhzefmlc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gapltwnuu.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gaglqxwgu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gscilsjyy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gikwfnzlv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/ggxrrndsk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gmlvcidrt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gegoxgtdh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gfxpeeszc.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gblfuwgqf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gkhbovnqs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goyfieklm.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/giqlpurvi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gayvbizkv.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gwmkdvxya.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/givkigiqr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmqktgxmo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gwpkxyhwi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gxvixxshj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gymcsycly.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gbejrfpue.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjgfkpdqo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/galxwzesm.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gnxylracj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gctyomlzf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/glldwquwx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/ghroefqye.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/giksnypcq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/grckocvwd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/ghamnsxze.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/glpxjzszp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/ggntpacpi.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gtzswnyja.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gtjkresfq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gwpaxjhtg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gqtqgnrkf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gkjttypen.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gibwbwgad.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gkkvtcmrl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gjxudszok.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/genjgihbb.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gokbkjpyp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gvfqmoiln.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gfploxfcc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gabgynqqu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gjijolmfn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gfcpkwuni.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gryimhqmf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gucmmbykw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gyqlrdcdy.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gnpvunhmw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gsxvxhqor.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gfnlhclvb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gukxqigje.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gneisgwgi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gcqevmsnk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gukajwcxu.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggcaicdkb.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfjiuvehg.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gvprxgfxi.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grvqsbeqv.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gumevwgji.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzrvbgivm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gayuiskyu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gqvexpkzj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glzohvekm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtjfsdvgs.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gcdfxdkhp.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gbimdmuba.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gmpxtiueu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gndxvpefq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gegzutbgh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gyigrkxtg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/giondvkrz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gkxfdaaay.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gvklvgevl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/glwxddudn.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gypmqzebv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gkhpzitkr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/grolwidvh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gtvctcrcv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gapyivqgn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gerkkyigy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gkkuftxzt.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gncrecwdu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ghiihnqrb.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gnhirjxwm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcxbeznlc.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gudhommnq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/grbtgpiej.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gtoudldql.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gjhinxpsg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gtyeztnlx.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkkpalkyk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gzdnrpexw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gvabvzznm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gknpgaoar.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gzfdjpicd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gzqpvkgoj.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvpleuccj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gprvifruc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ggmbrkrtn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmlofirft.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghufxisai.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxhyuyonl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gstdxhawi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gztsjicmr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gtdldrujg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtnvisqey.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gdoohenzq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/guhpsofbd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/girlpvblf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gbhlcsqqb.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gbivhzhpl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gifosmgcu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gieccikza.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gcqdasziv.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gyfgmgqwu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gffjetyiv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gqtaagjjo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gfcleepic.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gqebfkgmy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdbvtzjol.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gsuqvdvko.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvslvczzo.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gcslqdhgp.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gveswehox.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqytvwgba.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gjrijksmd.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gnnmckpto.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gyyjhdqft.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gjgaqzsmq.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gapszlkfq.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gddnceqzo.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/ggxcuqvdw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gnabxdrfx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/grqicktmx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gatimembr.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gourbzytt.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gmyrotsdd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gvtikgzgw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/glcvkwica.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gtbvbkjul.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gjpxloqui.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gfzfqdchs.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gzeuphfeg.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gnlmcjvjx.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gtzvqugnn.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gxsdzyjjz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gmkzphggt.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gvtimipva.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gyywgtlrr.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gwhclxqst.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gmqemqqor.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gztfzcbwe.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gluzoxrnq.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gfrzhqrex.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvtpnnmd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gzglzoifz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gycbhgckt.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/glcqvtbso.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/guomwzdbx.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gthhdxqzv.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ghqxgvftv.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gjfqnbgkg.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gwntoebqi.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gdzpgelha.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gknhzkvth.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gocrchyog.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gcpoghtme.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gayghvyfm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gptmpfasp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gahjgnpgy.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gspomjhlv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/grjixfquv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/goaebmfwh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gfxanopzt.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gveriebjy.sHtML


<!-- 参考信息 -->