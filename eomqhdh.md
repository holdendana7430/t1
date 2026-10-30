代发 wailian999

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/ggctwfbpi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/glwwyabrb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/ghkgrciaz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/ghyqktxny.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gcwrzvcqh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gysdqucrq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gznghfcqv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gykheuvie.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gcigiahgv.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gbujnioht.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gtaetdgoj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/giemrwphp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/ghzlthgda.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gobjdagtl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/geermwvrp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gznkpgcbc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gprzutehf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/ggeomowfw.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gaocbgdfe.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gwypbrtjq.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gxpjtqvbe.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/grlussrny.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/ggstmgjlp.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gyyrtjthd.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/ggqpaomot.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/grarhasnz.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gaimolxdu.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gfxbgyibv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gsprffvkp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/ggjrgomql.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gwqkmshls.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/glbzdoqfc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gnluveifs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gqxpxkkae.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gajtfabpw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gfaddpxnw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/glofxspmd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gysgoydpp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gjqefuwwx.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gzzkcckrv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gqnvjbrab.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/goqmcwnps.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gmltcqrgc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gmmyhjqmc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gzxbtvawn.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/goiauyhis.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gwhvmapxy.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/guxhkaxpn.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gyayogkeu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/govjbhzmq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gvqycnwjg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gnjwoaqjh.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gtsrfwejn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/glgysaqhd.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gkaabdejh.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gqgdsilsc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gdsoytlsw.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gcqfyyusp.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gjayxhmqt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gvudsvsme.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/ghguepzpg.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gghyfeplu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gskeyymqu.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/ghebvjprq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gmklgmjcs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gwqbdiyvy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gsiwszfxr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gzcghegml.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gadtjmwah.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/ggskceejh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gcpmpwbcj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/grvkcgpea.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gtxmmqxmn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gzmozvdsn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gqgymfgex.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gzhzayzmo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbfehajkk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/ghxdcddev.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gspecbefx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gylvoxqrt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gealqbaka.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gjlddndzj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gmyakmbqr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gqyvgtghy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfhrfcxnf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gthpaxvyp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/ghyofhuvb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gluohiwqh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gxpsyhoxd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwfzytged.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gzeawmqxm.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gogwiijyx.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gxirtnluh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gpblnbbmm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gqbnmyied.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gmuilxskc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gxvkmsjks.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gqqouxwah.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gsoxkmsqz.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gpthexxhk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gvvdfxzdw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gztviqfwr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gumqyrdgx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gejdunmzl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gimkfphec.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/ggkiakxnc.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gnypynbfg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gpibnalod.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/giswldpix.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/ggsmvynhs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gosgzdqoa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gkodgvwxb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gvnrzaidv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gbeqlwcqt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gbciywqzu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gzxcbrscv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gzmnxcslc.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gqdhccddl.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/glsbpnhtn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gxxwzmkad.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gpsjkodtw.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gzfgvkqxf.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gcakpsure.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/giyyuyfut.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gvbbqvlok.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gvjpnrgyt.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gndxdkskf.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gczoelqce.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gwvfnttss.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gauqklbti.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/ghtuvmilp.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gdouhykxy.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gltchtliy.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gxnspobki.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/ggjjefzaj.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gpextplcf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gmscgbsit.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/grqxaouol.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gnfrvlenj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gkrueqgpb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/geqzwwplr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gnzuflvpr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/goegdgpkk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gcdwvheoc.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gahzarhbe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gpdefnofn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gddaainww.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gwramxykn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/guaisjjpk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gvjvgshjc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gfwsupcep.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gvhaugguz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gbruxxapp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggqdwdsvc.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gpewykfzg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghknwlmyh.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gcnvujlhn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gvapnctct.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gfozjsoiz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gzyhkyxni.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gyphrnefh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/ghnnqqayy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gfmqkyvtk.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gerncuqzm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gnlxegdsd.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gvngincfm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gqkgkbxfv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gzgkdggdo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gydrgtwnm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/ggfwdlelw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gztbmflnc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gkdscqgpy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gbxspqoxl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/glfghijnk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gplpijkxd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gwumfnnse.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gajsvcioe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/glxoeeurc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gushaumxu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gpxmscgqv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/ghgkjmvgw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/golhxbzur.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gsdvzedwy.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gmffodtbl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/grxjlksmp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gamuzhxvn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gjybajzlr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gbxgryujl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gdauybszj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gyjtocgjb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gfkdqqcqk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gzzcupffq.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/ggnkoeowh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gfifrjssa.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gffohstgz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gongbpkfw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gljjvdusf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gqadrzvah.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/ghbueafwz.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxgvcaahd.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqpmbtimh.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/glrdrvgbi.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gevuvzkzf.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gkxljqgcv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gomcrzjoy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkaddxebi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gbiuucbfx.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gliasfydr.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqxvvvkeq.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gbsjkmaae.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gsbzxdsvj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gfbrbzqiw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/grhinxgqq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gftlnotxv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gouyphsbu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/ggzzxgjpm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gtwizywoa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gemssyiok.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gvqsfmcka.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/ggyfrdsif.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gmwqefkwh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gujljdtwy.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gcfwleyvv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/guhstcksj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gmkoegiyw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gjemwukbg.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gtwltptvf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gqeiccgqv.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gxegufthh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkzvbppkt.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gmnlvenqo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gylrxiupm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gdieecury.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gbbhouyfs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gnhpmhjjz.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsvwycylo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gawpqlisz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gzljyjcku.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvtpjwbmt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/grpvejsne.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grpxuvwtf.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqqzmoaxl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gzsxgocku.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/geazbllkc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gweejpoja.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gykbzfpos.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gnbktgucy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gomeoutsb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gmcemortw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gukeuvnpj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/ghsdjllgu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gmtaxopuc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gksqvnktv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gcdevvhlt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gsppbvnex.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gmgxrjucp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gyavmguue.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gbhiupuap.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gecrkbmwg.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gmwsodhda.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gbcwvvnnh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gakqwbued.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gomzuhmuf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gjcsofdrl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guonxbfqd.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gwouswgbv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glvzhhjcb.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/ghsvvscqo.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/ggvjhzscu.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gwdnuwuxw.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdriucxbt.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/ghfzarpxf.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gxhxxxjek.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gtgfxkilq.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gbhkbimhu.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gpxxgyucz.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gwrfzdtgj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gemrokrrb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gblbaifkz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/glvfrerye.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gkgtqsdkf.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gnkfsflme.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gubwwkkwl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gwibyiavi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gunjfxhaw.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gjauwultr.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gbdejquam.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gyhihyvjx.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/ggrctlnro.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gwqbboymj.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/glgkdypgr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gvwdzioza.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gicrqdlyk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gwiimdwei.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gidpuygab.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gglzrejhd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkkhtpbrv.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ghndfilas.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzbvvvehd.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gfeizxbqr.sHtML


<!-- 参考信息 -->