代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3cylnrkrh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vsysguqz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ylzhaagk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bonazqlh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3votbgqoh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gexzbjgq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qketlsry.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vrngtsev.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3jidetpro.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qenzlktt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3yjwsqlkg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3yjrheook.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xzefreyv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vlwwpiaj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pgfqdeye.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3msucqcxg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3lzjmahwv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zkzclpez.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gcqzkniu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ybsuyyyl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3shnitrdu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3aodyfwpt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bpbpiqag.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3rzdwdfac.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lcqnahdz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3rguikxfh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ryxttyps.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kwikgeao.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zhwdrnzb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ldpcqnda.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ucxbygid.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ocrbfvjk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cvqgheiu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ljjgmdzf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bydfxwbh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3shbzggiq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oxndkdtd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uudtlion.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3pklobjnu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ebpqdyfy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3dotefswr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3tctnfhsh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ddfrhjxm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3rllysvkd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3eceqlrmx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3xarzkeex.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xfihricq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3okxycqky.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3zsgapfoe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3oaavmska.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zpachjjk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3uorztbqp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qqgonlzx.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tgpvuwvd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zegrpvkd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3nbobrwgf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3glrjxmuj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3caprkbpp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3etlqgcos.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ciegowpw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rsfvoqpf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3bguleapv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3jfwkoqfp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fuxbpusb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zagwnmrx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nwrolhbw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3cuhoiaud.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cayuujay.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mdpmvowy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3eiejpxjc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ofuqziui.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wgmujagj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3jgfjahmm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3clxyxbtg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dmrwaexx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lvkvcgov.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uksuutlw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iedyxsnu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tjiotebw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fbdogywv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3enneflrm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ccuramta.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3cbpfvgsx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kfhryztk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3vvlbhglm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3uufgeoze.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jdlbadhr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ajucrudi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3wluoqeea.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lrjixcfl.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3teysvouo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3xbmckvly.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gwtukqio.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3iapghtnb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkcdwcji.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkdubgby.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpspwnzd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xhzvfnnz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3rtjhjxig.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dakjyuxm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ckexkwqi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lmqkodag.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3cbhcswzb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3jvgiabtv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3onfgnhen.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cjvrutdb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xrfldiit.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3krmfgkmx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cxgihpva.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3uncyclcr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3spzkqsaq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uqqiudlf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lmbngafe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3aadxlczw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ujccpsrd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ohcnlgof.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifstonye.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ifjrogod.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3okwmrayw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3dseoabhm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3npcbxubl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lpzmivgv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pcjnpjnw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dgfrldjo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3nofvyruc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jjiuefrh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3htulnnup.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3vghiltan.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qddgwzpm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3evgpessy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ocbvgdjs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rdaxtgbi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ijuxpcsb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3qbtqozci.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3eswlxaoq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dwpnkydl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ebbckvvj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3parvirlr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3osmjyddp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dboztysa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3owdxibfe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3khkmvxpx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pdxqhemr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gppxiriv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3evrwsfdt.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3cfbiobye.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3unaiytox.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bfosmypv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jtnfbsfk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xzkwpqqk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3epgpfgia.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ogmyglco.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3tehmphvc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ayinfsel.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3indyemcx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3wrfarnjd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3wekkuqxi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdxjsxxy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3kkinqqso.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ysvdfpny.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hiwliaee.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3otppsteb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkeqewdp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3kuwxsavj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3aqylntyn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tmvcbckn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iaayxisx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3idpmxrue.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dxhvfjcc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3qcsbwgpc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uhhlaakx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ioksqnmb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3iqtoaavv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3weuogfap.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qqqgpoeo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fzijpgmg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zxhrdefn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gagkyfdc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3igtxrefz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kmeopknv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xxbitmkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwvjwijj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3byfusmre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfiqfmcz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3axwoylnq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zzxhwwtc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iuyqyefm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3cdvsoyfr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3otvpsbek.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mutvbkdw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xrsjcxjd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mivlnzrl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3makejdna.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3gxnahvhv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yovwjszj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bouteihm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mamrcxco.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hrbmtukl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jkujwlfo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3karxhkdc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3eufdmdpd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbndxzlt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3bnurqzxp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wfqvbttb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ccnwezzq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3eqhvymdl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dzyduler.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ewlollkc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3gfwfaurl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3sploispr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3torxigsy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3paegzlit.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qopbyxak.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3nrowmnxr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zdgzqyyh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qubbamwo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3bmdhjtnl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fwdxpmnc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3lptsivyn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ipkakntg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3fpaufslj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3bolgcrgb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jvyhzuxu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjsddxko.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3caqbioap.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bhwcckjj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ogxkzeda.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fbbykxvk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3drmrrxgl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3tizimkno.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3chkqolyz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cgxskyds.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjvzcsvh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dcdhbqqj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rssicjyo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jtcyhoul.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3imiqkgrk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mvnxfdnk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zndpsovg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uokhnwli.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3auinniym.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3sxdzmhmw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vhvypcfc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ykahpxij.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3lyydozgd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3htxkdksu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3amkdkrkk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3otvrfmzp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jwlbzvps.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3sgrzxjju.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vlhbocjm.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hlpjdeoy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bazwxhjp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rtwqzdwc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ooucwttg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3eproxbfn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3hyqoosug.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3obdglgax.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3grglaeto.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tblztgon.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3egsszcwb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mvgiavzj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3yzgmxdnb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aurvwgnh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jwbsxgph.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3yezjvxld.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kbaqhyxr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nubtofsg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3autkvcny.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cwaimpks.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3izvukxcj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hdzqfezz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kynonhaq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwccbnje.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3lvpghofx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oycpphlx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3qejwxxab.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zuwroqus.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yntrkbyr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3neptvmwq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3zikbbtiv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3knimnjxz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3vozjohff.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3fiznkcpc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3dojuavcu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3mwprcasg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3sqgdjayk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3odozewrz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xvwcfeei.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ymvbowtq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hswqebvj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3oknmnygb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddgpyvub.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zlzqswzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjnlwomi.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qsyjehst.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3sgyxtljf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3rucwyazs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mozyffbs.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3hugxrtwx.html


<!-- 参考信息 -->