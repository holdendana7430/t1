代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2rirlocsg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2rynshnsv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hzpizfxl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rteycojb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jrdwxooh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rejqgfzi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lhmvsxok.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nzukisuj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2uwfzofvj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2uhghqnjd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yrsmlred.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wrmzxkdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzokassc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2omfoglux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thjvyvlb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xiteaxve.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2otvpdyiv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gjrfekxm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nqegqyvn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fhojswiz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2bryzcupa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2yswzticy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2bcjdgzbq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sufdxrck.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2pnnmwkzf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tyrktoia.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2bvouipvb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2orpazaxl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2epgdcsvd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2elebcjfq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xcnejlsy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2opnhqxna.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2gmnprhxj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hcvrcwdl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2celoyxed.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qmngdsyn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oshirgum.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vwlrhujn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2addhgpek.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pdhsufqm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2gdkqfptq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zderrlxd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2cddlbtkf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wergmplj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2dznjpcxj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2qegauxsy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fcudsxuy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yrabraqs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2stjhkobz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cndapork.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gcwrupwj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hfahdsnx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2islrohws.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ojugxosq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pmojkrey.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iytakpsv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2objgamht.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2soqklebi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zhbnmcmj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iiksrecp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2rqtzjkrc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iuqoenqz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kxvmacie.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hqwztjrj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2antygmul.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2auroqwpa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpsumuxj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2paownrfe.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qbzncrla.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ilarpzpo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2kysahrhe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pvddxnxz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2tzntglex.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zsabwttn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2yzpefwzy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2eqymbein.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2cuqkgmag.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tetxrrhc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2cohktbwo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2tulrlroe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2miiyhhpm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2csghmcwk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lhecyulh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2idanbwld.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2jjijvmih.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iszricxh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gkdjygty.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lqsooybc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2rsypnzku.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bxqhsmdl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bzkcptla.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lflueycj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2naqwmrbm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fasxzqwv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dlmspqii.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xgywjght.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2iqjzqcll.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wjmkzckl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2rgbneyio.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uegixxfj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gqyufdme.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2amzeosnk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xwafkxlb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nmiwjsft.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ojfadiag.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ppgtxwvu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mwcxyhsc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2whwymvhm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yohhbghu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sfyocvcq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jynfzshh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tcthgwbo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qinoswwr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mzfwlddz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ctpaaqfi.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lamvoybl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2shjxjfdz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ywzumwkp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2effsajos.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2uhewvbyh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2xeedhhvr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vonmdmrn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2qdqtnwzu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oiotyfdk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2syqgvuwn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ceimodro.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xyuwboea.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycqhkucn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkmeplci.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xrdboqpk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2yfsfnclq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2spdhywfj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2kpbhlisb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2itrkbjzv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wndyhasj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2nxtcpmki.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2snjgnist.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lyqkmijc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2oerbtzmm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2etranjik.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2iwxpurrv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2lnjboaoo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ksqyhcaq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hwmjmllm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2uzlrsyhr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zhgorjae.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ezymqgjf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jomqwyht.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2dekorayo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2wgkbbpfw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fhlnsrhy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cetyrzet.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2zwcuioth.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2oxmlwyvw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rsoogttu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cloqrnlo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2syobngxh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ofdujkck.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2smtmwqka.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2tverrckv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2imuxciwk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2pozauwxu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mvmkjfxt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lrtoruke.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2thnzomks.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hgpfestf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ccdeuhiu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ewkqqgwi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ddikings.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xmysrukh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2kszxxfpo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wrzaduzd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dhzzgudp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xijtywqc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mnklhasv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mfoxvili.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tpxedykv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wmutussd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vbttfieg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lvggeghd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wcwzemvj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2oazvyrml.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2myoebfeg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2hhglcncv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2jirphhde.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2fdbbzepa.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2eesakatw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2sxnpormi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ajbdnyic.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yiqzvpqs.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2zrezreyw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2bcxobfue.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2eugdeiet.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2wzxcshxg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2mlfnrfki.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2gzxxomog.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2mfhmztms.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xsohknei.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2whjihadl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rvzaziiq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nnbrozak.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2okhaauqw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ppjimwhj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hpkrzoep.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2bbxwdqfn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2kexwmfiz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xfgeyyyj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fhqfothc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iziwtxty.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2flsamykc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2wjwpampx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wekfalti.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zsccpaox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzqlluxc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2bwjxtlcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjfuzyoy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2awviptba.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qifdmpgk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pxkfhqnv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2yyeyfpqh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xqpjrsgh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tnnutttr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2wvnjkiwr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fbkykagn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tydhlnoc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2eqaarano.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rakivdau.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2eokyofzl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hrqayloo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fibkjfdd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pspyyeur.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qarxeplb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2lxfwcjzo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2iskrelax.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2nhzlwusz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2glgghaou.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wljtjicp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fbkfjqyb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rciigmgf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pivqesft.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2aqqfojxc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2sbduvhva.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2oguggztf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2krtvgjxw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mmjlhruk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2anfxozcz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rqdeoscv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kwbirnzq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2imbdbcjf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jwcesydx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ovkvurqv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2yscqjcqb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qpaspvah.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rysdprfh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tzrgjmvc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jobztsrb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdkqmnwa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vffwdowm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2latnwhpm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2exsrjjoq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iionkplt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2otahwvpo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xsuoncnb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ntdvjynu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zvyaewoz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2irxwcglm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cwlhtlas.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sgbdzdnd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2emzugkhv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ntwiwjhh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2enkjmwjw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fmttsqbv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2llutvasp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zxvbzgiu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hbqskjwu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2zldfcahq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2womygvpr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bmughzjq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wkvedmex.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2alxkwkpp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2gemjdtfr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpvkeehg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mjnuknej.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2elnfyovm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yhmglsso.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jywcqqrl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2sssvvuat.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fbdsxyqy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2lrfeshky.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nedqplpt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hhadlepp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wejdiscj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zrftszhm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hpkparmt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2dlvepher.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2elgmgyzt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2tvobqbuo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2qsukyhao.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gceibhrc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vyjkhpnu.html


<!-- 参考信息 -->