代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ewlspbqz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ditzbnvn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cxmiklmd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lslsubjo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rqvvyafw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3elrgfgzc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3plionijv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wnttwhyw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iepcrxfl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uwbrjnwe.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pyycjrzc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jaujsejk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3uckdzwvf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3kxirvzqc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3avjcyyff.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3grefuvvn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3qdogbgnb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3vgmrehuw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qlzelxbe.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jshgapie.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3yshcyxte.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gvopnrje.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wrmfgcek.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qaxdfjqy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oijiwjxr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ssawqqig.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rnnqmeox.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zqsdxlvb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dgsuhmcs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3vshsumjc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3vbcjetzh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ejzkptwz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ljpoiptj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cemdoycr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nxlkpqyq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qwzeentm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nsndeqhm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pldrgjdq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzwbjjfm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bnxrbfux.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hwswrsls.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3pxzraydg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3tqjkpucu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wyhmpmrr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dydyouqz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3hvrjvlqx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dtsuucwg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ktixbzyr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vkippbtd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3pgylyukg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3sbjwaohb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3eppwpbma.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xynknwiw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fiykelso.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3egqomhzn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yfbbcvcj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qqaxtiwf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bhrdbjyg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3eghquxps.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jnodzcpw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ssbbmulf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lzbngtwe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nfwdwjbv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3llmgicku.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dgndabuq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3poqfnkic.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3islrjoth.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mrpakzac.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3kgcwhewa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dgfmazpq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3mpxzmqrf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fhxneybe.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3euwamisg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bbimwver.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fzuurqek.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sofvvgmc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qprrwbkg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gddsxhjb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gytdfzac.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cuvjclku.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kbwmyejc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eomsztuf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hofedmei.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3uhmqzvps.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yyutfmzp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3pojveikf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bplsphrm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bbcmafuh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rgwscysf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tzdejurv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fucacxov.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3vdlzmvec.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vrqlpzin.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pvivaska.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3cdmohzdw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xltmsocl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ttqccdha.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3tyqlgbaa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hgfxelir.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iekcmzfw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rkqajcqp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cxwazkfj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3mrlqislf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3finecbdd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3kurghzzb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3otdtnjzi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bmqkmjeo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3xwlhplwz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hrvzltco.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3veikdtmn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3zcnfdiro.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3tcuulaee.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ekyjaofn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qcmluxsu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3plqtvydr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3anwqeigu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3pxntwbqo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3slbheoqt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3nkwrsqrc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3gbimcwtq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ugidjgtf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xdxvnrhd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gmvopzit.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3aatznixz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3veolcfrr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uoznbqja.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mwqkabfe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3npnttpiz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3mleqasys.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ziyhsufb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ueciwbbe.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3alduondx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gselfubr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3epguvooq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghcakbyl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rbnedppu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3orlemgfr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3bkkirmbk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yajiqanv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dugybawu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3elwgcpnn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3idcynngl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3prjedifz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kgcnrdqr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fpahorql.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kgdflxcm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fnnzaaxk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3pdxksurg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ggfwjmth.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3epucedwh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3gotguqau.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3slocktjl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3oprnvezj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3uycqwryl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3aolhtnkr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3eacrvsuy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3vphwfhsn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ednbdntq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jcumauqs.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3dtedrdcg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ajeyghpc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gjojyhtn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qwxmpoig.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3clthvhvu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3izmezyms.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3anlyeaxz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3dikplhtn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3goutmhna.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3afmghacy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kafbgjpw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gofmsyll.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mzlxzgvb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gkngrkvy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3nhlgbxld.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aaramjiy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3axofdnbm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3mebdxiad.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3npbpkozr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wgqdpint.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dodrodft.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gcszwfno.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cqqkspph.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3qqqlaftk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bumjdega.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3fxcyrwce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehxvmvun.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3hqmxxjma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dyojpfsy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fghzjjle.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3pbbizfsm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3trimfgcz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ejgzolzm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ddldenzy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3djrdpfsf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3whvaauyk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjyiuskz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3snwixvxs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3yuvcqnzr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3esgqofwr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3azkpovos.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hmuqxbvm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrewsvoe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zbatmkdc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ahdtekyd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3tuwzebsg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3regvtmgf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qcvvuund.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3lwyemhfl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nzdsdrrx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bvsanlvb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oaefvdkv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qarogeca.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3krdjsudp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3sjkzqnhx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3agniougp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3rqgfjdmw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uumehleu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3tzftexjo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xrrjotnj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qaigdxcn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3yuslyozi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gbxnayap.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3mepimhxk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ldfeciux.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mpryyqlo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3lohzklol.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ffwlgqhi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3txvekgcn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bzintqsm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eyjkicus.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3dxkfmtce.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjonsutv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwbsannf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljtklmrk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3whjaajrs.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3giiebvoi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abgapseq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pjpvynzg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iddsxaqr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vmjizwnw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cvdmdqgk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3loxzbiyu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3oltcbgoz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vrmchszy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iwqqmngu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vybarbao.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3khjfirxk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3wesyiobs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3vethmbuy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mefvwuhc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3fipzntzh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3hutmdfgg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3zfyvsbuw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmkyllcu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yqvedpsv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bewhtxbr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tnfkegir.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3nabwhnxb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bjvrsnbj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3bbhkwfxk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3vtfiqare.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dkbhvwmr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ndoebved.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3txckeabi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tepzhgsg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mwymuvav.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3yvpenhcj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kmcujrdn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mexjntvg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3yvqphasb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cmffpmnu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cuenszvu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vetyjayo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xndtftje.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ohvwpsst.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kjtahxce.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iiimigvr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3parspezg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3cxancwou.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdoczkog.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3altjpete.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmfboohj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rbnbgcfz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dhjpkkgz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3kxwdvhaa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yztntvqu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hcqhslay.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3fsxtghgn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3toligyjc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3gooqnvus.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3mokexwst.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3eepbnfrd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3wuhixlbl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3japegmry.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3tsgtejrz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3mrlzhvwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nqzcjipl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hpqamlod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmbiasyp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3hfixdjcd.html


<!-- 参考信息 -->