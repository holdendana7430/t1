代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ztghbqyn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sdfundpk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gamqcrqn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3sinsooqt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vafmxkeo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rngichns.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zzyazrgy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3evlblpmj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xebmsbau.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3edzfkjdy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yivixmud.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dxxhgfib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uiceurac.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xltmbvox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwxvmont.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vqjosazt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3haidxdlv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cdcsfayg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3varwjbdb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3patbzmyw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3nsynoego.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wknbesdq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3uwzlnrfc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fpdqshdw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iljcjlaw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mbfnhnld.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3gfnfimga.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nppcpvlg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gnvyjlrp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ijldijba.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3frgdvtkx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ceshtmuv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3trdwswrd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dxamyuya.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mpwylwcl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rqsyjjas.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pcoebchj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3orxpxuyn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xxuaczhx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jatftrcb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qovuqrcx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cattfiwz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3fcxvxnir.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cgdrppez.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3chhbcdti.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ozjobkzf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mldmnxhd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nifrihnb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3xuqrvghm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3aegmgegp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pwnfppnw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3fzvslcao.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3pxqetmxl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3adtrjxft.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jokejwre.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jgerhewb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3skncdnln.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3tpcntnwp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xllakcfl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ytrsglou.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3fxqhzbfa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lygyzaos.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kougiwos.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mdkvyvtn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sztwglza.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hdvljqou.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3erhhzsmn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wqooefuw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qgrsqork.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3norxlaur.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ibxwliwm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ngtcwrwq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3pzwpzbmw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gfniotye.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ghveeoon.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xpexhnhe.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3zbepizvn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3hxsbfmcb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3rbtkcuia.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ktkjnpba.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dxpjxhqe.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hrmononn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zpqdsyad.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ircjzjri.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3zxqkjdfe.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ddxqlwjc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nkxwcfvc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jitqdssj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wpyauaoe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vqvynsru.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lkyzwoet.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uuqaqzxy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3icdyjbpu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ozdzgawn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3uucazrno.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jgviqjrc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3pfkphxye.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sjewrfcc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3zpaedulv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vykmljrd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rbdbzoju.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pbjgiarl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yaiyatxi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xacmquoh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kffxcawk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kthfqmwg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xmvdkysg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gqlrudus.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jehwmzax.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tjqdyxbc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vjoasgds.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3swmwihzi.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3eandwqov.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zvnsmoss.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3iuneoakg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zkneepfm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3utwnqnwd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3yivwuvqv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tycivtya.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3sujsdfrf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3xqopylje.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cxrzdpsl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3kmzwaggh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bympqnyx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3thtcapkw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ciswghbb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pafunqtf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rypsytcm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ayypzmky.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jaousdmo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ihuagxnu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gbeelukm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3tbzfsnhu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3inumlctm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3mzdrculc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3whvfwoxs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zcmyocaf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lcmsmkgh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ojxjbhwq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3eobafwpd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sxjmgtuj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3uqqeugvl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3twkdisnx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nyfsiium.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3fayutvto.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tlddjkla.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3syedzgvc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3cjbfkcqc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3inutkeei.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ssphnfgp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xzrptdpe.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3uqrekssk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wxltjlbh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3epfetpzn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cyarkixx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3crlwovcg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3njjwrkuz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ecqgibmi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3mvakatoi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3fbdifugv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3cxhzdcce.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3sotlncvg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dktwdvdi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3eankaeee.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3snvqglyr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bcirfxjn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3khdrsjsn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3sfbkrykz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3suropnji.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ouptebar.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pwvakvrc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yexwdkjn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uaeswbic.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kblermtg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3epnmpima.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pgkakabn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3qxvtiqmu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ruwdknea.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jgdqcfpw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ptgrqigd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3oftfyjbh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3skxesrum.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zcsefkth.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3vndeqtmm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3fgwsjscs.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3gsdoxfki.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3yvqbwwkz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3lhfdcsfa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3mbwwicro.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3okjrhwha.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3dndosvbg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dodvdteu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hdqjlvws.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bjptvoyr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwcykplu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3bofuspic.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ntqghjcd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3inrwwmed.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pmxxtakp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3slatqjhx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bfuryxqu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3aayzusyi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rhllwwiu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jmhgwxpl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3spuonfkp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3njhagfam.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tbzmgqwz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nfsnaskd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xfvmelmy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fyxcyabo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3lgqqjjct.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qkyjjrrj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3epcdwwwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fefijech.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3aqugpxel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czcrgyuo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jkghqiwy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3fdejzitf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ivqimvhf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3cixjgkya.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uecczrsn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nxfxweoe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ctgudkks.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkgcxkbx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jdmkhlhn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3uroapppn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3rdqsddvk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lonlegff.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3huwcucfv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dkbptdbu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3slmezfnw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3fvskwdze.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ijgnkdrz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhcvvtgg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3bruhaijp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pwkzvhsh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3umzluaas.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nrlwleda.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3typpatln.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ctvjvjak.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3gotsdqyz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tcyvbnrn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mdhmcbyl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3qgaumfsh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3drwppoht.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3knbgqhgr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3avdratyq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vikqpvnt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jdndfzmo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vdyzmhyt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3leyiwons.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qlkootal.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ellvcerb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3kbvmidci.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rlcmhuaa.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uypnotrk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3deaxzsac.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qqaaxchk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3mrcwklxk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uypoalvq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3slknftul.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3dxdbgxce.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vyjnhfnf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iharffgb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3frcckyrl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sugzomou.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ulmwuxdg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3luywonxm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qypdtlau.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fbzdosje.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3iswmlklg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dxcsyygc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wnxyfydy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3duwsizij.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jqncqqpf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3giivhupi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3vdlejiio.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3emasarmf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3fhsahzrv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3emfzdgqu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3jvlqiyaf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkszmvxt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nckujxbh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tejlbwdx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ikyvjser.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xegseako.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nykkaarj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eeatzqhk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3rnpdunzf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wfdziuiy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mubalscr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3aznvmpnz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xfkoqxqm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ntkubmwo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3meicotty.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3opanisoz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zdofxeai.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3zlsyybmd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujdttade.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3emabpgrc.html


<!-- 参考信息 -->