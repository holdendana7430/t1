代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kzwocufn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3njnqrhly.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3qfeatmqi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cfylmypu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3urasvbrn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3sjfmneft.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mwkiwomh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rcybyrwa.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ckdlmcbz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ygkvjfsf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3oneovgph.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3owgmunsa.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ftfykekp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xckqygry.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3udecupek.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3allgccqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nipqkone.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3eyzshtde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffzjbozq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sbpreclg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ihssdkkp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3iptseezs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fijgpoja.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dapqqtrf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3iqlabngn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3tlmtgyfm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qjqszllc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vhnodpqj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3djlixkpg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zkwbhqpc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xybfgomx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hbefbzyt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wiruhmpv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ulhschcm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3khcxstga.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3owzdilzd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ywsgaxrc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kwzduytq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3qciegsfh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wdecliwk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yzqkaxpd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ftkyehte.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jfsnuuxh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zqukhtqt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ogtubrid.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3hpcrdnrw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3oisrgnsu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3csaeyhlz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vlpsdtps.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3uphbwcxe.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vndvcppv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vfhhbwtr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qqqvaryj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xvmixlac.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kgpfcmjm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3etqwzqpi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ysqcrcsj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tvpiceat.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3niznxlxo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3fquqsjiw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xuerjfnr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lfailflb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3pgigmqku.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ezewfunm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3dxjllbsv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kxahicrc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jkvtvkqu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hgoexcwq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wxrpnddn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gcnmwgqq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nibhnmdp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tefbbjtq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zrzpewxw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lkqhgsoq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3wlhwexgp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3odmmvrpm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3erazeyaa.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3flnoqzbl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3nzwtdjfv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3nndaymbc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3yhnpjium.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3zymxchrn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3fmgiexei.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3cwyjsyoe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dzftveiv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wjuhoasc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ldkezuiu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vphzoiwt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ummhktxx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vonalwrk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nabmjkpg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3cjzfgjrz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3nneeicxh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lgmegawz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3pqbdrfpc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wqdpebel.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zqeyryci.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3wnhohtjp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mwqbmmwn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gqzspbrs.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3oawsiyah.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vktvbvhj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3oechuykv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3crqxwmyl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3whetmqrt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3khctwfsg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3audbyfgg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3djyccisd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3sjbjgobq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3pfezpuqq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3evcbnjjz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ydhxkwze.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3czdnligx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ccovvshh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3atoxwfvp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rhuspkfe.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pchycjfd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3aopcnckc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3gpopznhv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pmppmccl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3lazugprw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kzxgbjzv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zssebkpu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3yzwbagnx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3bkhpusez.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3suuiggqk.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3qxwiayyz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qbgbphbz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3fgvwaczn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bznivyjs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3flzdnshv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hapmpcaz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3agtksgtm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dbuemmsa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3vbhglwec.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vdwsvkey.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wvrvymsw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3pcayhrnj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3pelnsypv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ovmfkrrp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gyarrgwb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3stpgfynm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3pmiyyowq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ovfadfom.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zdeavuao.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3umphhqfn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qjswmeiy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ldpyclzj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3avljmhip.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rghvwlth.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3lhjhzram.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vearzkxj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3suhhvmej.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3riiuzuve.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xsttfrze.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ueinjimr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3zqdjcmbk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vndywiwp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lxjihqle.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fwmufzew.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3zcxopgcp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3gdrzifmq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3rcczyaix.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3wtihuhka.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3gvfmzktb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jmubxtcn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3unidrsxw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vbonnzzn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ictvnuvi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qjvsgjqu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vbutefce.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3vvvhtqvy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3efvtnvwc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3qsmdazsc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3fsxahhez.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oikptofl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dipejqcs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vthvzzda.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3iljwumip.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ilcpetss.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3pwomlmis.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3mjikocah.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3quvibjod.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3auenrkfa.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3bbrqwhhz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3joiqgtnu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vnscvvxn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3bsdqnkud.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3tmrtvbhk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ezsxuacp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3dnlkknse.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3fclfgebl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zapemfeu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrmzmfkb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3oefljhql.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3aloyggyc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrrnxeju.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ysywnqqn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3psustcjt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3yjctotnb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3fuscmnba.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lyrztwxu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3upzhpcqm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3imynqzrv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xrviwrmm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3xfetogaz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qvltsarp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wbruycjw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3hglpbcxo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3azewibii.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nwxocppl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ouwuprty.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ciicbcpu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ejoellhh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ndhxksef.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3unzifdbz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zqnehzzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmfftrnc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3woljntyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lamuwgjb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nrehxugx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jhuqwcut.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3txeqxxyc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3tpmnpejt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ezcsxpxk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fmfxsnpc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3yhatptcc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wsezbvzq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3khvyfexh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3uqzaeapt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3hqzptlvv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3iudkzgrb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3silirviu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmpwudhd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pxpxcrjm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3zmiqhbrr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3jvmwfbaw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3gjdwxrol.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3wamjcqgr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3oqmaijbm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gvvimdln.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3iwrdesyl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fqytemzm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uxdfzgla.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3vohcyzgq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ptwmnejl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3grbgzgjf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ruprnkty.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jetmgeeh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ywbnlylm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sahybohq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dylmgcxd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3smtjnodh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3yhbnpxfk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3sajpzhem.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3xhuafkmz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mjbqucpi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3wbqlgldi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uihyyghy.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jlljgxbq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ngpyskyt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lffiyppk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3kadhgeea.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uvhltflr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lfpyxxdt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3cygtgypf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgutfscs.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jgtqomwr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aiiwgios.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iosepsrt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zoazpoiv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oayfsdno.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ygzldled.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jkgblwai.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3odivwejd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qluujyko.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3grcijote.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lapmpsgi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ifeoyswg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3jswtbrbp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qqphphap.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ggejgley.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3patmxihj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3wfixsebz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3zkhglfut.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dupfkfws.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nrhhzrzq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qxvwzmjl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bhduxpfj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dauvxssr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nnkdkhft.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qgaeqtoi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3mmelnizi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qxnidtda.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hdwhxxym.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3roxebsmp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jkedpcac.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yzkcrfpt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3bncvxqic.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fkdvonrt.html


<!-- 参考信息 -->