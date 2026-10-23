代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gopyptrx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rgrpgdph.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qxdcnqur.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zxvijjzu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rufwedhf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rbohpzhx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lhwucoid.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wppaitrx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mmchekqa.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3yjcsljls.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uhgsijtr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jskxuupc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbijpgwe.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ngftekee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcyoujwz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mcqsyfek.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3eohjwxnp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3qhcdruak.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ueqfxnji.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3pfbxnvyg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3glhzikqq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nydqxijg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bzowjlbi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wifbsfss.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3erprxjgg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pttpgzfb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xpryrmkw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3elhjdtax.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lhiolvmh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kojjzorb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ginkclpx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3myrqrhxk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3syjlsepk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ouoqwebp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rszfezfx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jbbhjpei.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tmbruvea.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hjhjrubw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uhwyxqbj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xhfchozu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3vckveymu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ojwmplex.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3mviyvjuf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rnqyufpf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3fvbcmoll.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3mgxcblvj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jnceajqb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lcngxzcj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3pssmyalz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xdtnzfzc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qdmmxgjc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3rvfamrev.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3iprkmrlm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3nbsnzvkh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uwoqpgkd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nuazptaj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qwynldtr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3mqlapwpl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gvhosxbl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bmokxwgc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3irdojjff.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3yfgeailz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fxlthrdh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xsqpdcqo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ejdukzau.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3guahkmpq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ypyikcmt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vdgzumba.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wnizmbol.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3wzkbauuy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3vsiuosjl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3psdkrywf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3eqjrajte.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vbrqvgzy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3zoykgdxy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gigregef.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ktsscqgd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3qmxhskyr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3rpkymomm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3gqlzmjpu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3doxotnbo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mcobdzhl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3uakdbzsk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gdhcqxwt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qwthedgq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mgctwsfw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nwqvvthe.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3qneuhyhv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xotxxbtt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3kjrfiqfk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3igmdrkxt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bruemebt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tvlvtufy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hgnwnqfc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3jgjuupgk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wyensfmu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3dejtofhv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cpefilxh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xxtohzvo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3arjcluus.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3icnzwyqx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xlcpqbdi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xtzjedsv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pimgrrvw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qbsgctnp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ywspqclu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3atepongq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mefwdvlx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zpgrxkqt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ptpupzem.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ifeupnae.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lqdzkuof.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ivqhynzv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3loaxychf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3fmbfsdcu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ldcaibda.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3puanuahm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nuumqxmv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3euvwxjgi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3kvizrlzp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zwfqohtc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ikmvhpcy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3otnnrzsy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cgevinad.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3dovkbrjk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3uhjdquky.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3irqrxkwu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kxdceuxn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pdrfvrjj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pyigsrhq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3dxbbpsut.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3asvkfhdm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3aetbzynw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3eltwlrqr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ovmjvyfn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3mcpwoukb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3kpjuykko.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3susmptry.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tjbfcqgj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ribxpmyy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3eonwhplf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rikpuxtp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ucrulbtg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3bjxmtvdl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzxecrgb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ogfalucj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3fyctcbab.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3usxmjzof.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrwwyhmv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lqrvshkw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hvbjguxb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3oietrgaf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3oykcomer.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3klhawlbd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3gdjiparb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3guuwngms.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3fzwjryhr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xzaekkxg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rpwpnrkf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3gadjcqka.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ggauirkr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wfqpeiip.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxywvbeo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3phiiflbv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aoogptlq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ahnospcr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nbhakpmr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ckjqljiv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3skctcatr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3amoxowku.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3kwezobie.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cfacoqnx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wbsqnbfo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fiwbtngl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qgjdqnjn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3erfwyvkq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bmtuypig.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tdtcceca.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mzwwgvlv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zqnxhzpv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rzxjpseb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pipjrfzt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zqcsezzk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tcyfezql.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3oznfeuir.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3truziqyx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3fohybatk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3bdaiejtj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3bfrtitin.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iuqufsbs.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3cunfrvoe.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3truwtpst.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3fkdvgmmj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3uwejbqik.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyvjcbxd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3kosljtku.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3bxafibzb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mcbnoavz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uuzrceea.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mavgzjmz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ehqwqbrp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3wgrzwyts.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dkmlaevz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3szawxwcl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3jfvkhfzc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oyrfudhb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pazqmnjt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nnjzkrpq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wkyatjyf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3atwbpgir.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jofmotdm.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fgwxpdkq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3adahaaaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyfayhfe.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3nawfwidr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyeunbmb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pyxiwgtf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3enacdcjo.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oislgzrb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3wcutzcvk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3crwhoedc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hgpdaqmq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jhjbkcnr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fawkwywc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wzjxndhy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3prqhvvbw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3fhybsrof.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3gexkzzmj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydoppljn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3auxudhha.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jvjnlzsu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xdorjfll.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3tiwjueyi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3dklvduhy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3rvahtdjx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ccmdppiu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jqqbjxlt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pyokzsfl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3upxuvhfs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3zxirhfwl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3xrezocif.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zoegfotm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3reyhplxl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3tgifmvmp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pmtrbqaa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3lxzoiyjx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zvtzuvzx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fjdngjjv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3atmmzcpi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zkuezsqq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3kkvkksiy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zhttpnsw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tyselpqu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3rymygspt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cpzrwxcf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3crsfxiss.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3siygbqfm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fkalsofe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wjgmlegu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hpkwbthp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ccobuhza.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3duyviiqf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3etbqbanm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jqzbjimm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3srxnvujs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hudajqny.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vmuqqban.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vnzmxqwp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncaynnkd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mixvqbha.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3wcorpmih.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lltdnosz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lcfiirmy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yccmajma.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hkhmbood.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3jgpnjrfl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qjdisnzm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3retvjmzc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3iygopspp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3gdlfxnwo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3evdcjnqk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3obivonag.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hrvqvlkr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dkkwwgvn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rrnlsnqf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3caxwrbvj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wcwhujmj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3apwrjddg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3pwamqrkx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wrteqtkm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3putmotzy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mrvlhxxe.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hjgvwdbu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hcjzxgpp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zdjqbpmh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aqimjobg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3trsmfbei.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3wybdricx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3heovzogo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fvbraizz.html


<!-- 参考信息 -->