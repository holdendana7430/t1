代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qpqyiygo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3vsozuezs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ewhjnhvv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cxivjioh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qwlgnxre.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ubaogarw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3dquczrjy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xtbuvnra.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tpycdiwh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xveuglnr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oasrmhvc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hbnairct.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bqcuqtbq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lactaldr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ocdcsgps.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3japqykha.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3paudfurf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3psqpilfa.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hkduzopg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ekhswbtv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lxtgfdmb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hnhervde.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ceilqswv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ypgwiofo.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3koufafln.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3slarplug.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rjvghoux.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3inoadbsm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3aapcrxpx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cqlufqaa.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bduwored.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3skfkpckv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3mvohitez.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ifvhoutv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kszzsfqb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tqlhtdbo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zwtiqaih.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3rqwwjdho.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gaxkjogk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gtqxzvaf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gpetmpbx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zdjqftbo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3edybfiik.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ioliqmqz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eawwjetj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jarzmcyg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rbfzgceb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3juftlvck.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xuxinhsw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pdjmapwr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3jkunwvuv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dfbnfobv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3frxjpzqy.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3biqlduxx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3evmtjkby.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sdiscxwp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xvkbrrde.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ivgxrudi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3nhtyjqia.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3yuorrybp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3gdodwxxn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mbujwyoo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3urtasnck.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zkwdcwch.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3jtdbmpxh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iprxikri.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zwtmfwru.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3hqwqsapd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3agvlqilp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3uaixwgoi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dssgsqaa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rvjoepyf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jcjsaolu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xqmyfqdc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3sxibwvah.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rfhwubud.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3vqmtwhfr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cnazdjev.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dhalxpdc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mtdksnuc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mjwxmxfy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jqgmupgv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rdsynakj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yrugzdkn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3szieovnv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3cmudbzyc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jpsytpsw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eknmkvfr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dudikhun.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hjephicr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dpkabhjx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ftkbjqdt.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qceloeab.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pshsbhir.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gcskmbse.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pjwtzuoy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rjbldqiw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3yoompzhx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cskobbhg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3fqhlpolz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ryqmpden.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xkgtvrmc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ajaiazlk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3mgtndvrt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3gdmnpmhl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnkxxphd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vkcbewer.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hgfhcunb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jfurtjty.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3jlzhoztr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3lfbiqbaa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zccsmiil.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3xszrwfzp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ekqeppkr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3rdnqidzk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3wwcuqxhu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kkghdooa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yjdtcung.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3sokqkxax.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3oicyzdxp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3spqpfsmr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mtgchtnw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3yomnbxty.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jtohrnen.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjyzgsou.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3aekinnsa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3gfrjwnvy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wyadbmra.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3izdgqhzs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3icobofxa.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3emmshoxe.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bztanjus.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3zcecvois.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pvzzqbnf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rddnyusd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fcyeipvw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3erpzjelc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3deyvgskt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3atxrrudy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rucljhij.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3obrezdkq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ngbnchsi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wuwokkrc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3swzupkta.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdpgbwpc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3iyaskfkj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vpsebmps.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3yvyclfik.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3gjmexhzh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3rzklgmbv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3shjvflmu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3npohhhvp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zrbhtfjk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lopwgamu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qphdbuvr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3habgnhjy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xxxgwbrk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hralzmsk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vuxwfkyz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tvupunjn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lmkgtufk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wwndtteo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3wtvpwvwt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lpmcluky.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3usszdpod.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3xtvxvnmp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mjnfhdqj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xmunvbnd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3yolcgpen.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ebedlpwq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfgchpjn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mybqxzmo.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3htrgapdq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hetuxcqh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ivpczfik.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3swibgiyz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3evvyigsz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3irgaiokm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mowyfthz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vwhedwfe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uljltgkj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qxoseuot.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xshezktv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zoyugnjn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fddydhei.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zwbjdzal.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3djxmcskk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mlpxavmo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vxqgrvns.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bgduigsp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3eaehvjag.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zlscwfhj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ojtyltqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3palikwdb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3cvjnuqiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pkfvalpu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ofwxlhpq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3owordnnm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qzlcuywm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kvprtyfn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3aetsnary.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dtrfwzhw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qrqjuzfn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3utfvvxzk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pjmmrizi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3fkplkqay.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3wtqtwubg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3nidzooqd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nyssmvnk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3syxbnncu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ojiiyzno.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qgdyuhck.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3rjwiidrz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rifqcteh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3geuqpmzc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3uyepmknp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jdcoosbm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3prpygink.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sdxuiezi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3nmpkxjfz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3mtiahxqd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3kxmhpfjv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kwkrzvoy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqhxtdrw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gascuzzp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jwsihmby.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rszcqorx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nxnhcyyd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3wqiezaus.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xeexzpmq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3krvfjisv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dcpmkvyr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hltzrtzv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3rbrqdqrp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bhzvyprt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jmqxploo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xmnkmrgb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xaoboztd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ajoknlql.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3emollmfv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kvrwbtbm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rsasdpqi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lscenudo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eknpckus.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzqbhkiv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3coqiuqme.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sgetjcdk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3odbxzfak.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hmsursem.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ggagevba.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ukcolwoa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ncahekmj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wkxbexws.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ixtxjmfj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wocujncx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3zjfanqkh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3uojsqpvt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3jksaehdm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3bvtgcsqz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3flrdlgba.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3aneoqujl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3impzhoig.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eplfmyzn.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zrkgrmsk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ldkrbdkw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rlgvuuig.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bdoponis.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3kuzaxzzm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ggdcxfbi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vniitqkt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mcsvvzpw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nnrcmsuc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3arufpefl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eovkdeuy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3gfkljpju.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sezwtijp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ibqguyki.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3erhvdsyn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pcvouaif.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lsbzdgoo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jayaufdy.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kvqptzdi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zwyujhjx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ornxmozi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ymzgpdys.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtzopvke.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcuxqorp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jijncasz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3anperfhh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jpnnourk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kiziknef.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3msrzcbna.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ieogrxme.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jeajbdme.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3qbxcvzcd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3wxerzodb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3pgvwuktw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3hcvtdrdl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rextfiba.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wmfqcskt.html


<!-- 参考信息 -->