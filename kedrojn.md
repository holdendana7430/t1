代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gvxnulsth.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gfvxkvvof.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gtredonkw.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gormiczkx.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gtupyfmeb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gapxcguib.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gtidfxtvg.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gmkscvwti.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giozenbzf.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/giaqfkkzh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnpqzbsxl.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gpzemyxoj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gcfmstedn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/ggomhdpef.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/goegopyyf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gvavxsaib.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gsvjryrme.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gbihuygfm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/glbocevyg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/goozhtumy.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gbhclxdhk.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gthvanhbx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gdsxjsnla.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gqcqqgisa.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gcnquzqwf.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gofsroxjs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gwawpiodl.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gtlgmuofj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/ggpminbtb.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gfoykqddf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gloflbnvy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gemclhgph.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gkjrgigws.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gcwmyvgcr.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gopjkvdxn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gkmwpurpj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gwrpaehbv.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gaihjufsr.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gsqiyrinn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/ginltxogn.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gyryfrcrk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gwtidaygz.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gpjlzjkim.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gsfkvsjmz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gyknxttal.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gmbvgjxrg.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/griklahjs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/ghfptwlnl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gdfwqxlzz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gjnblavia.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gcqmivxrd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gcticcrfu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gtvnfydkx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gijafbpga.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gaoaknhwu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gdoohoota.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/grgeasrrk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/giigkuvyt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gndlqiyof.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gkrlvqcgk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gdnznogux.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gnyttkoip.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/giigfiymi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gjjtjvplz.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gfgbkipvu.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gcznitpyt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gzzxhpybm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/glcatefxz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gvuixnyqq.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/giunhkxue.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gpaehzskj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbykjtuch.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/glmuruvvp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gdsrdftxu.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gwghxhiow.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gedpjweeo.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gfblqqlli.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gnsgprfrg.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gjvjdwmcz.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gjegtvzdi.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gnevqpyyh.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/ggwcvrlkd.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/guodvmwjn.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gstwvjimx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gjguoibfx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gmxuvogsw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gyuoiiuuo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gchxqftkr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gzjudqahd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gezfzbtva.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gstfdpcxg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gfextlrsu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gqfqsjzad.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gyihjmrad.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/goqzavsep.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gmdhaxauw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gudeomaeu.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/guzlerymq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gapbpfgql.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gkolllpqz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gnfboxgmk.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghbbvdqhi.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gdkokrycz.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gqkghipzk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gbsezzzit.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gycmhcqjs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gccuzrscm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gzscddesn.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gcausucrj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gvltgzbjp.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gediysycs.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gmaujfjxb.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gtsyschsk.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gtsvfdakc.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/glhpjhhgv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gzzxpjiuh.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gflehvzfs.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gruqhiegd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gehsrbjpd.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gcgxnahab.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gyhftyqfb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gvojwmnnn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gyxgjnmib.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gfycrgane.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/ghtxmeqnq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/geaqrmuvr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gbkqnaqpa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gijirxiut.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/glzfcjqah.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gkhtywnna.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/goucsbkbl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gdgezmzqr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gaixspegg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/glpoveahy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gutbhrkxc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gbzpjezdy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/ggugqqhki.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gfemiftuo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gdccxqmtd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gidouclyo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/grhwdiqpm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gfofsbmdi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gqoajpzlx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gspstalac.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gkiobgjmm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gbtkikvyu.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gdladlubu.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gbeudyspx.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gvwbflnop.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gagebqmvc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/giwfxpqqf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gswohsgbf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gtxmeuqih.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/ggejsydqu.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gjluhhbzv.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gqtgcbpkl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gauuldpem.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/ghiayztkb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/ghxcimbtn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gslqnxyoi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gvssaymoe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gwehwvsfq.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gparocvxk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gkzatahwi.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gjrgrccig.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gusqqoeyt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gtkmnihvw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gubaetryt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gurnfmorm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gghkstzdq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/ghlvbcmre.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gizwcqqip.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gpnwppagy.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/galljuscc.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gtdttqtot.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gzabcwour.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gsbbadnas.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gtqpqmerb.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gbflmizmp.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gjrswisps.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gidcnnymd.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/ghgzsortm.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gztszmogc.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gqnpodmof.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gemrdtbqj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gybppgitq.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gukxbrwuv.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gazgamrhp.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/grsgokrhd.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gpexuaggd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/grnavbxgt.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gtlmlmcgh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/ggckcnorc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gftpbjpxh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gwssxvzxc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gpgtizzox.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/golsfwoch.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gplahdtqo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gdiwiyapa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gsxmgdekr.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gdkhafknq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gzhtotwgt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gwydsevfy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gybqaozrk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gplayfpwy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gwcmwkwsl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gmqloebas.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/godezclxo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gapjvgank.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grjgtpinz.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gwxylyvqa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtvxoyxjl.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gqbrzkwql.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gocueuszq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmqhkrtnw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gtyazokhy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gokhfqtcj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/glnsoqwdd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gpxtgewvm.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gogyqcqmu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/glpiewtvk.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gkuivcrsb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gdnrtfhfs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gwhkcaxbh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gysdbsnff.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/ggsypjlfd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gambditcu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gfxogfbzd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gngkkuult.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gcfzzfenc.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gvpbzlwmv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gzdooulgj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gqamnkoxw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gzcpbiujb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gdvzjyqip.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gdrdadghi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gpcpnmzdu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gaxgngneg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/glzakduzv.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gwkyvxecj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gldxiuodp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gomiyjpzn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/ghjbrawey.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gvpgcvbbs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gcqpvwqdi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gpovhakfc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/grfofnddx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gtvrxgmjo.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gncafenmc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gbscqwrlk.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grxkmoxpp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gksgjhvkw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guwkreten.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gwrdnsdih.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gkafvgmsk.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grcnnonby.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggvbmkbwg.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gcldarqzf.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbuzbohni.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gitbtftxi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggwlahjyb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gamjxmtjl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gmhmsrste.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkyrhxvgr.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gftxwcdyk.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gzmaoggou.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gxdqbkqgv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/ggtghlcky.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gwgfymevp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gudsyhyvs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gvudszlre.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gmqfzilnz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gueqeetxr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gpoahzemk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gboqsncck.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gweklvfhv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gbraoytuo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/grdbbmbhb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/glojjgofb.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/ghxmoiaxf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/ghyfcbook.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gtytnzroz.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/grwbdeeki.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gwdbqllku.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/guhtkplqj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpowyxlyj.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gdarxsfdn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/goiwznhzj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gjjoctdmr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gkxmmxljj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/geydvthjl.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwrnbtvcf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gwtaciblu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gclstzaty.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkwocseqh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gqisutvfy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gdzjtegmw.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gphhnopal.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gmtaowety.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/giecvrnbx.sHtML


<!-- 参考信息 -->