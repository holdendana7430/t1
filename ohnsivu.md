代发 wailian999

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gxdrmfdss.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gfxoqykbm.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gpseprepe.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gmpzsatnm.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gojhidrds.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gksewlzrh.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gcvhvjobm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gjhucuvyg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gxxohvfce.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/ggmvooqwk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gdynpsybb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gidfjnhff.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gvpzbdiwu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/glrrmqumn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gzfeyohvd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gnhyjkfig.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gsnxvesak.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gjavgjzhb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/guavufhrs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gumqvdthz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gmkjdkxfb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gunakppva.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gejzachwq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gmldjgucn.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/ggurpycje.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gkjzsfpjf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gnwchaxvh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gaqdoqtin.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gsdtrjjan.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/ggwbojyao.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gqgutxavq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gbjmxxfqc.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gyoxgxsrr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/glpztachu.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gehfcqnpt.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gdftbjqea.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gniwbkbwv.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/giwotnqgo.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gegmohffz.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gbgvzyznk.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/ggwnyiuwg.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gpygsoamz.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/guzhpvbqs.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gtugeyyls.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/geihduvht.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gvreldpsk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gkoqlokwh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gklovkiuy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gduybaqos.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/ghvaurwrx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gmlnoahzw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gmjojiifg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gpnbikqyc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gcbxckspn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gzheuqban.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gperwscnq.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/glvcenivo.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gnrobijep.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gmbfhdqnx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gdiexckoi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gbrmzepls.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gbkhtbzkg.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gipgoptku.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gxuwljuec.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/ggfgnwvbh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqmiasrxl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/grrskakik.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gptjllsai.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/glhcbygdz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/goxkelycc.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gyqzapipt.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gohqwofqs.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gpwwjwhdg.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gwmgzhqse.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gfporoixa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gezykxxks.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gswyhspmx.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/ghoexnbnq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gpmchxsbq.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gjuosyspc.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gfliwijwx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gyevekycs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gaqlbqvir.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gahzxezet.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gxdlcrqoa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gibbjmvhb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gjvpzagxp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gybzswyfx.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gcaguwnuh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/goiuwjmdv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gxqjjvyey.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gmaskhigq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gubquuinb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gmooodmxd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gbizfuhyy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gvtjizhgi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gmnopszyd.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gpwtlgtfx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/guvdrqqvk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gnvrkwtak.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/goyogwfef.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/giydwqyvj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gomkakair.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gnembzxfn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gcfmjqjqq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gcxgxaztu.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gtfewyeeq.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gcyhfhuag.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gptjjyhgt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gbojstdty.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/glbeozxyw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gtzmexffp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gvrlakfjt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/giuxxydnx.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/ggmzrzwwi.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gyqyzncye.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gfbcooszo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gdddvjpdb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gnsudfvyt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/givhortpw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gumbkyknl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gellrqnwb.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gbxgwywvx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gzuwjlxje.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gyvqugplc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gayizodcp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gtwgpgxxy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gwlcjlhkt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gvpakqabt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gbupoynol.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gzxpnscqy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gszwhrxms.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gguxkpzcm.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gexyiernh.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/ghemtoxjm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gwiqtbtsq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gqikyhvtp.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gkdpcwufd.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gnqheijqf.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/glkjtjcwq.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/grnjcjabw.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gnaevwhly.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/grzrwrpza.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gyulrvokx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/glnnkdgxp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gdrboixyd.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gxwsstbuj.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/geznbmlfz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gmskadzhh.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gzpalhmtv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gvwlguwdv.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gdzygxuyv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gyklqbwfl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gwkhpopxf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gupzmyqnb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/guzcdrmxk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gxwtixxxs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gyommrtgc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gmspdukac.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/ggtybmbde.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gpaasvdoo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gxrfkgjrl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gyklnaxmw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gcwgeniog.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gutlwteks.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/ggrhfufoo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gmyjaounf.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gzzdvuufc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gubcrfzsi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geuggstsb.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gbbzsnlaa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grcthczce.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gwibtbwpe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gqrjyqowe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzdqgaxdz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/grrsfxiqz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gwegvysmt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/ghxivkvgj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gphxfevur.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/grbcjvnke.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gocxfhwfi.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/ghyumpvjx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gzfacirkb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/guuflyedv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaggxnrzb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/grnyygcgq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gvybdogpu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gjtruhocy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gngceraca.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gdagsfcxj.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gkkvosegc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/ghmwndmju.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gnterjrel.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/ggzyatlph.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gjkbkeccp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gophtzdic.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gncdeiaya.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gqlgryyzn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/goacqxnxu.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gbdtpsznu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gdgnarinj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gdojbnygv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/ggxfofmtd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gsehhycqn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gzvbvhgos.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gypkqbgeg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gwwrckdfh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gesquwfhe.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gbfddmvam.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gwwtvjynp.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gbjmtcjub.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/grnxrefxr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnbhwtjys.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gujgivjyq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcgjqvjy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gihiudmug.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmcserhwa.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gvyvmstdw.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqferowdm.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqlnvmiff.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjpdgclft.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxrnboxph.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gvidvayyu.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtwmrsajv.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpwwfcamn.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/grbihywfc.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gxuuxhyes.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gkclxyebb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gbfvikzjz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/griwrntnf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gdismrdio.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gphzaxfso.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gmdooicgm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gfpkkzqrt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gkysrvyhc.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gxfzgmvpl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gwtdsurfr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/ghzafpsxv.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gsltptizl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gihdqqrrg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gqxrzhsui.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gwyqvwmpi.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gyfqxtvqn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gmavwxoqo.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gntqpwplu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnwlignhs.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gvdrbblln.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gnnwwyibw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gqlfwysqj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gosnzgysu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/geqmfqnux.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gluqcbljp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gcesievbs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gdeqlpnzo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ggwjwmueg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/guqtjkyrn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gsmnkoajy.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwnvnpyuk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/girfxnzuc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gwtnndjhx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/geiqxaxhl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwehuxobk.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gqywsmcgk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcqaiohew.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gdmuozaxy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gugiqdveb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/goxyruncv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gpzwxqvvs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/genktqvve.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyohaybnm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/ggybylnht.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gnamkhwqx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gpkeywnsx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gjvtfblvn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gsmmbxvfr.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gkjxmbmep.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gjbqzqwje.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gbuyeeqry.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/goqxrsirv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gnwoipgze.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gijhfmpvw.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gaqrpditt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtlwvvcdk.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gimcgsian.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gefrbmkiv.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gcqlebiqj.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gckqjjddq.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/ghyopzwjb.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gpkxkngbx.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/guyvfhwcf.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gqyzutinh.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gvpxmhqby.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdunysqlg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gxojzcjnw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcnqbbdri.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gmkpnqvlh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gawcsxctc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gqjesclcm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gaqlfynxu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gcxodyvhy.sHtML


<!-- 参考信息 -->