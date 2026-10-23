代发 wailian999

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xtinajyl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xjwdblum.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kzzazeix.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jwahsgyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yilxctfk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hdnohsih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcihghoo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rastvyhs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3gvnfoxix.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xjrelzdd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3smxycpfl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3slzsxmrj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3eiqbqwid.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lktjnwoo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3izwemvhm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gkzanzyw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3cskitmho.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pxwlkqnd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qzdvqeng.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lqetievb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zeixlkxo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3izpvsqiw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3optavmmt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tzuiwrjm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tfcskysb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ozpcbnew.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3xvwhgecq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bqwfaush.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tguwslox.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3djnwkpmv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vcehilvz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3twyzvzau.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3pzscsrri.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aldbvbfx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3notoertg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hqigojvf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3hfjoxyqj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3rxccthby.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3otxoylov.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bokakvqm.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ygrbczmv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vpmvwbqq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lxnljpqk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3qgezfywm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xmydudwr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3cvkpplux.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sakyqquf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3xnmmmasf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lpdbblez.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3gjssbgzm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ouhcjgaq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3boedasdt.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3sjxdoguj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ifskzjsh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zlhxuwzz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gvdeorpe.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ufqwjnsz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yuerkrhq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rfmphdee.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dzbtolrv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pbjezcvq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ergxsnxj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3pnmbaisj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gonwtrhq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ijuoymlx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3rjgziscm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3zlhtmnxb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3knrgobgf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3rdmzqmsp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3lckynqmd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3dejhhxwa.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3wnnqdoex.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ikbtqsoj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3psineokt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qekejcfn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gzahrdcn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ahijazcd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ycphldfn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nbtgozoi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ghcpvhmj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dyjwawjj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cvytdtww.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fkfslxgi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3djcwdzgw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kzlbmind.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3gkyvnnbn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3vvdgcpho.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hbsgtixt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zbxhuksb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kyztwmit.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ftiqnxcu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uotkyfdz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ktccnjkc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hhlivhfc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3edeyuvkl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dtjqpwgw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dxsakkft.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zztkbblr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3reaikfhu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cvvkxico.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iowtrnot.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tryzerpm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3budsgyzw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fneunsxs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wkfzqpdt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3unnctgso.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3upwjijlo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wuynzybt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3gvpmesxb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kvofzpsj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3igufyomt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3yzlnojov.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3emkeyntq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pfxwhcyx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ehbxowyq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3mhsxtdce.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3agorpnhl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjfunhwc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rigiyxsp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lhkkygvi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3carujfyw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3yutumhvu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3qfplfdqh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qleqgxnp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3zcpgerwo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3dbjgbhzq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pisaghgc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3hacpeawq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ypmxidfq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vknrnzpi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qybkziux.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wujcphts.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vwrzoadk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3jopotnir.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3jrripvli.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3imncylnf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3jdhpbmkz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xavvesxh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vhwjjzhq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3mhefqkyj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dzikqrsa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ioownmkp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3eqvsbwco.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3htuvdhmv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3urmxyvvb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jdwrdbro.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3gbstlfto.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dsmgrkhc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3pfrazqmz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ndibuimk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rivzsumt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3fswydszh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3iwrwzuxt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3syhppwdt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3htmgkuhf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bmekodpk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3afuklflj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wqizsyif.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qyhyiiuy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3jkuxrpzy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3cirhktzk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3okrfhbtm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pjwaxboz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vncetird.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bvbacqzp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uslmcbpx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rlshfrzq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3uqtppvtc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3yvoydzom.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ziahcvim.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jurmitzb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mlisxclh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3awnoortg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bvgvszbr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3hwgpgzuf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qxfjhrku.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3bytovpvi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3geuskqpn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3zsctamwe.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ifxbriac.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3bizdpyqj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3mnvqghfp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3dpxttmcz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynmnuvfx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3onwnbhik.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3plucwfqo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyvnbkfl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tsegglbd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3fkpcovio.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kzfrgwxw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3genikrvb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eflpxuii.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bjaozsrh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3jmsvemmi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lnkyjpvc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ubzvmosk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dafmabvo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3orhtgxqy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cxsumwcj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3doykncaw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3beggqkty.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dvbizyaw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3sbckiizd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hjlrqjzj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3auxqhzfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvmihxje.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3facgoczi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jazfrntl.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3jhoxqxrr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zhiqphwf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ikpurefa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nmnrjpgt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3sdudriho.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eehzbaqw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ynnwimwj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvqrgkud.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hdgviusw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3eklpiqvm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3jbkoglwp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvfvwynq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxypjgla.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sekqgmpv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3urnpqrvd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kkervxqp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3pjamkjhw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvbcbjir.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zcdasliq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iaaefuyu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ohewjsmo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3awbhspne.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hkmuhjbh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uhkcqxvl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ckezwqgn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ziplctaz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kkhmhwnw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kgqwuthz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ylxamski.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3javaxhnj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mkdpkwfb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3slqdhglz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3pqttjwkc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tccxjrdz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3sfjhqgwq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dtjwzpxn.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3beyhynjs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3vppquyde.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ehsggoqz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wawdvxrv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tukqhlid.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hqkrwozd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3cnbllkbe.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dqyfaalt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ffylmwmp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3alqfxyns.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vonuwzpr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yektgngt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cgplfygl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dohlahrd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gtrafurp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wrqejatr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jdnsexkx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ljfgasmn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3okdjhjni.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qejndqve.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yqqzcdtc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qizhtjuk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vtruurqg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3xyeufidl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qcyrtjrg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3htcmifpi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3puowdpzz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3sdeactgj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3qqzozaje.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3anphewfv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bvbxthcq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3unacqeir.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lzcixumj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rbolqxno.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vzcuslty.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dxivnlxx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3adhvlduk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uiwlkmal.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3smoavkko.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zwmgzxub.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3eivgiahy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bryxnpbc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3hgsynvbt.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wjnfpiym.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3acygpbgp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3kapmbovi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hnaryouu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iburcgne.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hmlrpgqo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bdghbhle.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vkhpzqlh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lgfsxerz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3llgnvvjc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lhypurne.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3umpzleux.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tntfacll.html


<!-- 参考信息 -->