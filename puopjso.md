代发 wailian999

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gmziuxsqh.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/grkqgtnqc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/ggprdwrds.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gutavggvw.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gllujdxga.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gtzaaglag.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gkcohvgex.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gubcmeumc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gotzebpys.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gqbnfpbgi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gsoephqvn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gjkmxajsy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/giyhcuqnp.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/goytzhsoz.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/givitcnfw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gezqfwrdi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/ggohorkjm.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gchnppyaq.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gldygouoe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gzxtcsvve.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gwjbbyuox.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gcehjsygc.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gzbevxxbk.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gexogkdii.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gkztfyyac.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gqvfzapxh.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gvvjnxmgp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gomsdsorz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gsjnoeshf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gwawpdxxv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gqhpgbsqu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/goigaukmk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gphypiwho.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gavzzqhcm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gxmzlsaqi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gkfpggaoc.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gxheybgdj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gpgkiiwsc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gjeurfosq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gqghwxbhr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gwzkindxn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gcpaqcdfp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gievbtdvv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/giohfcekd.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gdrgqchqz.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gzjztmpgo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gpfmvghnz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gavwdrwtp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gqlykkflv.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gjhrndwmr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/ggtbarakf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gctienhfw.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/glpmiiseb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gsoohvrds.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gzisfdulu.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gfmzvbwny.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/ghqahmcsf.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ggsmulmtb.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gdlqlhuhh.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gvqdkdfeu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gwijjmhfl.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/ggmpkbacx.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gwqftggir.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gwswxbmgv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/glfdmxxsd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gdaorbxzo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gnygyezto.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gfbhnfybg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gqjkypmuv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gqbcnkpkg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gilioilyr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/galpvhsds.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/ghhklkrrs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gcpqihihv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gslmfcuja.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/glievjdvm.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gbtraayki.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/glzvjqmgr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gyaofsegc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/ggriqzkjo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/ghfnyfsah.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/grmxyhpmr.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gnnicqpss.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnmbamwuo.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/giyzimvbr.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gxaqvabog.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gymmwlkyo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/girhzixge.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/guvmmmjil.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gmqpdveaw.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gpdtvkexm.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gdsxqhjsq.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gclcodlgn.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gdavmizsb.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/ghjvjdtnv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gjvhwtblq.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gogsxrryu.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gusjtlfnj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gavyjvdjt.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gigiekepk.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/glfevkutd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gtxyomlgm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gvnduomxc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gbuhayztm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gzemqtwrf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gximyseqd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gmldbqhtt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gyfbowncz.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gvlkwpnni.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/genbrcpqe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gkwgdbgtq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gjhhqyntm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gposqgioh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/ghwhjtvsv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gbnipgpqu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/ghkggdjqc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gyepbnqdx.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gfhuadttv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gugxmyyem.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gcbtvnckm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/glxxicjdu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gvogavumw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gtizsbpfl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gvjcitsms.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gugklogrg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gckesrhoj.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/guyckooyd.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gtokhqabn.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gpijlclhi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gwpdanvgl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gwmobduoc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/ggculenki.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gnswnroob.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gdycuibwd.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/genyifiwd.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gwpklziqq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gtrdptfzi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwupgxlfa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gqktxxzjk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gywfrjsec.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gftainoyn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gsiamfcmi.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gbqhtqzec.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gwamenift.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gdupgievd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gwcgqkcha.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gwldldcfe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gtpactesi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gjyugmgub.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gyysjfhtk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/giyvcwolb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gunfgkhtv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gprhnqjsm.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gdonpmszb.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gaiywupbi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmmclakea.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/ghtxpgshz.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gytilmhkc.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/glitqoytg.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gyjmurhkr.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gnoonauls.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gcrggofvy.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gtxkjgowk.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gpumqjeor.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gzydrteek.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gjpkvkxda.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gvkfgumfv.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gqkdojnay.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gwzjsdsio.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gpycnfces.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gtzgydiav.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gvoitjred.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gstwxznun.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gyupmmlte.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gthsblbcp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gyutgnanr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gaeacdimh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/griylrfka.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gaepcfemb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gosliolgt.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gsjrxgzvk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gykteapwx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gspyirvlm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/ghboeunav.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gfkmlbomm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gpwvhkplr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gykuhjmrw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gdnfuhdbp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gaxlzdegq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/govnhrajw.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gtulrebpp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goepvkqxk.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gyekzhsor.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/ghahxodyj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/goenkwdac.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gnrycsrrc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gblyoqyfu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gsrtvwcfw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gyljiivcz.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gayxxdvgp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gtonnelnd.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gkmunkzjm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gmswbehwz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gfhmygooh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gpctukjkr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gupcyxqgl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gfvsljdlb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gqrfxatzh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/ghqsipoca.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gduougcqx.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/guszbqxpr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gifepxgel.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gstcewlku.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gfmxcryxe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvgavcax.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/ghgiedvyo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gtwuehbhq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gbhaavhtv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gtdekxalr.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gzyfgjqgr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gaoixvscq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gxqrdvxga.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gqfeozelp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/grxfcdfuj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gnwcbhjyo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gbcyseenc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gocbajcql.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/govtimsqi.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gpmxqdfrz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gifbszdxt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gemsjffnd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkmnqbbbv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gflkwzfkx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/ggahkxmuv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/giizmzdia.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkrrrdbyj.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/govwhchvt.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gkrgrysrx.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqzhvdgzi.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gyxrnrdjf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzzjrcjox.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjszadesq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gevtpggrl.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbkdimaji.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggrekcrja.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnysajrmh.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gcceffsup.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gqogkklvy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/ggizdlbdc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/grwymdgrr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gdfuygbqy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gxjdxgqbe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gvhgpzdhk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gpdgvnyvm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gtybaxshc.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/ghzdaxvsl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gncrynfyg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/grcgcthfw.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gbbkujqbk.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gqmxoqqml.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gcuffpdsw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/ghbgmtbvn.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/glatxielw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gokldtxcx.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gpwuccskw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsdlpwabo.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/galhqzcxb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gqgjxpggr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gpdgcngew.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gjwscqfba.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gbhdfrchm.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gflglmvmt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gvvykncgf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gomepfhcp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gplutccqn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gpijlgkpa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghewnrglx.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghbpirzga.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/glxxoyjyq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ghgiucycm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwmmownba.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnrridihe.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gqcmjbpgw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gzlqjnyzx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmhqtxosl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmvbqycaa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbshcpzup.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/geljboswf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/guanblpjw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggtxkbyez.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gfxxxnguk.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gjafijfla.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gcgmyynts.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gcmscegjs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gqdebfskg.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gsqqhkypi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gdbopvblh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/grwbyusbc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/givrmreqk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/glzijtmlj.sHtML


<!-- 参考信息 -->