代发 wailian999

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mmtwogsm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pqaucvmv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jvnthajo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bemouhkz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3msscjikd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dpdurzvv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3nakkxoai.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zmlvvbnj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ajatnrnp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sngzfgmz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3wahtkskc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3djjllghg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vmqsoggd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hhdkitrp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rscfycor.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ddwkxiem.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3btxtitrc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ybsecyec.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3oabxxqat.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wylnxnpq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ormmtsyx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3hjtbilno.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3odgmspzv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xmmfrdsn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3yvvplarz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ovnctfwg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tsdvkkjd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3emlmsyat.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3tpwcehsa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3byrjkmwi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wfbbbims.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lxvrnter.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hnvaswch.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3xragpjrx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3msfngosn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tlcvzhss.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3vgnfhiyn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jjexkfyn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ziwedton.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dnuirqvq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lyfzlbxo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3leeuiyhp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ycsmzkom.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3svcktfhf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cxwszqwo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ssbigjjb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ftzzbaeg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jwqivoxv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jvxfajyi.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fhfifucq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3bwgiafpw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3purjiuvw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3bcqmceuh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3itpismnd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3siysnnce.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zgyveqri.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3lfbpjqah.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kptrnnok.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3aoaflwhy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qexydaqv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iyxiuixl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ufinexjf.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wcuqsddn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3sslacmds.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ibiulgwb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tbmicmpb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vhjxmpwr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3izdttlxs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ubliyzoi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3qmvdjjvs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3qxmzsolq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ttlspxar.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3cxrhxlez.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jzznnjkg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ysfhyine.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nyxcqdmg.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3utopqdtx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qqmjqqkj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3erpqgvxg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3terkfegq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3zydetfhh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3qlhhpjgg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ypgadzdf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xafhrcba.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uvcmkbdp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fxsyufyx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3hxmdemtu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3utpbkzja.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3aivjppiy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3npeqwluk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3tiangeqg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dwhpbovk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3grohpkyf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jevivoul.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3sjglpwce.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3vgucpxun.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3nusxtpsw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vqzjcsbp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hehiztvj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3roghivps.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3iocohhds.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3pllvuqsl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tsxfsbtr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hixxmkfg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwnqdxta.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ayfrfcon.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3glxhuvai.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bcmehuxg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3qbvouira.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3vvldavtm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3omgdoeic.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ttqrhnrf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xamhmjcl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hobcuvta.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kframxwe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ewaupcaf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pxjuaixc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3fnvbfvcg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ogzafxsu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tkkhosgj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwjoidig.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3zlejgxlt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3wvtayyto.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3tdltdmgu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fbwcjfeu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3stobysyp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fyxylhqo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3glfulhbu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3uliyjqqt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3valczkpi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jbfljkaf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3uqeyklce.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zkyygeal.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iuhjjwdh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3fpfugnyi.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3armthfnh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ggpafxzj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3lqztlrlp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fniksifi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3flqbjafp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3yigydepw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3gyqebyuw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lwoywbxk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hbwdqquo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3kuiwxdfg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3xjgpdznj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3fslfvdey.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tkhmiqax.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dsdxeoij.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hbojmpne.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3urwblkew.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3amzfkfpw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3sybtuqrj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ucqpgefi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3bljwwllm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xxockcbk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lnndbrgt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wjoeixpu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dbpyturf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3xmsnpcsm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jppnksgh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3mxbkggho.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wfsyaoky.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3frtsaidz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3yitkjzjd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzycqjhv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3poarymyx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3crhuabon.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmxsgzza.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3imzymexl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjmygolh.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3imcpuwrf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3mveeskiz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mlkliyud.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hzbrrzfd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qbmrygti.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bsbebmin.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3pbovglws.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3plurfdwl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mkfvdfrv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3pmfpjgdg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjtucjrk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qedsavea.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vyrsbhyr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xnigwekq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ebqmcrtx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3gviqsuor.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3eiwzaqxr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jwjprmjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxfjdrmm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3offbuekn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekzoepxw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nklmhlfz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3rzyjbbul.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3udbaugjz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ojasbyhk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cavehfel.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gvaihstk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3syvfqqip.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jejdnroe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cbdqpjxl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3hkkumjib.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3qnosqyse.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhynhcyg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nersexgx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zgzhyeom.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3chutewom.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3dazgbdbb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3euuxhrlj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3khqymzdy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3tegwxuwa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3amthwsyw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bwrbkfsc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dswqhdpg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yveyhxvc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3odkdahju.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3zyouqoiq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mcymwoot.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zakheyls.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3pcsnalee.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qymppdyp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3glecgpvu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lwqrctrd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jfijornt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3kbgtnkof.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3usfsuydf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3vvqniyhn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ftgdzfbi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ozfcdqso.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3rwpbdedq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3btxbydci.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hierczka.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eavyviat.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pihhbblx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3quqiejyn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ozgbhpsy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bnysgxcz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3neriwxfw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xciqtdds.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3otggdmhu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bhhqwhht.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wpmlhsvm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jcnnirbw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hzuukmwc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yuhowxor.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3djhilpqo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3tlwilneh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jqyicadr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ugnomrvm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3yhaewzqu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cngglklc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3fyiixvmy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3uzhsgazd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3qafkbqiy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ohflwnfm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3lbgcidxp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3kangqbuk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwkfgive.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wosjxvca.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3brjalwdz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ihpebekf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3lurcbxoo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3upvfvedw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zbfxtuuv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3tqcmaalx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ewlqyuqj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mmcswufe.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wjlffptg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lsuxixrx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fperdetz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3oertqjcf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lrtubvyj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xmbkowkl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nnpzwjgc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbxdsmvt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ozcsdhld.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wtzvoxnt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kgfyojtc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3pbfoxqiz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3anogkimi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gnixynlm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mwiwnums.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3hvoamzup.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3itvnbtep.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3lbgufnjw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbzacmrf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nvtosmuv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mpmdhfzc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3mcizioyn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hizurule.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3jzhllmgs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3wslnkocc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3dpvjkagy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3pxkvfsal.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3sdojfdwv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3qzrqhoch.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3kfzfqgyu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ppcynjxe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3sozgnjke.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3hvvlripz.html


<!-- 参考信息 -->