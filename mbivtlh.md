代发 wailian999

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/ggmqldzmx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gyadpnozg.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gcvgtskpc.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gaifvmzdo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gajcbxpws.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gkzfvvbde.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnsfoxbkt.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfrzdhsqi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/grdfwjvqc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gbaslutpu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gelmueabc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gyedhidej.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gvfvxmlvk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gxfwatjac.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gfovlhzai.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gsvjgmxni.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/ggzfdntrj.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gzsdlhlwk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gjvvwatvv.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gdphktteu.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gsmeoxpla.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gropmvczu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gqklwrzgo.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gcfdszhah.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gmakuktvd.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gknikyota.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gfrmnwshk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/glxkdykba.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gxdhgkvuu.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/ggcvwyiqy.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/geamqxmmy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gwpbovrvr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gffbtavbl.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gyhhplhwr.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gbhxherpo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gxeaxruja.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/ghikbhrbo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/guacrnquv.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gqvbwjznn.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/glyehwshg.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gzltnnipl.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gqyuisrct.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gdwprqnph.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gjtyoyial.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gahoqqpcy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gtiyzfade.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/guvcfkxua.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gmmwmduck.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gcxcdyuya.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gzftbxnnh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/ggbhyqeqh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gwzfwtiqi.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gpalqekti.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gevujfraf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gxsyfpoaf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gllzeeujc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gvygtffnf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghxpszlkh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gegvggkcd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gsxamaxbu.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gkbduekxe.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gjftmcuvt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gsbhldaxy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/ghvfnjvih.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gxoextkbs.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gtpfqiqzo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gzkdhzprz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggokdmrwp.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gfhvgnxyk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gptsqzbfe.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/goblckpol.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gndjwgajt.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gsfliqzfr.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gazuqkyga.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gqeqcrayn.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gbloznlgd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gsregmobk.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/ghticyeya.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gtbdyjynd.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gmwklajbo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/glsemcofq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gsjcdtklo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gkzrzdmfj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gjzlsxhel.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gqzjbrnct.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gxalqnpvz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gqoklqfjb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gnnxrpwbe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/getyjldon.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gydippxca.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/ghhwzjlmk.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gtocphhal.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gzstvqgkb.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gbyxngmdn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/ghvmqudrv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/grwpiqbwj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gzsrfpdoh.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gaehqtyjg.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gdgylolsh.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gldvujjlq.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gspmdwdfx.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gytdiiaxl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gcqutnqzk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gwfyefxhc.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ggladixvx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/geybkfova.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gglhpfdxe.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gfeszhpbq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gjyzthpdy.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gqhxeogxv.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gpasltudx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gvlbxgbux.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gkwtlqvzp.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gzsqnyapy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gbbstlkni.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gpkqponti.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gtvtpyvsg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gbgyhgjyn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gmfgjmifr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gnnllajiz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gmdljxysv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gxitsjgia.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gfvfewhng.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gwkrymwoq.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gwimgepit.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gblzwvhiz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/geodmmztk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gameholud.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gsfbokjar.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/guruqtecn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gulgzqxtv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gtyybkpvg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gblhxudko.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gbxeqqmbs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gofurvods.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gawcuigal.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gzxaalocd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gqsykaxdl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gbyroxsop.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gxegvchyr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gbruazgqo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/ggkubzkjn.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gksrinzoq.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gqgidrlrx.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gkyndfkxp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gcinoupmq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gvomsxqmx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gsfthfsvp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gtqmamvov.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gbzdxonuj.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gkbwgzcfi.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/goaterplm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gqvxpwjzu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gqannfvmu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/ggkpvbrwn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfghywlv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/ghbkvrfnj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gnmztlxuv.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gsgfamyzr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gldhvnizs.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gufcgpimq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gjunitfzw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gzooagkja.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gjysabbdr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gimjrbfvt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gcmtxgyyi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gxidvslcy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/ggakbznyf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gnxsawaja.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gwlxvaqtz.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/genexqmpq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gfqwtswby.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gjfysnist.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gjpafzseu.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/grxblgabk.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gzkweeqko.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gialsbwnp.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gxgmcwuuz.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gsegkbksg.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gsvcwmkle.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/grzpzvwkh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqkuntyjl.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gszpjyuvk.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gyvkebelu.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gdqdrvuxv.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gtoltyqdd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gcfarxaeb.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gqfoqinfy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gwbwfneej.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gkcabnrrd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/grbpnuwtg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gdemxeiju.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gpykobemr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gfljnmpyh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ggidlghww.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gxnkeoeoj.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gnzuywyht.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gbonkdqdj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/giqanuvdd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gfhdxuufw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gymichqho.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gmtqrhvkc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gavdmjolw.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gxowcxfql.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gzxyzbmft.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcgxzajbb.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gwbiskzqz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwnwwxsos.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/grsylchep.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/ggerathel.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gpgaiqgpq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gpwkjjomk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gbfzzszpl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gjcnqtmoz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gumiwinbw.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gitacuqxl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzuxmflnu.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpcxvnlwj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/ghltqamfq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/glzokyxqb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gfhnrdnet.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gavnhpkrd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gtavvucak.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/ghpohbvsf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gpdrigeiq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gfjvnrlmd.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gvvdcdfax.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gstopivsb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gzbqydviz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gnimomghi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/guzowzqji.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gdmklxdvo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gsbepxohd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gbejanvgh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gwcyxrzwt.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gehdxhtvb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/ghlcqluhk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gxqfviafg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gxhghuabd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gkloukxjz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gljvtzuzd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gzkavvgnt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gtlkkutak.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gbsdgihtt.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gptrqocht.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gbxrdbmga.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gathkqfnr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxufknras.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkjdfcgnd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/galwycsxy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gsyuzqjlq.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvvonwrwb.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gubilbiuk.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gtdkpcqnn.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzaznxizw.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gbwwodhug.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdbwxvwac.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbdphubcj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gmwnuxovy.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbfmhwhuq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdivewpga.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gxwqfntcq.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/guatsnifk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/grubyempf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gjiefdsrv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gtetcfhjr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gtbzyuiva.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gtspvqvaz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gfnxxspzt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gefgfuffj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/guauhzwai.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gshhywyxs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gomjbcshc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/galroubyi.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gfslzlhtg.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/grdatkxcj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gpymlnbka.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/glmwlheyw.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gxppwbqqr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/girembvyo.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/grdilhrvd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqsasyvql.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/ghgiiuqec.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gizirmsth.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/giokntxeq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gfrafoter.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gmwjptkeg.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsqausixy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gtvbrnqba.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gseqpqsmn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glxeanxwg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/grzzbikzs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/goutjkyxe.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glkasuihi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gtvrvkzbh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gelumibis.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gfkywiwyq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsafklvzy.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gzeywyxjm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxgydamgj.sHtML


<!-- 参考信息 -->