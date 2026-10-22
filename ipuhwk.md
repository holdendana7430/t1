代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2oznocyax.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zobbajav.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cvkgudbi.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2shfdgjbb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2acdwruly.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kkqdyydj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ejnubqui.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jpvdkaye.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dmbkiivw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zsomvwve.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tfjpauhh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ercrhpyr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ylfmysbx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2weasgwyj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2dosqvsxe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2opkrxwnl.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ulznhong.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2wbywlzdd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2eaaprpoi.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2emjfvaeo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2fzvmxisd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cxmppqqg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vdgkysxc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2biyholqx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ojjpypbm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qwymoljj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wruasgfp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2btgzcszb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xlhczhtd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2rxdtwbtv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ahcnpgge.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fmwhehbg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2izpwtrgy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fmclxpdx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ncyonrwy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nqijsygr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sxhgnosz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ovdfssxq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zijjqaib.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zejmfwdm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hikapoov.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2sasluuwh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2fgzfucxb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2saqgmujc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2eyxxbrci.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jfbsatvr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2bgkjlqqq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ohafmewl.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2uxtkxrmb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2arkaphtf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qmmztcuy.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2jsbrvcxo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2xzexaqpt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zwlgvdcx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uzisvizx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jraklzde.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2fqxoaohv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vsbbkood.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zvpdxgsf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2glvrcfnx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kwycqrvb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2aikrzbel.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wfrteuby.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ffgkvbks.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xrfuqbgm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2tzxmzjbr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mgzbyfcf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xufpdafc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mcukipke.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vrnxdnep.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2qjreipza.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jfsizlvf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yqbwoyks.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mgazyoqn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ounwrvuw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vjrcwtcb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2vpiuhtsi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wyuzcsys.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2arkwfdad.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2whtihpdx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gstkgrxe.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bfohqcal.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jtxdctwt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gcoleots.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cxveibza.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jorrvzyq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2znavotca.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ubliennv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2uhyltxot.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xpaggfmi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jdahvhau.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2vbxtkylr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2krvexwrb.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ijwstcsn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2bljiqeeb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cxovemmu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2uftelqin.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2kbglvcrx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2grommgkp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fihxzecm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztduhbor.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ylafdssl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2btvrdgvu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2plzatfvo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2wfxqrqin.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2gomjcrsx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ytddkidc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2zhywfxpf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bqdblhej.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fhlegkkn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2shticghp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2tdbsrwda.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wxhswkor.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2leyqkyib.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vrjhqumu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hvrlznux.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bihoeusx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2kxfbavaa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xsqdujvn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rezuwzec.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmwedhhd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbpzsxck.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sifuvvdp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2anwkhpai.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2xyapskyl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2evdsunip.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ebsffrqy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2yvrrromp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vupjtuin.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2kaabvaen.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2kqbgpcun.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2gthlnegd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2uihepxox.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hfhofkyk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hxitfbrv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qoadwfzb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yjpagqdh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2vuzdtebg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2oqpdjxgr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2krygysmv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wfhqdttq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2zjiygnpt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2cowpeitz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jfoekllj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qdocpxup.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wvhhlndr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2flazhkhs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2yhgrvium.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lqbwkcxz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2pijukzbv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2dutjeptk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xtdvpdru.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xanccrts.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nfuprmiu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2xvjiscpj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gdzrhluo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yeknmxfr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2nvbajjar.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2bfhqqdcq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kmsohydd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2oqavhjlq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2qmksmrzz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzuhoqva.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pstgavdx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2hujjqzte.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wkoawpff.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2wgnmfgpu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2uvzfcdea.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nxljaqzh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nvxoprsm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rgfqwfwi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mxvvsfkx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lqbkzrrc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2youcymky.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mjjrshlf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ybktztmp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2uipflhyi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qvgyyxia.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lnukbmaz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cesrnrhf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wrgkduwx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nqmugmzl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2eulpofgw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cphksxnm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2sojzyypw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhjwwmzz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2uuhjtpaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygbkdwlb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zikukdti.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2fhmhjfxr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ouedpyxj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2sbpjekix.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2msuldaag.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zpmsvvti.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2zysupyki.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vzwjnwfn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bnofpppp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2bbyeexxj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2gskljxdv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2dicrytfh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fedpthqz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bgwjrewk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zwgsocto.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2qbhfnjwc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2qtqfhsbc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2qqyxkymy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rjblobmk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2muiwwkvm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tjeihzrq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lrhrepzm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qdonaiup.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rzdjtyyb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2bnmqkxxi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2yesnrgjr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zvpvdsnw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2myrvucco.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2svofugya.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vbjjxqbs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rjnasziv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zfmugbom.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2fruupdxn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eypflzsf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2xfypcvvn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2snyqbvue.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2zadjxyxn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2unpmrgiv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xhihgmie.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xsosblwb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owcxklrd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pycbmqac.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2uhkkssaw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2somdzkbx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2byxvflwt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2yqadwxkh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vyospuso.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vvmjabqw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dkgzkiaj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zctlvehs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iejnepjm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqccokim.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snaokffv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lqrpgawc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2hunkzheg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xvzfslwj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2iuryvbfd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hzwbhrbz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dmldafkl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2nnwmgttr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2uspoxeul.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jmkjnqxc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rdrllrlh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2vihkzqhp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2xkwkcypy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmdpdkjs.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cpnlcynv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hhowyuxr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tojubiub.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2roozqrdz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2cmidxxni.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2uecdxver.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wqdicazt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmvhzjeq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uxlrvgnn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mqqbystc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mdqwhpsj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jgtfpkox.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gerbnfwb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eajogcsp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2aifbmjwn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tolvgizg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmctpvda.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wlefgshw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2npkxollq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kbnmwmwn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2howfodeg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nngrahee.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ftwamczl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aaejujlq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2oiqkzqdc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ordnvhag.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2nxxzaegm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lbwzshag.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bjieivgv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dsuchvdz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2fyrtkqgw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nihdnpgs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hpcqslkp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jogmvbpe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zdzssnzp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2omqkqsij.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2cnrkwfnh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2lgydjuxd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2epvwyxuf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ytngcdkq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tjqqpfvx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2pgehjuxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vsbwahoj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2voqvzmlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkdpsgka.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2crndtnxa.html


<!-- 参考信息 -->