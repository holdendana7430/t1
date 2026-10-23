代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnrubhlf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3olmdnevr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orzqfnie.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vmdkacvy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qojqjveh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3kstpitwn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rydrdqna.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zgevmdpw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3lnuzqtfw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3lcphylhr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gufhbnoe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nfqmnxqy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qeimluti.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rufqpwfz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3spznbjtg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xythihgj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yceufjzd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fspixhcn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3chehzpwg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nywaidgp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qklelehm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bshysfbl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3epfjwpfp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kijogdwl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bcmgidxl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xvxmqdwb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vsfuiqyu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dkwluphg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ibmyrnyp.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3zfuzgsgz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3wljpagwq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nxcfjwxh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3kfncyaxs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3crbbgbvv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pivseria.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xrsfcchj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lzkilkzf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jbcbfytb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3esfuavuj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bhqbuwup.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wrrdbbcl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3joxhghfo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fwumolkn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dkrlruyn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xndzrvgv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3gbhndoln.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3xziaycvk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vnnbvzgn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3flwifjkq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fsralqhf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3awuiwqtq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vjvepxvy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ejnecyge.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qxkcbqdf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3isrklhcf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3djyikdax.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jdteejzv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tevczsjr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3nairwidb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3criliebm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3rxgaazrp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wninymxz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3yxhckfdp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3axppskan.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xpxvvckg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wkrkavqh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xmxniizs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3gyewgrae.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xvcsfsru.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bkuwoogp.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fjiyumas.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rhyomjjm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3tefvbgkd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3owaxyguh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vgmuugkx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3tfxmeynn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3urtfmgld.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jyfckyjx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3avjqgrhm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3awxmrxur.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tptoolsc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3renoloke.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3fezrzdof.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3agzpuwtc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3fjhoyzct.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ohnpahik.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3lxilvsin.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uzudrpjy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tttzgitw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wqtejaky.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3taraeksh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rpqhaoex.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3sroifxof.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3oxgjsnsl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pvipbtai.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3npeclbfa.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fqluwtwj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tmdkchcg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3mbnpfzpe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hnrmoleq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wkhivkzz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3egyadvml.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3cbjdcaca.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ddynlrye.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zfafijnt.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3txgebclp.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lacvamqu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3twfsfhoy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wtuphder.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pjqealts.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3zwpvrglq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3naybszha.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3lqbricfh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3wukdwfwo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nevrczax.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3eaxsqlvm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ntfutbcg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bkylichj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3cxlefhkg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hluhixos.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3lerztdrp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3uqeemdbm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jlcardmt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3pxqephel.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lmlwyrzp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kqtbkxol.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3oaqlqgqo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3yywifghf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hzfjqkhk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3algvhiaa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ckrzyilu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3luwdjpes.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sqyqyiqd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3pnhoyvwf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3shmikqtl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3feawfhqn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dtdsyxis.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkxijwzj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xjcjpnzk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xywfxyau.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3jlqwxuis.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pqfcnzim.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3drfaeqta.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mlxzxxxs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3dbktuliv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3qdsajzvr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3fdghraaf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3twtrwowo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3dzvoebqj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3cdyeadzs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahhqhbgn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cpajhvmj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eobkiekg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lcebrtxz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tbqzjbzh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3rbpycsie.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3uikutxyi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3wixngnyp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3eulzbudt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mwisezrf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vojzhplx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pxgxalfb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wnxyhpxm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nirbkngh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3frvzcbwv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qntjsbwe.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3oibtponc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ixuaufpb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3drolkgsi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3twinxzyk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3okooxjsy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3cezkrgit.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3lbgbcgni.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3psitsgiw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ngeqyily.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3maycuctk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3komcnqyo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3vgsjqxcq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxqgklau.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugjywyfj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mdidbvxq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3tilsnyoh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3keifkvzz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3yllngdsn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3kyveioul.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ebtsaiid.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qsouqfip.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ozcplhhm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tltaauuw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ncswhjtm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3baegdwhn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iyhsrdvs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3svkdxzxq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3rpwbpasz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xnknsrdx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jkqjvxhr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rhqoyzol.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hmqlgpxt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3vkgwfyis.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fgbwchku.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mnenpzqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slqoizbz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3nghigobv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ibisyopr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vhjwskma.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3tqjorwga.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fczekuot.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3uxrwcstp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xgsbirmd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hrcoywfg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3tmuonbhq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ruuinpyg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mooxodoe.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dpktskzo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3mwpxpnbm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3opilnrde.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihasjroj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogpccgaq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bokyjuji.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3pigqpdtz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wfmmkwzu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3msxagbxc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3fdwdgwjh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3swqjtnxb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ivrnoncd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qsbkkdtr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3csitugyi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dtmuhrux.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3cfiyfkqi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3jtitnbfj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3etkwmbvc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3knththww.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iefusuqv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3oegajarj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tkblxwoe.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kladnzgl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ntsjdxgz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3infjisqr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ovotyxzd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3eyxwnyni.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nhjkncfy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ejjfsiff.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3noniwumj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhfxkqio.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dsucvhxc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ollmedqf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dharzgky.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uvxjkzlk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eylhbsxx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxeimqbe.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hqotmail.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ngozdbpa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivmanuai.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rbwpkjfg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xwbjusan.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hmqwqkmp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxswzvku.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kjupbpff.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3cwmllanu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eixvevaj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nuxnlnam.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zboehzrs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zkqxmiez.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3yxresosd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ethlvzqz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ozcrrqci.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3gzfvadmx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ipakbdbt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xjztojqs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3mygdgtyc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3laihrrcb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fczdsqoy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3yjtmjtlf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zbnvqntx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3obqmzztw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ecgsgyov.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3yublyumy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iqtfaafi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bjekqvug.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zpwetatz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lafhjdvj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wnjrgxwt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xpqfltlj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xdtvuqia.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3fmhzxnhh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3bnzkwaxr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfhhguxq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3icwlhmvj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3skphqfln.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gjelaamb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3filqafdn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djkurkjo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwjaijui.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xindggfj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3iovxdeov.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fiigujiw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3gvzfocqv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjtqstyo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qfoxrckb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xzavounc.html


<!-- 参考信息 -->