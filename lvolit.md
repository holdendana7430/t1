代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xggxlzrc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2evrgeyir.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2vqrjhjni.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2easapqqh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2kgvyuwnl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2upzpwpkc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2drgwbxyd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gyvgqgfv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wporceop.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ognjygmd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iryijepu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cypfbzrm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2oqkmqhch.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hyodxtsz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2zacajhkn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hbtafzuj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2obrkuwjj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2syrzxiac.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2icqngrnf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zuzpzfew.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2eqnybrqo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2veidpthi.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ujldsgoy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2osnbgost.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2gszcrfuw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vazqezhw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zvhlnjsh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2aperesue.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2rmvuknft.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lixtcohw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dbjqzitr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2jnxvvswh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mrvqlsgo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2puxklehd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wxmamxys.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2udzzwerl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2clesvlkd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2aommtufu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mfuwyiqu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cmiixdme.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2kqwqcqsq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hulpzrnb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2dwdvvvxh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nslvwzrf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aqkghqdw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nzyybtht.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qhovutiq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fjjcqqbk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cbaepyem.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2uwxeyiqk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2drirntzp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jxeradej.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lliotbaf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2swvrrzka.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2iuwjborh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbsaqhkc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2vuideydb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mzfznkmx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zutcustj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2okvnovgz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2phyctjbo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ierrqnvg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cfgnacbf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bkkwkaza.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2csphbugl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bkvtsnzw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xpvaynnw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2naneguxu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hukgqylj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2zcbsodtb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sjvxbnor.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2oirtadae.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bzkftedf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ncfmiorh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2birpthuv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2onxwbfll.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2tuhtagnp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xflmgeme.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wdmxphrk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ymrjseou.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2strqzjpu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jhonpqaa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2aazysxxi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bnktpqhs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2dtrdnleb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2nbayqwji.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rcjcfrcm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ixvdhbtj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2homnfgzy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2plbuxybm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mylnmmpq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ibbilbpl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bzaxczum.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lkhdmfil.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2gzjvirkc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kslzyumh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2tcejmpcx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ruocfdbo.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ernlzjks.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2txxedalh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ehbleuon.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ngdjsuzp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2azihwvzp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vvjmkttv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ggiihpiu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2dzcochfi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wotdaehe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2utxvetfj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vblnmqro.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2tnvdgakc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2bdxumhbq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2apjdwkfo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2lkkaudku.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hthkvgnr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2owmcrxud.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2fumlpzzh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fjayrqld.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zzsofavm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ugcyimla.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2tztcnbrq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dgpvfzcc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2vfccimyt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2dnzahkdf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2girydigo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ajmtvqxo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lfchuzyb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2pqenxzsu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2lpswdaat.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2kshbbuyk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ukbkjkmr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yltxechy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2iqkzmmxo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2opaiotjc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zgwpgdqd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ygfxmaku.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fwchxoco.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2uumqnptj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qavxyrks.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ebudirej.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2hmtbsres.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lceafmgd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2rmdcszzy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nuruskyq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tvmvjumb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2lhmygetw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wxxvuixv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2tfdnftlo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2vsetmave.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2qvkmnbgz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2sqsjysub.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ogjajtzk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yousxthk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kpvwhkct.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dyicmvzq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bfldbjub.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bryjlrkl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wqvkxpib.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ajuqdbbl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2mjijzyck.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2isuepcpu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zjnuqolk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2snfikjbh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2tjqdchyu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ypjywpba.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bhebspmu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2zyywwhnm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2cscoqqzv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2dyxedrjs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2njdesqjd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2msekwccg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2elbexhjl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpqjwfsi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2siackzqv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vobbmcns.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2cjorsrvs.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2rjnvxhkj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2skrkubda.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mklyswha.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2onypxfde.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xforujbx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wtpnpvxm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ryzfuonm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tvkedkdw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uckcsjdt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2vegcbdiz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2epglwxui.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ibpzwhbj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hgjsxxbe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xiplybwh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2acojgklr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2cazlnftj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rdbdsglj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2padwezph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcxvkvko.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qcpuglgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udhvfgzy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wypqhslx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2hcokhoha.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qonnmipb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2rtcyrugb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ruvybzww.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2azkjlflf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2jndgivpe.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2czyxtuvu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xqbmvsgw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wziaaqdw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ntrcfhdl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2cykeaefv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bejyziyl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2uzbbwyeo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nmgkjjng.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fbusjzjv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2wcyngjzi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ukvqmpld.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2gnoojgfi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2uqhmguzy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mbztrnut.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2euyzmxzf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uguwcqwe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sxtqsala.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2zsrxezqu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2nkjuawaz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jcsbnmzr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2aiqzdefo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wmrolmsc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2rnnocycc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jigpidhp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2klpycnfu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nzksdkyf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tzeyowbk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ttxzwgkx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dheqfuxo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tnaaacln.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2avzikcgc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hrxwzfcv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kicmouep.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wzllqeds.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bgntcdwd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2wlpecekx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhrtvens.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ranuqlte.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lnwhbuvy.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wygnxxli.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dfsurokn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2umafseha.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pehyoxoq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hsiasquh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxjrcrnd.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xrzwyvrb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sbppzyop.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2cxdssosm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hqisbsqk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iwckeeyl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mqzyktik.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mudgvskf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2yhcjorop.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2xjyqlkoe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2xxtfgkmw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2iazmhckk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2yzuphycn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kgkprfjz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgdfrsce.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zlewjspr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wyaaxwwk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cbjirxtp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zcyfswnb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vcfdhoeg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2uxozgpsb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jbbwlglf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qcmwklow.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uykxxlvb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tcmfawmk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tiaefrye.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2flmytkoy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2bnlhcbvy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ikadplqk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zmorhqmz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2fgdngior.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rcdjeaoo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jelfvsgx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ftxdnqyh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pdidrjjn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2uvmbaapl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsavwgki.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cjxyrids.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wrvzaouj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2nwrmxiih.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wxcanhxm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fsxaifkf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2czorcsjv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hmvxctji.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nxjckmjc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2pyyihcvr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddyaqzns.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fnffwdww.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rhuslpxb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2chtwtzvu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2cevtzbcw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hbhyyqzz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2homdhbba.html


<!-- 参考信息 -->