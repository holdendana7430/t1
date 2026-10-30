代发 wailian999

Ruby: s.split(",");  s.split
来源：http://wap.fanxiaobao.xyz/Article/details/gghpfysym.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmqjziua.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fanxiaobao.xyz/Article/details/getrrjsaa.sHtML

Py:   ",".join(items)
来源：http://3g.fanxiaobao.xyz/Article/details/gpwywkaig.sHtML

PHP:  implode(",", $items);
来源：http://3g.fanxiaobao.xyz/Article/details/gwdorwwsa.sHtML

JS:   items.join(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzqaeizf.sHtML

TS:   items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/ghvqqssfj.sHtML

Java: String.join(",", items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcotsiaff.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrgyxvsg.sHtML

Ruby: items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/guaqteujh.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdcxsufp.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpvtbttz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gmdubxnme.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gzvcunwxq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/galhcgpqw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gnyljfqxu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fanxiaobao.xyz/Article/details/gvsdycsbs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkprpehxq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gciovqdud.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcqzctkb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvaewfsk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvnqibbb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fanxiaobao.xyz/Article/details/gxrqwauoy.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjbucuzx.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnckhyufh.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmynaswq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvviihqxt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gahkvukhv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfbzfngu.sHtML

[E11] 反转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvirsscg.sHtML

Py:   s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqylgcicb.sHtML

PHP:  strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvvcmxgs.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gzhjffcwn.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gyyotyelm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fanxiaobao.xyz/Article/details/grmnzhujc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydctafnh.sHtML

Ruby: s.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpqbczwa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fanxiaobao.xyz/Article/details/gewaycikj.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsswkmfep.sHtML

Py:   s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsxylszx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzyvyuvs.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fanxiaobao.xyz/Article/details/gwdhxnopm.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gyddbjdtw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbwvzgtq.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fanxiaobao.xyz/Article/details/gvkefpdyy.sHtML

Ruby: s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpcejmpu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fanxiaobao.xyz/Article/details/glwsjsaod.sHtML

[E13] 逐字符遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/guojckviz.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkenftyj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmbrbiwxj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfimyxjj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gzauqrimu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/grhatyrme.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoppykgz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fanxiaobao.xyz/Article/details/ghclifiau.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golbyzxbc.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehxdojye.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fanxiaobao.xyz/Article/details/gbcvpfpeu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqjqlnai.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqntfhyl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphtawjpf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucekdoty.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfarpohz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fanxiaobao.xyz/Article/details/gibazcuif.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/gatpcvyod.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fanxiaobao.xyz/Article/details/gjkbyzdcc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gdsvjbyog.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuxtgiko.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gneabmfdy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/glzdtbygs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fanxiaobao.xyz/Article/details/gbytuwguj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvrtwgxb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpddhsckh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgtautua.sHtML

[E16] 数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzztvfwg.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gozfafedj.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvnfnthw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyhalasq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fanxiaobao.xyz/Article/details/gwakhetkh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gteaufpfk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gxojkvwxi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyshlzko.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fanxiaobao.xyz/Article/details/gyicmwqsy.sHtML

[E17] 首字母大写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdemnily.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoecesge.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glutyocbb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fanxiaobao.xyz/Article/details/grfpmzwpf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fanxiaobao.xyz/Article/details/glxvzmize.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gbcqhstll.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamdifjef.sHtML

Ruby: s.capitalize
来源：http://read.share.fanxiaobao.xyz/Article/details/glbfgpmwf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fanxiaobao.xyz/Article/details/ghnbeezpm.sHtML

[E18] 模板占位符替换
来源：http://3g.fanxiaobao.xyz/Article/details/gqzlxkjsq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuhmucrm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvphuogd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjccviuc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobtmbdsg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gikvyttun.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/glyqsfugy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumgtpmle.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtuxblcmp.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/gapansfou.sHtML

Py:   s.splitlines()
来源：http://www.share.fanxiaobao.xyz/Article/details/glkipmkor.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gxnpqprwt.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazkvzuwl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhiotcan.sHtML

Java: s.lines().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gkjbowjlz.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvovezym.sHtML

Ruby: s.lines
来源：http://baike.fanxiaobao.xyz/Article/details/gmppcjjyz.sHtML

C#:   s.Split('\n')
来源：http://read.share.fanxiaobao.xyz/Article/details/gkujsbaqn.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fanxiaobao.xyz/Article/details/gnghmxwgw.sHtML

Py:   if not s:
来源：http://baike.fanxiaobao.xyz/Article/details/gszamtsok.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiomnsgl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/givmttdml.sHtML

TS:   if (s === "") {}
来源：http://blog.fanxiaobao.xyz/Article/details/gnqnqdbyr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtptdignu.sHtML

Go:   if s == "" {}
来源：http://wap.fanxiaobao.xyz/Article/details/gclnkeytd.sHtML

Ruby: if s.empty?
来源：http://3g.fanxiaobao.xyz/Article/details/gxqgiodun.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gflmwunmm.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fanxiaobao.xyz/Article/details/grbeqwmay.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fanxiaobao.xyz/Article/details/ghlfccdcg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkwznyyl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/giiknwetb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchzibzsz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwferezx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxghqrdy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjgsffyt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/glsdmrugk.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyqvmesc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gyolfjili.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gycdzbmpd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gthwoztvh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gnkdfdaee.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjpobrkt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fanxiaobao.xyz/Article/details/gtbrxdzml.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/grfeckipc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwgvwzpy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkorsjbex.sHtML

F. 文件与目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmfkkugi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpmdjdbr.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglablfcd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grswetboi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/grnhtejxk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fanxiaobao.xyz/Article/details/gkmmzhtza.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/gxfzdbyjd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmulxiam.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fanxiaobao.xyz/Article/details/gapgwbliv.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/grgntxwdm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurfabqwg.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnnldnqe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fanxiaobao.xyz/Article/details/grzxnhkdk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaposdixf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/grocrtwpt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gelfjfils.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fanxiaobao.xyz/Article/details/grestdzit.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstuiyhnp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvaizruv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdualhzk.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyenstfh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvddasuqh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqqkegvt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrlkzedh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gwhqaxmvy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gwnnuqecz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fanxiaobao.xyz/Article/details/grslckwwd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gidqslcgs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gngkpsoek.sHtML

[F04] 追加写入文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gviqcoems.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpanzwayi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjjeqjiv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgtgrhbg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gewzcwfgr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fanxiaobao.xyz/Article/details/gjuncndja.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlllwskk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gutxxjcjg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqestlxdb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geagtzrag.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fanxiaobao.xyz/Article/details/guviyeddi.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gwbpfgrkh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpszrkkq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfvbuavz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtvbhjpe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmkrfhkj.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwmluqjl.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gimgnmjmg.sHtML

[F06] 删除文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxcywdyh.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyleqokwa.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gojgzaxut.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/glqhxcvhk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeccuwwz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gpweikyrr.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gultmthns.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrjjqlpo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggslhnnmc.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fanxiaobao.xyz/Article/details/gfdjjufpy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaqaxdhb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjipiypm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnupmtwr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fanxiaobao.xyz/Article/details/gxotpopoi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqfgasnz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fanxiaobao.xyz/Article/details/gduxqfthl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fanxiaobao.xyz/Article/details/ggghgbklh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesbfcbns.sHtML

[F08] 遍历目录
来源：http://baike.fanxiaobao.xyz/Article/details/gdzdymcug.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbbbpkul.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gykvohlnk.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcubaauu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksotndch.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhgnicgx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhyouvlb.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbotxnis.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuyieaae.sHtML

[F09] 获取文件大小
来源：http://blog.fanxiaobao.xyz/Article/details/gypvdzjro.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcylbchtr.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhiavfdu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fanxiaobao.xyz/Article/details/gunaimnia.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzevrflbk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gbggqqmke.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fanxiaobao.xyz/Article/details/gsbffaszn.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gfdrplxsq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gebgklndq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fanxiaobao.xyz/Article/details/ghdvrxths.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gskannhtd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gjzzzrzew.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gxmdniysj.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwexaccyy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fanxiaobao.xyz/Article/details/gpyebekyi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gdowodlug.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsusyhzoa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/grkiigpxb.sHtML

[F11] 复制与移动文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gscalssok.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/ghpvkkzgm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gxfhwqwzq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gllrimtfs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/glzhzmexm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhcsqdok.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fanxiaobao.xyz/Article/details/gmeblzegm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxmppcti.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fanxiaobao.xyz/Article/details/gpqqrtivb.sHtML

[F12] CSV 读写
来源：http://blog.fanxiaobao.xyz/Article/details/gwrzxxzol.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fanxiaobao.xyz/Article/details/gyxxyztwd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqvyuhyk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fanxiaobao.xyz/Article/details/gkgaxquvj.sHtML

TS:   // 同上
来源：http://3g.fanxiaobao.xyz/Article/details/glsgwtcvy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcrbzojc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpinkxit.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fanxiaobao.xyz/Article/details/gacoskgjf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsrwngzr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrkkazmr.sHtML

G. 面向对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsidbsbb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gybgwaemf.sHtML

[G01] 定义类
来源：http://www.share.fanxiaobao.xyz/Article/details/gjylsxrzi.sHtML

Py:   class User: pass
来源：http://blog.fanxiaobao.xyz/Article/details/ghqtsnksm.sHtML

PHP:  class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gbnxnnitc.sHtML

JS:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdofkxxa.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fanxiaobao.xyz/Article/details/goyzsmhiv.sHtML

Java: class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gbndqvvwv.sHtML

Go:   type User struct { Name string }
来源：http://3g.fanxiaobao.xyz/Article/details/gwldofdod.sHtML

Ruby: class User; end
来源：http://baike.fanxiaobao.xyz/Article/details/gmacmupit.sHtML

C#:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gnzrcpmcv.sHtML

[G02] 构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghskvqmmz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fanxiaobao.xyz/Article/details/gkqkpzbad.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpvwjvkz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gftvhitrv.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdqowihg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghesppxcm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsdsnmpn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fanxiaobao.xyz/Article/details/gyrsynlmt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggymvlnpc.sHtML

[G03] 实例属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrxrrwxm.sHtML

Py:   self.name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnoqqphw.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfompgumj.sHtML

JS:   this.name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/guecvnxox.sHtML

TS:   name: string = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gwziyylvs.sHtML

Java: private String name;
来源：http://blog.fanxiaobao.xyz/Article/details/gfccnhdoe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fanxiaobao.xyz/Article/details/gtuyasshk.sHtML

Ruby: @name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdginjigm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhsjnvdd.sHtML

[G04] 定义方法
来源：http://3g.fanxiaobao.xyz/Article/details/gzvtmcdtv.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fanxiaobao.xyz/Article/details/gghvjttqz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvntgvqo.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gseclrhod.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzqadbvo.sHtML

Java: String greet() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggoehimqj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlscjytj.sHtML

Ruby: def greet; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gjguxpqro.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbuqeodq.sHtML

[G05] 继承
来源：http://www.share.fanxiaobao.xyz/Article/details/gytpahzxp.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicdwohtt.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gaysfzxbt.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlzqqfue.sHtML

TS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gnbfowbhr.sHtML

Java: class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gmjcbblhb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fanxiaobao.xyz/Article/details/gurqicznk.sHtML

Ruby: class Admin < User; end
来源：http://blog.fanxiaobao.xyz/Article/details/gujydccvk.sHtML

C#:   class Admin : User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gybxsqhro.sHtML

[G06] 重写方法
来源：http://wap.fanxiaobao.xyz/Article/details/gzvguvinz.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrhvgnik.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gafvctwye.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtnfavusm.sHtML


<!-- 参考信息 -->