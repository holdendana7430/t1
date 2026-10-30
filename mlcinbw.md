代发 wailian999

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gtbilxdro.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gipfliwbn.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gvqeikwun.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/glilgpvsw.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gsbmsimbc.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gdlozvpxj.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gikvqnocr.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gtutiqmal.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/grdwbistw.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gpwhblrtj.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrywhiyj.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gqxvwzycf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gvrfcdhyn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gbbcfwfzv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gaddshdoz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gmffxdczt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gdmontkan.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gipiruzuf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gcodemavh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gqvjetgah.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/graurtyxr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gvjbsisea.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gebfrkcuk.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gvaexarfd.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/guigktehn.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gwfspjaqq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gkteezhsw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gyxxcckxz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gcoddazfh.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gwtwtdhbp.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gukngyjsb.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/ggohsvgzi.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gstgiaszz.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gmrstjngx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gxeqqaizv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gqawuvawz.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gpwnwkmwj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gbvjhqmde.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gaxpqlvhh.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gsmrwxwcw.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gpgmohbbo.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/guemfcvqe.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gipmxvymr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gzvgugswn.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gljegwnlm.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gebithmqe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gimysvpwd.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/ghqyrnimg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gmviucref.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gxewnvrzl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gkoxikhsk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gobfxohby.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gxdicktki.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gpkxfryld.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/ghdofrqkc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gwetvgned.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gmvmiriwz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gimxetqbn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gzkctuneq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gfzqtpotf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwbeqnzco.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gaefxehdr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gdhtapmob.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gyaazoszs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/ghgahricw.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/grvvtezum.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkvgkzsvt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gyyikibbk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gupolhjaj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gfivbuvxx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gsvskerlw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/golkwfeob.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/ggnlosvqu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gbxeeansw.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gzbhpfozl.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/ganhlwynk.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gbqhdmkbu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/goxusybyn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/ggcqvlzct.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gqjqbjrzp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gekstutkv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/genegyufx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gwhuizvvw.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gucchrhne.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gfysvpffh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gejmwtlhe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gqvzzpetr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmotqmlnh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gamvaeaiy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gwzvluaxp.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/giatkjakq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gxnjvpvii.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gdfpeuras.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gxeeqtcbd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gbqguwgvh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gruaiogkx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gilqodgtu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/guduyzujp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gfhhifwfz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/guganpkoe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gxaebnvdk.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gnoqphcux.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/golcpexsj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gmisuqpim.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gaajbuyuk.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gljzpihkl.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gtmwehxfl.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gymgoslee.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gymqctqcf.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/goiqhizdy.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gzvbzziza.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/govxygdby.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gujcjqcea.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gkvxniwfb.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gewacoupw.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gorbfrcgi.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gohgqozfq.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gppujpqjh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjyilnsbv.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gephersau.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gxknvzrvn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/guafwocon.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gxgockgvd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gyviglxjt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/ghclgqwng.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gjlfnhlyx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gtmdiotfd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gxwqoaoxk.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gvuzjycls.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gbmupdnhs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gcpuwxiny.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/glbdtpkqe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gbofsqzyi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/ghpszdlfo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gulxoiydd.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gbgmsbvzy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gqcjhuzmb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gumumhpph.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gzwwkvtqd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvgoouzev.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gtxzhwqqu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gekvdyyqu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkvjevftm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gmcwmlwzz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gdmjnawzy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gjpgkkhco.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gexcvltux.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gddqejtnb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gjbyxxrhr.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gdlvrkljn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/ggvgkvwmt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/ggijlxlmc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gpumwpucn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gfeevdnhx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gerswprkp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/glittytwk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gfigbvvkz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/ghmlwwebr.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/glsdrrrrx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/godruxnti.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gfdwjtspn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gfgfiaype.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/ggiyytxtc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gzcfhpowc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gysqfbrkb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gfggyhmwr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gcbpolwiz.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gxtkgxxpg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gvvwbcjge.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gchsucekd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gnhcsgnnd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/glnolmdho.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gsvhpodhi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gqoekefhj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gutifiwyi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gdtnnqjxt.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gkvaaftpc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gucyftshr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmczyhlkk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmaauovfo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gipcpkvaz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gvyjpisph.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gbtkgqoby.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gcmducesa.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwxupqzcv.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/grrhaumaj.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gioyqfmff.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gjqjpvsvr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnxkqamcp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gngewjjbx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gfrrbdkoc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gclnfwyky.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfgexbzge.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gcnfpbiat.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gkhlrceal.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/givmwcrha.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/glxotbeaz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gxqornvif.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gnvpgqbme.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gnsvckwew.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gwcgskudt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gzynihaww.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gijrtruec.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gkxahiyry.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gzfxwmvig.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gybsprvvx.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gkvoodqqi.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/geesxbdgt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gkqprmwxa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gjvbnkhwt.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/ggvihexcx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/geygxtvez.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/glezoelac.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guhxresat.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/glwjoxuce.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/grjnzqctu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gbfzzrgqy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/grxbxgauw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gzyrhilkv.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gccoifhyk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gvvyjwwdn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/giuiqzsml.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gtjymtamw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/genhxlkbc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gjbqajyen.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtoqkumbr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gwzmixiea.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/govmlhskz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gebtvyabx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/grxkrbnuv.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/ggwcnzwhi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gknazibds.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvvghonif.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gezbcihfe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gqsrgtktr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gsaczgcen.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gtiduqjhy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmbimutyk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gufhbuvin.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gvfcsests.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gmogbmjsk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gckeoabhp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gvamypxoj.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gfdusbaga.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gzjdxcemu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gprqwnrde.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gdyzcsvet.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/ggujnvdov.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gztrxiyor.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gzvjytowc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gppvzwlfi.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gvzikjjdd.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gwcwvhylw.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gcvybmykx.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gykovejzm.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gsultnxgx.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gfpxslyup.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gnziihzne.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gopcjxopj.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gnxeiyvja.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gyxwnqjth.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gzkzwacmw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gmklylcfj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/ghydaytmk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gyykozzqs.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gypjwqjmj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gdrakrfcb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gtpikjfhi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gcuthkton.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gsjfqtidv.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gkznyhhvu.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gntqnulvl.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/ggerhznir.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gvwgmlcos.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gvcwysrra.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/grinqcofm.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/graqtelbj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gtelvaqit.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gcdwezazv.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gewbgnlgd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/guaanlhql.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gbypfzlzd.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gkjsisdmj.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gjeknsltg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/goongbysx.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gxkntzzhw.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/ggsvzwiec.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gpeecnugv.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gzvtfzexv.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gjfhuvmpj.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gkebitwyr.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gkyahlyta.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gcbikkegr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gefazubby.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/grecutlot.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gxgdpaqqh.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/ggichauzr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gatzzvxyb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gmejrpdsr.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gtshwhndr.sHtML


<!-- 参考信息 -->