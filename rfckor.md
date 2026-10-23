代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xmmeiijl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3prmgvasm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3efczjkpk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3mqcphako.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kpgmizhx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fmkgfcdz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vygdaftz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xdwkxexs.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fkevrtlm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3txvgioiw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3guddakya.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xucaqwcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwakyclx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3gvzdyeer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lryyijjc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ddojxlam.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3lzhgokzg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wdueyots.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xxievqry.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3huwcaarr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3yopnlvve.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3prxlfqap.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3htzxkcoc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wnzwocdh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3obdaopyg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yyziircv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kcbtmnxn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ywhsvdaa.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wtzstook.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3snmduzqf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bprbglkm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ctvlkjzn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3sobipdmy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3obwixvcz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3fcaylnnj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3inygscxl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yuoeleol.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iqezrmtg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ctqhhygp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rqlubbck.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qjgzvwig.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gvhmsttt.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3vnzfhoxp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ozunstts.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3yfrmfoyh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dbgnpwmn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bgazohup.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uaqbcfxe.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ouyydswm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3uxtdrsoe.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hfamhnhd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bafmjite.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3urmznoku.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3wnecesjb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cjnvgtrg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kqakebuz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kadsqbkt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lodtrvnf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kmlaorym.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vqcnnzhh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3qxsdowkb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ywpjrdfv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fvuokeoh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qtbelwwb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bveckdkg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3odzvxajm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhdpyolq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3irnabuss.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mbjdzeto.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ydrvvvbo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ilbtdjam.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dfnwuepl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zqvsbbqr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3dvolvbhb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3eycapewu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3mzfbmsgv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3omenrifb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3uyroxbmg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3laipfjza.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3greeegdo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dfvcnxjl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nwtzhjes.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xcjocmty.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3eugbaymp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3coyyqdzf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fzeilfjr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3eznjmxbc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3eciqassg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xmgqjevs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dtfktdnp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nsfgafum.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xmtwsnbw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3asovmsia.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3oihzoioa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xnqtgpms.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gdixrisd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3snooqdhp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3osjklzlg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3nihlpnwl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gyuulnwn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cxodvoba.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3plvrzjrs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dyladuvd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3odywmzgk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3gqokugud.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3lxlqwejb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3drslgqcn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ouvvuvqg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uarngrpf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ddlrxgso.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3xbweyrmd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kpooqidx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fhyutvek.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ehtbmdsr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3zvgzbqin.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kwbjgqgv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3aftfxgid.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hgchvbll.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3stpqkuxt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3nejtxees.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3bjdwhgof.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pypnznnm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3kzsglteb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3lumvltgv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3vfhkynel.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3plhflykh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qppwgfyt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ycgubwkf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hhceyuxf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xqwyamcc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fbaxmllc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nabdflix.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3jxyvqqje.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3prhzgxxk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3kpfsacfi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3fonqncyb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gqzifbdz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ssfpxvic.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ojfpwmvy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3oadrrywy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tltlmfzx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3kzliinoq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3basryzlo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3duwfiaro.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ptyfjkfl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aahlbgxl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3gvgejrys.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3qbhpeykl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owxiwnjx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzqgceed.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ztolewet.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zidyttqg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3radjmbkd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3iuajbsxk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zlssdgmv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jyfivthd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3thmtsyqd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3mducaokt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3bccpvizu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3mlvhviau.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3iznylllr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ukfxrdwl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fbgoggit.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3syrxvluh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3inticakh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zibcmidt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jqbpfjee.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3imxuynlm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3eqirauqi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3cqfjvrip.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3gwavvjga.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xnnkiqdv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zjdlwqdp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xekjwijc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qthuujez.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3bifzkedw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kxffbgtn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3wgffsifo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3gwjcuxha.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zafymsrk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3iyefcsem.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3briempdr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3seybhckf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jgvyaesn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3rzrxsebo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3oiphecae.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ibljcnie.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hxxctgex.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3slxqudws.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3lgliupda.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zdsvnqeu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bagfmdhk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3wjiiluju.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3mfnmuzzc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ctmntmht.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3gygfslob.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3tvqyphru.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cdngnwpc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xxlowsdk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ipodqtnr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oqexpwid.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3vbcbwigw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wzffsxql.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cvvztmjg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3yzwdbjas.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yaalcrmi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uqjobtxv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cszhbvjc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ucwunzst.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3daryibad.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3hxwxhoqu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qquqsxyc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jyhwuslv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onnqfwri.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3nfrevjqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwfoslyo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3epopowos.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3toskzlma.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ztmamyqk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ismcnthd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3awcufhjl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3asygnoqk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3izlzxdws.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3prynteny.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mkqjxmjr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3zjbwrszz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3wmbzjtyq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qefntgzn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jipbizje.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mheqyjff.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gzqreydo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ojcpczhj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jxicchqx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrfgmuyt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3nmnecuxd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pbosnlvz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bjpotkoy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pnaqjcsy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kiwovizi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rxrlswxi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gleqhktq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ltvwfeev.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dnpvhwka.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ppptiwhl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qedvjltn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3sascylfi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ptweaezo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hbvtfrhb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3iyqnyubx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ctnolulu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zfdoclbv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3orspcvnv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3clstxvte.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ivjqcfsj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zgdbupbs.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eknvmmfo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggamirjo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nvflrsni.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3fzkkzbis.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gwleuedg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3undwlxam.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3wgobatpa.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jsbatruh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vuihmode.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tskfwwgp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xhtqnaem.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cwczahwr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pwljdxjf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhytadto.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cqomoqxc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ikyckdtj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pqfyjxee.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3rravjrvx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zelcvygc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3izkotjoo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3yzceomqr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3eghqxfix.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3kdkmqmtn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3nruvrvic.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rnvjbzni.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hbdxlmep.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcyqigjr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kgjhxobl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pocsbqer.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dpnovqre.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3pjaufwjv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3igijltkf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3okscowcs.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ucygalqu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aeevetba.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uznaujya.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ngqfsxnr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gahtumrn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sbnpixne.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3enxawgrt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wlvhbjxw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jjnfvotb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3wtokuaur.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azhaebdv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iigchdvi.html


<!-- 参考信息 -->