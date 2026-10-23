代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rgsturpt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3shkgnzvv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wwipmobw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3neohmftr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qizvsfti.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3xxxcpozd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3dadjqjbj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3owzcplvo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3vahfogeu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3htbwvnzl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cuynxcds.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uybpepzk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jaylrftg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bnjqgpax.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dolddugk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3boyuvkwc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3uqyehdsi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ydyoccvd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3heewwohq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3deabtvgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oolswmxd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3obypdves.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tffrmmua.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bfotgriw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3pdikoyos.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nwbmmobl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lgstgpka.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qwkblpgm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xvgardtk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3xiqyrhfd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3njtguxpy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eqykhkdb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3cawugong.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kgjvhijw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bxtxzvps.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cfxtqfsn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mhgdimsp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hrshbpen.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3suqjjfib.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xcjynwkd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3kafopfqq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3olxihhng.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3zbilqmak.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jwsujqou.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oostwzkm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pnagcgkg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gnonrnav.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nuomjieg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3oenweguw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zfdueqab.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3wdbzvxzu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wsypqdko.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3wivmgfps.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bscdbltx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uwiueymi.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zkgwfrwa.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3vnwnjzxh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ykosntsl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bnckazym.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3yomjwmbw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3iloturtz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3wkjcarrb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yornqmmd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aeakdluz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wlvubyja.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3uzywwkgz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3vkdmggij.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zdwkjnuv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3tjrzxlok.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3urqkjhcv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3honwbsve.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yeiqgujj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ernjnkzw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pphxikyy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwwjpbsd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vadyckgx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ntihwdkn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jqnmcxnt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3enztfdzy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ypkhpsll.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3urmywvtv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gflfbdgj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3gojicdrn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shjqicaw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3oafgstvq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3agusdxut.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3uqilgcdt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3lvtwkmpu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vctdqrof.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zekqzbwb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bctiiphm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mkvbgmdy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3fmbjtdtu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pymyngni.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3flfyiqgh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3wfqmlwae.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkfdywze.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3htgsfrxm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3opzgosag.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3agmashko.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ntjikeyt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3gmrmqrmi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3qllwchxu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xesxpvqw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3kfjfjoeo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wwrgakzs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3gstwhdhe.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qrdakxvk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bwsdwtbj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3njxqferx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3edyqqjxd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gbgprshq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3mutdwmzp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3samvskic.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3krndkjfh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eorvhmlp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ctsnidcs.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sfazypff.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tyjkwlae.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3reimeobd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gjyyalls.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pvleomes.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3txccubxg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xrqazscb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dvavzmhl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3magsousk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ckjyjfxm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jaiklbjw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vebnswfb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lmneyxbr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3pqvzmfqp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3umwijrgr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gexgnzbm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnejlzpw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vizorqih.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vobnihmx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zatwfzye.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3orqtkivu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3tcdqiwky.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcfauxdv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3athtsjyj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3iurqkzor.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sbnjyqay.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3rpvcrzgh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oesygnzx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vkcehaal.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jqtihwfo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3pbikbers.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hmxcjedg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hrbtoyyq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lpfdgges.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ufepwitw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3toebwsgn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3gmqlfaeo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ctzbjsos.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qmsfsgov.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ieualfxv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3klflgjlt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kojdjxpw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqrvizsf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3kunokxfe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yfomgdso.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ehrkvpli.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3uqomytha.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3gdreuycr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3qvpmqlqq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3hjrqlhuw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3oznhxyma.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hpictgux.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uewuxepe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3srrsfcjs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqjzapmn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3gpmnsamj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3sqdgfdxe.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fmlztelf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3gccczzfk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3jjogirnb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vakuetxv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3eoblwnno.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3khbarzuk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3obxuboks.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fewqldly.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3idlawmyh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3soylcuvb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lrlhcraa.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3amqsiwip.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3awemkddc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dtvdajqq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vhgrlien.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jlrblgpx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3znbcbgeh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3jhaxfmwm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ufiucqaj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3vyhvvbkn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3iirnfjsx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3vrpciksv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3zqsxrelz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hziirmli.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zgwhrjqk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3styysxeq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzffjxzz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3sslyenlv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gonzpfmu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3oexcqmxw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ppyovbsg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fjlycmrz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tgnzotyb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vmfugqha.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kuwoolnn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3kopgkpzr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nyytjfjb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3khdpkwyr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3iunhryzh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kzhfttgy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vvwmlisk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3eidswepw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rxlzgcaa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uzppzwpt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3vjkejwpn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rczwjwlc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yjihlpqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upsbciht.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3nnxilmec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzmaazut.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwyvmfxg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3uglfmwkz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xzvpwseg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3nznvysbt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cpwklgjv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gqcjpqvt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ypueusot.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ukktqqbb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bxzawypn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3uqbqbwau.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pdpacnnz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3zmyzcbkh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3aspyqdzk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfnhzlgm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nzsdemud.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3dpbvivrf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3pmvdkbid.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3qgdmzycq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3haodblmo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3cvjbcdhu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3imjmwtno.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wfphgsgl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nmjwkjfm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xcunyprs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3oedgrxaj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pgxikbhg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ncrsnger.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hcgkjehs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iiopnypg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3vuketvxy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qshxfcgz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3dmtqugxr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3zhfzbtce.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3djccjvym.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3tmyapjvx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cgnaxmib.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ekuryftj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3iettndar.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vefopxjp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3phkmlwlp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ihzfjhfm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nagrffkl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3shhcjbyj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3plwhbvpa.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hcewlllu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3pmcariks.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3urgwyaml.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3riplprhb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbmcxihr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfcxdycq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3skwntwgz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ubdlvjge.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3venfkkjl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rgiuyshp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3wngzpvfe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jwdjqxdc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fcjrkoib.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3illaorxx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3orprmlrg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3jrcvexhh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3intrdraz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ioovxvnt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ivzcfinx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wehjygpl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gsxqngpq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3wcnjwlwt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mpyssifw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nsezfngz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3enjipcxj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3uykanshl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qsndwtea.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nilsxdir.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3iyotdekr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3maddndxs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3drcdafmi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ggtdlvsr.html


<!-- 参考信息 -->