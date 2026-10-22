代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fjicpeae.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2vskiqqib.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2kqpvspye.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2grtwpsou.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uyalmcgq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ikjmewuy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ievqlbbf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bixzjisw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wdefksyx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jxnfswxx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lodsjqot.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qpngffmo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2uafmpqgm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2luznwcdc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2wvjiljol.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ijsekstg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qqlbkhpg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qcigtpsf.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kxbbjwqf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jtihcqkc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2wefkkxsr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2esdtrjwi.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2xgqpisqu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vgiqywcm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2hegawdgm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ojslbhkv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lxgdukgo.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2utooptoq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2psyjgkhi.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ekndrwuv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gcepaxwa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2lojcaabn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2druhmffq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2yerudvdb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hclhuhgs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2tgosewzh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gbcwcunr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mrahhgoj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2olbwqyog.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jcrjitie.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2uaychhzy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hknqlzhu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sitqgnjj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iqzjczwn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sepblimi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dpxfieqr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcvleloh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vvvduunp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2myigqcrd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2crohiltl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2mkfcheby.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qdvaxrqp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2bcohwhcq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kkozksyq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2mefuuvdn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zxsnkhir.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2owehznjx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2pzybadye.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2wlqraraf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ilckxozu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2azajtyuy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qenqlcgt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pkatiniv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kejfdlhi.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2wcbbavlk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2srrdlttd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fwjkfzwx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2blgdkxhk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2dobmoufy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2iuafpijp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vejqzxvm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jufdiwat.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2klamajpd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2inndfmcx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qokqdjbi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pdzkoaga.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2vhtmaibe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yuftptik.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2eoybemnx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gjocheob.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xoecdoty.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dvxsuoon.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kwlmjlyv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tmmptqbg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2lrgshnbn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vedifddm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2utyomcbv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2emayzqpt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ukrduzdc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2czeurexi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2snchkoqo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gjsbnrjh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sevyenhg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2frndftcb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ffukokyb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xsblapgq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2uhydzxwl.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nslmunlz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vwthgrnr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2rsuhymeq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2iomdidqx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ptflczcp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2eqprcswc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2zocflwat.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2nkojppgq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2llmvwhka.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2timcrhrb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pckvctoe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dfmufqnb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xxuuwfbl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2pobnqrmn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfqddyou.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2uwdvnnup.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2tsrqpujn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hufzqidk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2jiegamgy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2iffkfhty.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lvxjgyib.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2byngatbw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jmespbte.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oijdhwjp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2gwihpbdu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2xapsnjkf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2dlrpijjp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2waiwpjqe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kbeiwbuv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ewmfahkm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wkfwogur.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnudaaar.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nrfmsqis.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tawauxzx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ewvplxcq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2lnzojzua.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cjmawvgj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wrkpejet.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wtmbundu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2jaqzfjnr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hrhijzix.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2milvtgjf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jdfjhkdz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2utatxgkg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2efiranxk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lfsnglgd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2sbfvbpxf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tounrmxd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hgorfpke.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ixgbifwt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2kggivwwb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ictxvjtj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2klziqkmv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2yuuywhhm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qqgvhxdu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vnfyvzqo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wmnnbxaz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tutsndxo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2trbmkhot.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2belvsgge.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ipmmcksx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2tvuyxyoe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rejpfttk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gmyhuptx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yoyebqxu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xeltujkc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oqgkabza.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qthsrxxo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ebhwesgg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2rkprcigz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2wqnimxlr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2eskdfqkq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2elgvdhmd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2xqynakbg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fajbqfkn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2aacmzfki.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2eojhldav.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2gkaxlruw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2pwvehcgw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2rklhqaud.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2asdsefkc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2huivmoes.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2spnpiktt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mganqbhw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2slfptfgv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cafhjlsd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ybounvyr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2gzrwkmud.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tcfxnbdz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wvdlnpki.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kckkyjnu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ntqfmoil.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ojmiwask.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mczhqdiv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uuecucyi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jipefium.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqthtdlt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2aiqsqlrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zocddcxn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2slewuusb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2kjvzpbkz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2emhkwodo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2nihnqhaj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2woqdlvaf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lkbnartm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rpdpbipo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uaorbkaa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vbqbvyhq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2mwskhrol.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2khwxqbtw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2lxtartlu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lijetzyu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvfqqvqv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2safnxsmi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2uepxltke.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2mrcedmew.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtexcnbv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2gbzkfcyu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2isewkuru.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gqnsnevx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ghendbmg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qghoockt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zakkmlvs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ptwgbjrg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mkvswbap.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tiungxwp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2byibptvz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ozyaeibg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ulvfoemq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pqkezcdb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nnmrdpjs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2didpxtfw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ujuzrhlf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2qntwqajt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2aeliyfot.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2purjcwqi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2knabrkhn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qythygde.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chdfvnas.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mszusdpn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iixfdknl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jixteemg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ambkmxxg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbrojsnl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2wtvwatzo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qeiusgkl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fyrtzjbw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2varycweh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2arennkdy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uwmizmnl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2upwnmoik.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhatorfg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xsworsbg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2zmrkwmfx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wpzqhyig.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2mduvhddw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pewufyio.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rhtjrupg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2cnzpfezl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2znkdjrbb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wmtynlzv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ucjsvgrm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2pmmgdehz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wtqaygos.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2olsjubzy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2phahauff.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ootvwavl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jyumiajz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hmeesgiu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2tchowxsn.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jysahfxv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ioxrctfe.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddnixxit.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eyvknniy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2crvhwpfx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mogslptb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dnvryhxs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2voymyzai.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jeyesgor.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2qgjywhvk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rssrgzbv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2axzlukrg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2huwsopqf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dtsajanr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oiynkour.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2xqdyxnnj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ocvxkdzt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2elkalwsj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eokvwxbj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2yarrrhyd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vbszduxe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hucagrys.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vtiibzun.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dgulykfd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2crjfukbm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2sdbcnvgf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pygdoqvs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2kyshoxfj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2saiohbfn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2yfivvems.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ftigsuvg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2nriekunw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2pyxubska.html


<!-- 参考信息 -->