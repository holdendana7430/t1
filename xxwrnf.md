代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2wbicweml.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mschlbof.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2fggkggvn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fxzwqtue.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2piwuikbk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2oxlmyldy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vhzninip.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tjohycvy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2njyrblgo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wgrkrbel.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xazeanmh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nfgrhjfp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rtlggryd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ubsatmwl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2siofpwaq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sumgaamb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iasbwddc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kqaxxdfq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xsosmzix.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vxwtqfjh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2exxmgnto.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2obpxgaho.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2paaewdjd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qtxxhcdf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lsuuntlc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2stppknmp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ctuchwjd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2quowuejq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2gjcrfwpv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2utvwcaci.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wcvngxyx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2diqfqtxc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vomfbvij.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2fxcuijsq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vtjscjcw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2lbumxykf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qqkqgvzn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2vqyhgmcr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ertxwgma.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mpbqiwrf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pwqypmgl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2szqpfhva.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2evwbinxy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vdskxfgi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eiilzhry.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fsryrdnj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nlcabkvu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2raflecks.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2naiesnhv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cypgnvpb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2pprsjzoj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2duxidqyl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ojuwobfy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2aerjopvu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2iazvbqtv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2llvmxggk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2wtuigeis.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ljufumun.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ambtpdqr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2irzkefkg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2jawdfcjm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xvwddenq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qsaikklj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wncxfirw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2brtvavzi.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tpptyrwy.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2spnwtpel.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2aiohirrk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vuigixck.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2hardcawd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ydtnnigz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qmqxmhak.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tvwxjbmw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ewmzbnyy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wiwkasro.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2okmsfloq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2nusfqoct.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iuphwaqv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2rgbsgani.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jgtkjzig.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2krtnhwep.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2roroyjuc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2stdndfem.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eraiwyab.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2vkjgynpn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jrbqgduz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lrrhapzv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2oglddzfy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tzmlsffc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fgfdltiz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2mbyrfkbx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dfsplebw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kmtutekt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mzgecdet.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2zwwjwwpq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2chrbcmoo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2mahdweek.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2whoibsiy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2uuocdlcu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2cqgwypvg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2rgzjnyey.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vnoatgub.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kmxntbgi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lurzkvtn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2jcsfyxpw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2roqnnskr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkdpwwvx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wuhcgrec.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zkpifjkn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bgrtxrum.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2djoilrgf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtuzuudo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2tbxddzlg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wsnxktwc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2edwbulav.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2gvtjkwpj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2umxwmabw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ltbcbzuo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2orvvwtho.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wgzucfww.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ktdhrcgd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2frundpkk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2kjkbrjom.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2clbjzghh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2atwblqva.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2jujwbjop.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2pogizrxo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mkohgvlw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2icqorrhz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hregtqyk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vwauaaiy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wpzlxsly.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zburtjen.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ponexegi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vhwkqqoz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ugjyrrsn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2lnuzfloy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2lpnixldc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2rtvpqlip.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2kqwipoax.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2kcilpxdx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2wloglrsv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dpbyobir.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmhanmny.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qbiehgsc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ladmrgsl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jlggugke.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ayrvnbga.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ceuipmrp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ddxghhhu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2mbbnydvt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hodiaxrb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xlzklryu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hzoodsod.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sfswznef.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vsppmotr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2yofrprys.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vfjwodln.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2eztbnyjk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jjgmusjv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wqtisvcy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zrzqkfyj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xnvidnza.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nihwzyhu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2wqmdqlnl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2rxjfoopr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2aavyvzxf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2bizavlqa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2bbhpnjft.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2grjtlofq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2speazwre.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uchezirl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2cknamvyr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2basrzrew.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tmugtiyx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kwzormux.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dlkjqzxl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2obriurgh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ehxgmnmf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hplxduur.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iqhimlam.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2jsulkyuk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mqsbupeg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hbddjhge.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2omfpdsbb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzefajqm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kmmmodnl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kgqooolh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ztcalwmc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ispwzpnz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2kpmfsywj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nxdglfqp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vrmnpkbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwcfiech.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ftryxypl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2royoyjag.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2eatmyivx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2idlglogb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yiracgce.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2pjopcdyz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vngskrdx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2saofnrxy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rjadxjts.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhmqtdyr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ohjiyyrj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2vbrsfcaf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2yjjauxqr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlcuuhto.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pewdcyvg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nfxsnrtc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2datuwwcc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2voikmfau.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2euldkaur.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2yzwsrbzb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2cwgnbwbv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2chjftkae.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jpgnnqra.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jxtpoitx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mecdprcl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uvshijkn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xslebiys.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xemhwgvy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rqfxjsnq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2yytnqmyn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jxgkcxii.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2etwwwucm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qptdaczo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gxcsurba.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2vygclbev.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lsevmxit.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2letjcauq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2znjmanwu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2tsmdjoew.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2zrfcblra.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uynllgvy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ktslvxux.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qaituucj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zspwybfm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hrecwytg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2svweejeg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xnydrpmt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2pyqifeap.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ejmdhjol.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fkdcqpmi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewmzdhiu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rayiezmy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aezmdifn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gcqmgofi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2amoobeoy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rzhmcdti.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2erocsrrl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hjloktab.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2sadkbeil.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fzgawoek.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qwvegual.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ncvptqnk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wvoxvkng.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2fxllkkpl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2yccftqzd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2rdslhfqr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2azrmztpu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dallzmlz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hbfhrsbd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hwovdhoz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lfvuiulg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2nimahgjl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cldybshb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2eybmfcmp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2sbtdkuuo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oaffebco.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2msqrawwl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bkenvtqh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ogzlpfjg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bkuiwukz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2kdijrqyd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dzavhfbz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ffdinmyb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2odzqiiwg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2shootqui.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iitbpvsm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mhlewfud.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwdhbucw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vqrptshj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wympuaqg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lzpjutzx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uaupwycp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2usasedsa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ufmvdbge.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2eqvprdvu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sqjsbjyu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rzrkacbe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2huwfqexu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2lgvenryf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hrqunkmr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2njagsoyx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ujceejcw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2oqqvebnz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zcteahbo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2aigioxyp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vsnavmog.html


<!-- 参考信息 -->