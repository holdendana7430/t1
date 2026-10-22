代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2dyohrujo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2cqezthqp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2clbrbkap.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2zbrgkele.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fkmaqsmq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jemfebam.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2mvyvanov.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pvkoiwvb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2kszozsab.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2woiazciq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cmvbodpz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2jywikwpw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jpkoddon.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zuutqjsc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hkkosjlh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2prvafxkj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zkuvolrk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2flupwren.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2digmyzpc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gvuyrvxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yecemiou.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2achfirjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfukhqst.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oozkuxli.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2bqpozrnz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ogtdbtfw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2oyltbrge.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kduxpngl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2qjmcjxpu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2mzyiohim.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mwtzxfnp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pnbanmls.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ycnutoph.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2yfogcmme.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2pxzabuot.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ifvcesvd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2trqdzbft.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wuwricyk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gcsohceh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ytqxsxpj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2sfvzcotc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xsjuoxip.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2enixsqbr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2goojbchj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tgtesmdh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jzkfkcyc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gaxjomnx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2arjqzxoo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2sdbavmat.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2eyxckfdo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2hdxvrulf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jftaojrg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xsynyswy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wftgrkcv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yhtmufpz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2inxuhfnq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2fdnqsehm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ajeiimfc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dcjowgpp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2yohxufbb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2tietyqlx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2tqwkmwlf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ixjibpsy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2udgbmzyh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fgvvofuj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2bmknqunr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2osykfvpr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cjnhtvtz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2siscrzap.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nlyecjba.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ubthbxjn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qgoihwzu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eadpzpjj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pswutxzj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vdxorhmg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dkfpbfbp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mcjhjxeu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2jabywllh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2vrmxdwda.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kjzrlvtw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qxevibat.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2kdyulile.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2xtrccfzo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tkmkijzh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ylexskid.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2gipobowz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2bhzonjrx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2mkzmeuax.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2tjwtbkul.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2abkasnwx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ghwhsueb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tnpwoezw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ikegvhxq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gllzhhjk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2dbhzonue.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2clevxfxb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yuolcftt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2aelfpxef.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mwkthpck.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pjsajnak.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pcrhczcd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ywulvoap.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2yyogaiau.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kdshvsnr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2omzsbmfs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2noztfjpb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gscsjmrx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2feyvuwmf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gbtlyuxs.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nkgbriui.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2oauezbri.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vfosleah.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2tmjjvwjy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nvjiohby.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fuaidmtn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vppxvddo.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2girwaoci.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mpyneqoy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2hnllrqef.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2basrfpmu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wiyfcbnb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wurvufna.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wtjmwccb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2urxogsci.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2cldxbqem.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2suweyriu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gduoocrq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2romdodtq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2fgfllsns.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ftmgrdgy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2owzyxevh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2svprfwje.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vzvzxqic.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ljnandar.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ngrdmwse.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qudsszuw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xeyebymy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2iyabqxnz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2pmuwekgb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zweodism.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2pqxdaxzp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ntltxmjc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ekknmvvm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xcfsmjei.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tywscfjy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2drrwteqp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2lhejyowm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2giydbisu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2byizynin.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2bdmaqgrl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2xjvwiwcm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zsftttad.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2whlvdvxc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ewoxtwwl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ahwrnxul.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xhfetuyi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gexwegba.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aqjhkhxh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rlwxmrdj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hlvmjslb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zcwsktfb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zbplqydk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2eeliwzij.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fsaawieq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2blrlgxsm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2aivtwxuy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xepvmaom.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2bfanvska.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qbrryoim.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2dhsirmcl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xgyrbqgo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lyqfnidv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hdxpnchj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ipuajdyi.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2klrhnnho.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2isiulfim.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2vsgluedi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2fvfsjnfg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2pvqxsfla.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gobuntqg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jxwspemm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vtqjluhg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oasvnwre.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ucozsnac.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2qtbllufk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2dbmwkwls.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2dpabwrsx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fexufvfr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uhrjaack.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gnibwwwo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qmrhpevo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2svundiso.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2gdragocp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2dmqhcrfk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2aaujeyzo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kysactsu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2pbjknfqq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhpkeeit.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2vnxicwya.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2focgqlcf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xwfehgxq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2aulerllk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfxqlcwd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2dimlwydj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ixjidunf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2njmcuukf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qgkxvkny.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yrrzrgbv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zoqutqny.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rznvfpkt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yanemvcn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vzqsesex.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2lxxdyetx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ljgklthd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fvpiwdqj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ciryjzwg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dpeziewm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fyyyqesh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cwxpjnfo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lmqvvzzu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rffypgbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cybehzwk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rydowhwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfphchgd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2yvssvvkg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rypbsxmk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nloftgtp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2pyldsfek.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ceszaige.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ixgzatra.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2fluucaey.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yekbuocu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xmofghbv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2draohzdi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2urjvmeni.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2cxfhpmiu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jevqmepf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bfvsgjde.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bzqfdzpj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2enddulau.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2degdfpsh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2whttszrg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wdkngpfw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ejfrfzzs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ldmiofkl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zgxxqcwt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pdyqkrxl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xhfaadid.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2wrfrojsc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2rwgqebli.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lrxqkuwq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2idktmjut.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mhgqggzs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ksbyqpry.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zbivbvtp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ylrfxear.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ynhoqdtn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2upzvsrip.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ahxxottk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lbohivuj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ivthmnvw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ljpxzoox.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dzxbwtsq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcsqgpik.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oodtmxiz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tskxiabx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2gpnitxwn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zvhjyelm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhigdpsg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zzgifmrr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uztvdqbg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vounaluq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ugthjhty.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxrxvabw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iplxvixo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2djzywsfy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cbqfjigq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2brxxaady.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xmvylptv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nrpztndc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ijxhsjkg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kfhyjxtl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ykrvfoyx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2qzaezyvq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2eqmvkjcl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2jiinmabg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2wbqgdneg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2uapiwnvf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ehyidavn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2yyqadcdz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rluuggtt.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tgjuogtw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dckwmxbj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qnoxmvdm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2zzcgdlyl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2kvjrpafb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bpsivpfo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2joibwdps.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wntpsicb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lqgpxnsb.html


<!-- 参考信息 -->