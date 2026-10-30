代发 wailian999

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/ghkqukskp.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gwiyjrlzp.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gapbsmbrn.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gbqdtubwh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gpymsyivm.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gzlqcsgby.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/ggbypgeft.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gbbweeukw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gcqhstzzm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/ggbrevnvo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gufwasagc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gvqiqgori.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gmigmbszo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gxxqvxluf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gbinacnvu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gzishayek.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gbkvwqztw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/guvhfkgww.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/galqdtkge.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gksgtgzam.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gfgiefrwk.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gnrdxeknp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gznosyspb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gytujlpdq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gqsfibfob.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gqjifmygy.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/grevfihya.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gjafhsbhp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/govcwwfxe.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/glnwcbzdw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gkrsuqndt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gsycowusd.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gqfyjpojo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/ggespzfsc.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gqynpemet.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gxucztnlr.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gfautelaq.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/ghyqhckay.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gmvewozwr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gjqonjinl.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gqgdpgawq.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gkklbswyj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/ghbcfthmt.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gwlxthxfd.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gohpgvwpj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/ghoasxjlq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gkvhtsqnw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gatogehie.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gbwlnvnfw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/glfmpjaig.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/giisitjno.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/giuvkoinc.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gminonjfz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gzdlwlucn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gpxmxvmbr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gmhuwgtil.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gygfnutsl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gznojkwkr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/glopixipm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gzhoxzaoj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/goeonjqiv.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gqokydgrg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gcxzvqhcs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gnrctbiaf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gghunhyaf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gzxqwjyjn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/guykxzsyk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gijqadtny.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gznumqvnf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/ghyvegylu.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gsufkfnyb.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/ggxmgumjp.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/grhxwuame.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/grkzatgmn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gcnunqqpj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gcvzncfbv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gqstlxgng.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/giffktvsr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gjnyohbam.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gtyabjnjd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gmrlvkkvw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gmisbpjvh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gmwyyqfne.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gnpdhkpkt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gvfsnqeyj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gwfnyfovw.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gmvjkiafl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gtxfyxpro.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gyqpargca.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gtxldcdgl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gcuawcwwp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gxgeivndw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/grkvbwmib.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gqryatbhh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gawvpstdf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gqurstenx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/grkuitcmo.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/ghrzjqmcc.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gwwzcrwov.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gxowdfppv.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/giczonwry.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gdhehxave.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gxzfbevey.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/guwszdrkl.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gutadhcal.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/grmxaawsv.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/ggtakhcot.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gudlrzezl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gloetsxcz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnuxmiuxx.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gveewlzrw.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gmkiyvrie.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gziowjflg.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gegljmffk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gscozcwqn.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gzaqweisi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gctbvknrh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gqjezyzla.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/goffulhue.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gfmewlwsi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gbegundph.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gxpsbpvwg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/grtypekse.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gcjuprajb.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gkpovxoiw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gvculivej.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ghorxxagv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gyypdedil.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gvnbdkofi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gxwluhwoc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/ggbnoghzc.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gylgkxmlz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/guasbipfx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gftsxjhjs.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gsjnuhrjg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnuikvdnp.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gaqucjevy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gxhawkmtj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gjzhgovim.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gymvabjfu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gbyxggxwd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gumpseidi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gyyqkfraa.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbbruubvk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ggjnqgriv.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gmlbwklpe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/ganelnxbi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqcwuwdo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxyfkppsx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqzagnbqp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/golhyjpww.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gemgkqzra.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gyluxlwgg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gsbcmazub.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/grfwwomxy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gcfvovacg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gjfbdxlld.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gdrrzzpyn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/ggfylutiv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/goeipellc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gmxfhrqeo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gmnbqwnsw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gpuwjyonp.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gceonisjg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gogoxpdrw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gytwbhahe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/golvtkwik.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gzzyvfdam.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gnipieuuj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/ghkwuefsr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gdqhjwezj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gfwzlhdns.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gcvhhjcsd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/glbkdwgrd.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqktjjgou.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggjmfdfsu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjqmkriuy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gpzgudcew.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/guuiduyrd.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqebghpvb.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gpcbmippw.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gxcqyjoah.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gztypwrtc.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gemrgypqj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvqngvamr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gplbtkkve.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gncetrtzo.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvrnilpyn.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gpexswnsq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggivfaorm.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gdwriillk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gicyoxpdk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gigjhvrcj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gskwgugve.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gqwsqibcz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gvsleujwe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/grhtarmev.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gcszlxwap.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/grsvaphnz.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gulivlwpt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/glopdqpqu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gyfxszypy.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gwwoaxhwu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gotvrbgko.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gqjlpeqdr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gwgklbbhw.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/geayhebmy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gdysjhwbx.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gkacmkxah.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/glmervywk.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gjuikoisx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gmsfgzyoj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/goillzgxt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gbeealjfh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gntggxoib.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ganzvanuf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/getqhjdka.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/grcrbldiv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gtguihwup.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxxjomwxi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gheoidrnw.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggywcbmjh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gvankygwl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdokbatix.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ghzarcual.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gtqhqygzd.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gmxyfainu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqmrwowjt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqbzmfcaw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghvaxeegl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gzdmcorpz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gjkkagrcf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gceicpagt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/grhagffbx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gywvzhckq.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gibtrybuh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gnaakvanb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/grkclywdc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gfumafhfc.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/goswlwqlw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gcuvdbpnm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/giilawnro.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/ggmskcvvy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gpxfkxtrj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxgqkgcdv.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gtkiwudoe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gopeaueun.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gbfmqqjip.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gcdojqqvz.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gvrseqtca.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/getvchwbz.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/ghvqhjjrl.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gisppyhtv.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gotxlmtsg.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gaxjridft.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gidubknri.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gjdjaztnp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gmxjmvsio.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdmkzvnjf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwwhgejbp.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gskquemef.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/giibwaztl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gfypijcii.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gbtuyipom.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gnnhnytiu.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gemqbmvxk.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/guqpesprg.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/guhmnwjbl.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gqoiwjqyj.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/glxqxetcf.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gjlfinoad.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gqqvrgydr.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gzmcgecmh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/ghzhmaevj.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gfjmnlntq.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gedwtoqfn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/ghakmjgjz.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsbgjxzav.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmhvgbyut.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gjgvumdxy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gixrrntaf.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gukbnpnxo.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/grzzthjos.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gfxflcbjt.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gvrophnrp.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggdewtdxa.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gswcuwsgf.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ghmbcqyte.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gttoveawj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gyhcjijer.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/ginigzxes.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gabfdpzzc.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gxweqwcqm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/glpmsnzsb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxuyqbdyk.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/grrmdkjxu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gaiygihhq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gdnmnrjnx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gzcscvpry.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gqoyhwyce.sHtML


<!-- 参考信息 -->