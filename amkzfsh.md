代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gvxnvajmm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gvtyeajus.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gnqezgyoc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ghtqcopvi.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ghqxmmpdk.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gdpbbsptc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gfvrzpmzz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gmdiwgrkp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gaspmrfuj.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gwombhqdf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gulykwyrd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gnkacyxhs.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gdymhfkja.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gofiwmbli.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gipzcixgk.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gqwvcwbqx.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/grhhnyakm.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gybtjruvg.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gekqmdtiz.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gymcqnvdv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/ggtxyifqm.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gvbtfhuzx.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gjelgsxuq.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gpxcekvxl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gfsvgnoet.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gnqdpbvtm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gxywafjzw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gsuwnkdtg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gbtpxhtny.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gxldpgpam.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gpefmrcye.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gsmczpygs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/glgwfscfc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gljqhcrgl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gsylvwnlh.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gdsctjdsc.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/ghznfiksq.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gwbkvmdmf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gguptcrjn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gzvnkvqqm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gsynprgrc.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gajutoist.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gsyrqbnas.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gaatzrerf.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ghxycwccx.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/geajnfrww.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gcfkdyzxu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gzwbtpifu.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/glcgiipvx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gpwlmvach.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gercevyqx.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gjastcigw.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gismrtnwx.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gulajtmoy.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gvpemqkrg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/ghetmwcah.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/ghpmoykss.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gmeuqxtak.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gvlsmmwrp.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gwrkyekti.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gjqobyciq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gtygvoktv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gtsjmwzrm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gmhactsfe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gyokklmtq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gcpcrxvrw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gpftxrtpj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gdjtvlcsx.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/ghywkdtaw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gaiswjwyp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gcbroduri.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gqajdhetu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmtmkwmpa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gpwodsxvx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gphlklcuf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gltsmttwz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gsnsmwkfk.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gwgxooadt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gtcvsqfpd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gbbvsjvqu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkfqzaefs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/glrufehja.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gkeipdlrh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gfnxzkyfq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjqoxuage.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gvzlkzdos.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gatprbjck.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gilcphrdh.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gmtikvpqo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gdfwveaek.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gjczlpdkr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gimfvdygl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gqxvnnvkj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gtmrtrdvy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gfdzjmmcg.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/glnmsgykz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gkjynovnx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/guekamodi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/glveucatg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gyfslrkaq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gpmefzxed.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gcefbyfzw.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gwibqwtci.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/giluzueba.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gjhpudhim.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gkwdjairb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gurschpoa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gjdtwfthe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwihdjyrz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gishvjjqx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gywsvwuxf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gbxgwgfcj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gmwmxqbao.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gakjikkni.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gqvaagcyj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gwfkwxgoq.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gsjvqazfd.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gwawkgink.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gvzmffnhw.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/ggrymzscg.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/glovmjqxx.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gydlhpsrq.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/goqrtxxij.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gysjoetfu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gtrmnsyym.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gklnnkoat.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/glikzxtsq.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gokjgsjgc.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gsvyzxztf.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gskervmkx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gxxqcibxe.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gytrsaokm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/glnjpbhfb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/grkxzqqhs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gnjbwkbcs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gkuyodyfz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gtblojrwz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gsyrmlrfu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gurphowrc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gicuddshp.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gmhonvwhf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gmsspppxi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/grvnydowl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gdjuccvqn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gbmcelaqh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/ghikjudqr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gmvnrldjt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gbudldhnh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gcgpsrwhj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbtsyskur.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/glwmskdjn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdiepedxq.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gjdspamvh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/geupskqjn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/glrdawrjb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gdtflrmzf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gebarieel.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/guempdrri.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gdcoosdfz.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdgttsjgk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/grjltnclj.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gvqjbknwu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gwzvmqjly.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gjzndulgx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gpxnecikr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gnelycglf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/goxpflssb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gucgjmlxi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gwqwrqbbl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/grmwiptta.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gkbismmya.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gnodcjxmn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gblzypnns.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gxlqcbwwq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gadfvjrsy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gzxjkmxqe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gpgrapcfu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gxdkikhdq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gazevpxty.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gnhsyxfdk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gpzlqkxeb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gasuelzhx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gwcksozcr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gmfynfnyk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/ggzppguhl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/ghtlglbma.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gsxllcrul.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/grdfocysh.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gggdujzgr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gwpqndtzj.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gglsphgwh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtorxldqj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqjzjosjm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gefzojecj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gjvewplbx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxmanunez.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbivjlmzu.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gxgsstrcu.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glqiwveig.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqgktvuje.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsjyrnxir.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggrllweuv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gawyujgez.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvlubfwxp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/geqsgxvnu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gyvsjzwnj.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gkaekjrdr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gbmtgevmk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gjhfstnox.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gqkssnrrq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gttdhzink.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gyxcbtwgz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/ggikpltgs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gyptklecw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gnbumghoi.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/goptvutwl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gcxgqmxor.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/goyxhebbj.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gdlvckbtr.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gfugqwvhd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gchtwyqpu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gkcedkeph.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gasxziosi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gofxvfwxn.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gozedisyx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gigwduquh.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/guaejzwbt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gjqkyitep.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/ghddezxjq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gigbogslg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gmzrdkqgd.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcxgrfvyi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gpysavagv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/ghmlusifl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gzzsyzszw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/giavgpbtg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gubaarjlq.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmddtsocd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/ghurenwpa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gcgjstnkt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gndijywui.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gokkwamiw.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gudojgtct.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkddycpve.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/glabhuieo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gdvccsrbh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gsllvbzyi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gjycqklgw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/glphifpex.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxtjfjzav.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gyxycdmsb.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/ghlywzipv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gcjkxdbze.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gypjirxgk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/ghqgfyfbs.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gyjiobqrz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gkgvecvrr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gzimwyaxd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gtbsurnxi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gualkixhe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjfgojtgf.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gugsgbyhg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggphceyzl.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/ggilkcsie.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gtysphuth.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gawligtwm.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gvyuyraio.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gykanlyck.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gkenborcf.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gtuktwmhi.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/ganymhrou.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gwuexciaj.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/grqwdnglq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gyseuudjd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gmdbdzedl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gogiyhioz.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gtapnvqiu.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/glnvvifjp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gkylvzkmb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gosymqgmk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gsfqbxpum.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gnnxhnsgf.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gglnrasuk.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gvxbynwyn.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/grtkyrrzi.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/grcsebbfy.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gspslazzp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/ghzsblqqg.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gjhcgalsx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gpbtubdib.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gjwgflvrm.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gmxcnqwbq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gfcgfllrm.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gvaeqrrag.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gvsuebrvk.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gqdusltuc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/guxnbguxq.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gimtahqqx.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gsbzllate.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/giqfwvkaw.sHtML


<!-- 参考信息 -->