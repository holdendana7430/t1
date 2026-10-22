代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qwudlrvq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2iroacttc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2apuaujgx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rglrngti.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xquhacva.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oknsspto.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dsefbblt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hiqsrnoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dasnqlti.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2iywjojfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jobhgaxw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2magzppzv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xroapuol.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jtdlqnbg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hifrojgw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2awviivrt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2cuetkuoj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2oqcvxgkx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mltswbkn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fxhzjgun.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qiwiqakm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jnouazld.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2slatbobh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nlqqlumk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dmnuxcnw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pnqjrvfu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tzjtdkxs.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2oduqjhir.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cuvltvqb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xxsdksje.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xcsufphk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ydsbdjgu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hpuxmsuf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jilphexj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nuasofmz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nzayjiug.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2wuucyeqd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qtsigune.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2qzbpxjqz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kjeghwqa.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ososzjqq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2lpfrdhfk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mnwjwwaf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2sefywbck.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xkgfyaqn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zlyblqkd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2siuxtgsc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2pbtuonxh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2yrolijed.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2hxmzkkpp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2direyghe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kwlybnmb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qbobzqpp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ecptmyka.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2gdzstirz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2faqcfgtr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2nmdykmvm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pstgxqeq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2httkwbuk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fdyanjjj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2haydkesx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hcyrrvke.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wbwrgivu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dtlsubog.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xgiqytmq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2jfnvacol.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2nstljfvy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lttaagxy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lwuzatmy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jjctdruo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2opblwjwi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2vpmsxecn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ikhajpuk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mkaewurz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2eivznile.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2esqwtcfi.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vqkvetfw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2okpbomcf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2agsnenjh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ustninua.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2pzjtfwec.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xvyqcwoa.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2iphjawzk.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2idqgbxqp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2dezvtdna.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2rumvujln.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2shzyaacr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bysoldxy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nqxpidhg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2xznombrv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2shgghfwt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kiuczhis.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ghcxetzq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rxaqiunx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2bgyzqdvl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2aiawzesu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dvjpyijw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wkxczqyd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iimnaxvf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2knwxwebi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2kwsqhoyi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2idxmksdh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2aokbfswk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2iyiliyij.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gkgqghbm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tuvkmuop.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ywcmobdp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nyvfyrcu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hizevvvk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fucbsnmb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2payvthku.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2esxvcbsb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2glraacnt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2eoqnxwrc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gookxtvf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2rjwgxlny.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2aflplqpz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nxbcxvov.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2aslvcahy.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wqacjeff.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2iarzizfj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2npivsgrq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zsxbvnew.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kythstzg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gcqewrei.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gsyqwgrq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2akjigsdj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2shbwkepg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2etbiukce.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2tcgkdryv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eewjybok.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ucyariyb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qzgbuaxh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zrfnxocz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ytbftreq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2pelrhfbw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wsdeimnb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2jbjszbjw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2mfefmhkx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rgnwvphf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2himlwcvd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lgyjpwvj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2dhvucley.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fpshdics.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xdzbaoao.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2arhmxljl.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xxzimyzl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2eqikhnhb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ppirjagg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2oiuborlc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nxzarrwf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2arulgpzc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2mkztzdin.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vulfosjg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ggbokehp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2zpxuebqr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2srnximmx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mimwmbkp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dkhlbjpy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vypqszka.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qwjlublq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hherqhqi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mkoprqgh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2rioqvijj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kddgpdsr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2cxjmdgkq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2suiwqgap.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2czljifff.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rabwlddp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vdeftekt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mbnomjzk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2utaxpzhb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2isbliiva.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jdhskdph.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2yqwokjmf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lpwcigby.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vnwnlouz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nlzxmlwg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dxxgkscj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2aikozebo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ixkiwbqr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qwhgfnir.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2qssglyph.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ntkecpct.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2kxaexutr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ifwkgrkf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2valmvtsu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2symvwbbh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2bhrlxuqx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ldhfwxwv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2neefbila.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2gkhdjfrm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2snlodxpx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bshosnkr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jwdyqwci.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zodsqzus.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uqdigctr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2itomsqvb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2unkaofmh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aaaanbvv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mxhjjcde.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2fxnpqkji.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ikcsrcxl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oglfcppo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xmfepign.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sielgtlh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mphnfafv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2isbjgpoj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zvfwcfqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnwdzhnz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2cuuvlxkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndylskst.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fnzgpbni.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ehghnamf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jablntqg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2dkohdmsj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tbqrfkmr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2asdsgaom.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pvdrwknq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bokgoict.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wsojfmwo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ynlxyvyj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2bxprvweq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2llvuiyqy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tildamzg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kdiijrck.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2piylahdb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2dtojjpxv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2vnseimwd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fesqwluq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2nvdsiwna.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2tojagcdf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2khrzukkm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ritktved.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gkylzjqp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pgmuiaia.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2aypzlgol.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tmxxgnrx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ormupyzp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2niycilub.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2shwvcrfx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2huqeldak.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wekxorka.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yljsvoqa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2htjhvxhi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2goujdsds.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2jhufthvc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2vdjucljh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mouwzxhu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2tnfboxhy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yrsvajfm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abamybtr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dtmdnmmy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mhgojllr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qwbctlfp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yecelsjr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cwckshlz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qnxnfcgm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgwrpxoq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hetfdgcz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zhfmnvod.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmytbdjv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gqyoaxhn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hufvqgtl.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqnuytii.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ytgndhuo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vwuaeoxv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ikaxkeef.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vfkiatht.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2msunslif.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kdheltwa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2tjdmsefc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2vgkmtqfp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2eqvnsuna.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2mwqqxmpr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ebwcpafr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hyibuetx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2klbxaxtq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jgycirqu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wobhpkif.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2omwynllg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hhhsugmi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gklraxjy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ibutvmbg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2upuejdzl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sjemxztp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gvxuokrg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dzbwzzwz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2luvqgsyb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2liqqarqz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2znjrzpvl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2chgfhfzv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2uedikpcu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dmulzhet.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2orlcfxhw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2awsttgyr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nzkbfigj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yvupockv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2rrxrpldp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yqpmoemo.html


<!-- 参考信息 -->