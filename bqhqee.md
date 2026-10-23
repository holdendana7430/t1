代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njgmflar.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3qforsliq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptrzqexy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vkaqfycz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3amaijznv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wlnqbpff.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3miwostmn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oiibhlax.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3rlcrlwdh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3fcwcjfxo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3tflwrtuq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yumjcjkc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3shtfsswo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rqbqnwsa.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3psegnuhp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kdgpdmrx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3phhpidmo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dmrpcqtg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hveqebeo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gocbjgwd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tlygxjnp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gmkjoets.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3eiroqeak.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ahfkvgjz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xtmydqtx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dausqedq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3njuvtqpi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jbzowuye.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3avdswxdp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jriwbexw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3uzckflbo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nujyrxrr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3jkryuiaj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3avzprnrb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zlkzpehr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oansrxok.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3xbyegcoh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3naguxhqi.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ntrohjvo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3hxouwcvb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ydtqtxwl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ijzjowba.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qcxprhgg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3uqakagzy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xmopejvl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ebpvbluy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3vqdfkdwi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xtigubyr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3vzywpnsc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vvdgtlmf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xvulbwxb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kbunwvyk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3darealgq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ctqjtpdm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ktpvjziv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ellflqvx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3omnuzjnx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ihvdyftl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3eajignxi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mxdybohj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ohtnwdls.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3angnnssc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jonfubnr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3obselyhq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3rxzwqmcp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rxedmabh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3slscamvt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3unvorfwq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3fctgpoet.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tmdjrtyf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jjcicfxj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ippfmnht.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3lvwaskhf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zpgdqczh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3npvfezsg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3wgfnbnnl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ceuwjqpl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xxqwqcew.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3svzptufd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3txahboyd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ldgcbuab.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3divpvufa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ofdlakus.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zrxqxcpi.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3juhfruyn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mrbzqiup.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3pbselifu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kaeyqqpi.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kjgrqjgh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vbwqrwgw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3aapfzwpb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lawfpmkn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3guebrabk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3scblpzxv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mkxlpdef.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lbeldaew.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uxmiydsi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vyugwkkq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3pxoujhlh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3aodyfhrp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rpwbnxzs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3veewnjiw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tvwrysnp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3whqszoln.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3favhkbyg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bumggijn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3porymasi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3wcptwsko.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3lsokznik.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ewpjzvqw.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ncpvwzds.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ymawrlbh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3clrodvbr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3xncbkvuo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nvbcaxbj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xjlympan.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pehmkice.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3nmswipcs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3rhljjjdk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3evcimppg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ehhhltei.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3rncenees.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3lmppdjau.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3xxrjxoxw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xqnivxuh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3piucurlu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3irbfkqtv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3nftbhzjj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ocdorpks.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lhrbitfq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3swuvultm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3chvjmqqi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3imgyexjt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3mewqhobm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3gacbjjwe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3teahxlyv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fnglnaho.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3pozfcnpt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vwzuvece.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3hlehmoty.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3alaqccvq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3znlezpew.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ynslapyl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3detywjnp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3qqijhvdb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3hspdcpad.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ynypclxs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jqibdtyn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qbbzvedy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lqkkbsip.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzutrtib.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jqwmqdxm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqhnhmgd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3geyouwov.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hcucbcgz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3gwiixhoz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vjfagamw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3uipofpgf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3pyqecteb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xuophqgh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fuwqxuut.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xcaiazzh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rxgkodkm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3qqkoubvr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqxrbmsg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3efaweblp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ryxmmiri.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dauakgin.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wugeauuq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xknotcys.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3otglbwwy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gyidwqrh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3nstfrmtf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3wqihdugf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qslfgjyp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3nhgqdbcd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3kslmcrmz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdrkiewp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3sholqwte.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbozeimt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zyuzfhst.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ssyyuoky.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3psqanpkz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3sjgiuoyr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3qrcpnvsu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pokcpiyg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xeouzyty.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3knhlbysj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gcrbmtwt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3zcncnjlx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jxgfrkvq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wqjcsgqr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fvwpwczm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3dimyacxp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wkhpiwvy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gmypwddl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vqpjbxmd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dumcjmkd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3tshwumej.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3izacrayz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3eepferew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3myjmbjkb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3vhnhyqof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyiexcbp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3drqmiogl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3rymdrjhy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vteszaoz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3rqgknbwe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wylsslxo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hgcebryz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bkikekqh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ugyygdqm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qchdwssw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xxfgxihw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3pieykinc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3exdstgud.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wavccdlr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rnxigbmu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ozdnbudg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jesjwewd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vortrgya.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnfxkycz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3hhxsnnqy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fubwrwbp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rlvftybi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rwbdjoor.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ftwfujmb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gcttbuwl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3lxvspmxx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fczmphba.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ypiyswvd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ncvitzdd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ancbpcnt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3wtlmaqvu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cgmviicn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dvpmleur.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3onljlbla.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rjycriir.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3edbycygt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3xmogbyls.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ukvwankn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3othfzmxg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nqtawddr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ptebrxwj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ydpufemw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ylhckvsr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3kfuxycmo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwmcsxca.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iuamylew.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3jmhfaxjd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3huwtwhaj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iixwncks.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jzzxhzrq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ttlldnic.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xdmumhkp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cecvjrph.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bddoacse.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rarlrsih.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3bxygfdgl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rfwqfbya.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hudkeadk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gsvfuohh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bovfaznv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3pplglyjj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3eatodene.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ctcqhyta.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vbxenipa.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ctbaahpd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3kzpeuzgl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3arpvidns.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ddgzkgug.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hqhraqgi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rplrtiee.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ctgpmcsz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lymqesjd.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jgdwlwfr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zrdbjxrp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qzrxxesg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ajtmbbvq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ptmqwsmf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qlrcblyh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xexmbjfh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3fsxpvbpd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nzuawizs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hazymdgo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3bdjbghto.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ppjaobcg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lkwedglf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxfdvymd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3chwsydto.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3tbyhktbr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vjiksgav.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3krdyhiet.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mdchqcvc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xssrrqan.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ibwclmiz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3wvccxqtu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iyvdgfed.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zksdpwqa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mnymlukh.html


<!-- 参考信息 -->