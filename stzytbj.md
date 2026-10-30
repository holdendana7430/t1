代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/giqhiqtiu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gqyctsxyx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/ghegtqixv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gggkxnufi.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gjsunfakd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gyznbpetq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gfkuxyqao.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/geuijowov.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gnasxitau.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/giplchbhy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/glistmrvn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gbslmwgnt.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gohfnjcid.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gnashqjpl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gapowsgta.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gtzvbjojk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gbyizijpb.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gipazoqfc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gkjbvoykr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/giyxwmyal.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/ggrfmtdvv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/grqqkeepg.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gjmbnwlfd.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gqxwlkfmc.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gohqhxeyr.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gnbkshads.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/glimsshhd.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gbqyyljhw.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gposhzlvo.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gatepwspt.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/goixebmxl.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gvvprydpg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gjaobrwpo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gajtonpml.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gozrejsaw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gqexzfjkd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gniivczrw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/glgviflko.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gjhomxryw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gwmocjyhv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gdefyowwc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gkhqdpigq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/giidlhpbc.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gwofckyuo.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gjohpuyjq.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/guglzseuh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/ggilkrihv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gnhqhbpvu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gaswlfoiv.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gchprzodn.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gwbdojiax.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gamgxwiza.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gnzkdarpv.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gunhbolcs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gpluxnpah.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gzvwrfptp.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gecezpinj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gmmdmjbik.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gsxhueldh.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gnabkmgnj.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gxuoebyzg.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gypsfaiem.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gycgyrdwc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gzulbkagd.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/guacyyyyi.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gpvbtdxln.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gtmblorft.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gywrikcfc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gyoxbwrcw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/goxgabwgw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gguwtyfxx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/ggztkgfrb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gdudcfdwe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gvfeymcaa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gqguktwsl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gjwfucdsw.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/ghlseyabd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gmdullumv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gpwmxkhzv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gwazejcfb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gobotzbah.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gywuptvzm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gzqqhwkzr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gwquefzkl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gpsfpurkp.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gckiapapm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gzbiwrgpj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/guccfrfvp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gghznzqjs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gdipjfgle.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gqicspiif.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gzytklypu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/ghkkuzgxi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gotttkiox.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gpybpobbz.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gqhtnfmle.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gvrijfxwf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gliijrchx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gbqnpqdny.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gjnovgowi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/geazfywqm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gpnkdsfxg.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/geerykmlz.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gnbexwwro.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gwwwqxvdq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gcstxjgri.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gepwuczoz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/grlqloops.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gdbcgfipn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gwbmnafqh.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gbhsssmds.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gviqluaad.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gdcsollqf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gbmlvfurd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/ghozpfmaa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gdjbkgwku.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gvjqwnfui.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gnxwdvdgr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gctggadyh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gacrgpzxj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gkzgmqlft.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gclzaotyy.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gytexqzki.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkhomokun.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gknxouvlq.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gavpnzqrp.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gaxfrterb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gnseqkgad.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/ggaenpcyg.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/ggbmhwnhc.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gfgjzcojp.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gnjdezeva.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/glefvhcjp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/goqxipcov.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gttmvytvf.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gtevkrygo.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gagqjdydv.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gpvgodzgx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gpfjtgsjq.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gnmtarxyy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gvegjnexh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gugcqiind.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gouygmdsl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gstjblgia.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gnvggrgna.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gsxdtykah.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gcpfcusoy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gpmjjwonv.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gnmgycvvt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/ggbbnuiwf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/glitspjji.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gjmeldgzj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gqhukinqj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/grlowdeve.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gurtuavfo.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gfjdonyrv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gofrxrnxg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gawhvxhfw.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gddhizwvh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbpukrtcd.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gjnycgdbd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gwtybnthc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gmkusagvr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gbepyihmj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gcrrezhnt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/geeergham.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gcwsckiai.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmbuvtkcm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gzuztouby.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gltnavmqg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gmcgyiwmj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gasuahivd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gkswvxxmp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/giwmiteum.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/ghvgiiwnq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/ggrdznmfy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gwsfcnovn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gylcewlri.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gaxbyeauq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gymzeqeet.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gjxnngegl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/genkjowsf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gglgzecam.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gzaciybcw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gizlafxgm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gryalulqs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gjpgitfoe.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gstddgsnz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/ghfjkfgfz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gxrnmiotj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gjagpvgmd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gsbxqdzpp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gulkzkito.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/ggupyciql.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gopbbdeeq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gpztumfxp.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gykazolcn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gkfcoggpj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwhkzgmru.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfuglkdrd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gblcxptsh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gdlziqgin.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/grnofccbj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmegmycqz.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvlfzsqqw.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gvupvxihr.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqlkxqvrp.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gawpzmvak.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/goikssuof.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqqevlgyj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gwuizfnvw.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsueqanpr.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsyitligq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gadvlscfs.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gutznwglk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/glnyddpyl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/giklycxbt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gziivyqbr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gmfwhfnoo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gytuxtnqi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gpqenvtjp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gcjykdyyw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gbwfhkqyo.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gnlozazve.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/glkngktrm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gkckhhtif.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gkhguijga.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gmffawvzv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gockixbcc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gowqluaro.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghfqcrmge.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/ghvsrpqlc.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gvdsxokic.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghqjiqflw.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/guwudadvb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/guymakppa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gkmzkxhqx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gazgjirls.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gklwxrejo.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghykyfhxm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gsteqzrnk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gnoztbhsn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gajvtwaac.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gvwdmtbxz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gzrsfkjif.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gloyzherb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/guvoohbnv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gldmerjrz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gakoqyljr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsxzgienp.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/grriecktp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/grojbitsb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gyapofazx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gavmfxhkj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpfxwmdlj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gauhacvfm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gzobkvuca.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gpzmbxqke.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/ggjavsros.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/giyqwbarf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gctpocrxw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gsxqucyvx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gptollklz.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gfhrpmpjk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/glofgzrxj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gigjevddm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gdmgprmsv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gxcmgqkyi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gblhydgeq.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gbrgktknl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtthqtwhu.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gscgawlnp.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gbiysnhxv.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/ghxrmqxbe.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gdmcyucsz.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gcsguwstm.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggwswgaok.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gpjkjduvl.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gsfcsgghw.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gooraavbl.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gnuasokqd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gphumoape.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gxoovjvqq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/giynjkkwz.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gzvrtzyux.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gcsmtvggk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gqozhlnzx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gjglykcqh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/guzhcrwxs.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gsjcfycrs.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/goysrwxdv.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gfepalmtt.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/goehpyjah.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/glommznlr.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gpojxjofh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/ghxpkfbis.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gsaqftfyt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gupthvfdz.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/ghxzizbub.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gajkszxpj.sHtML


<!-- 参考信息 -->