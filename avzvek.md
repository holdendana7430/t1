代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3hmokihra.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ezohccjv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3eanluvab.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3raluykch.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3enbuxrjj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3thtuhwmq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yyohzbil.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yqibstxg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qygcexxh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ecwtqouj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3udycnbxv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wprfskhy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gcqxuhso.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bgtooavo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zyhshlri.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fmpficxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezsyngbr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ciaqqsjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3naakznmn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3thiibiqd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3eqgrhuft.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ssdnpzgs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lpvcfvvi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hgywvbki.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gkpazehi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3gvorniyd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3rlhlcwqd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mutgctuy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qddyavpw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fqfwxbyt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qgcigpgf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hshjfpvm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oqzovwod.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gqgefkpx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3anbkfduz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lcbdyekr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xtfnoktp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xkyiuvnf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3oheomzhh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aoryiwcg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uawhqvkz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ibniuuip.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wotmgdrx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3uuhordvv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3bcvjygag.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qjbxoscf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nfvcgwbx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3cgnaoakn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3escqbxgr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xudgxxlg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eeczamxs.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wwwmumkj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3vuleilrt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3goudofnb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zbbwjqmf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3llswnhqe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3azmhbkas.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3yoxhtbza.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xzfglkfw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3slyabzhc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ykpolbcy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xvalshfd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pokfhgvu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pvoufzzy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3rrfckryv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gspggqvr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3jjvnvoap.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yycqycxj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bvpquklw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zevwdwdy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pxmvzgwo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3htqbuykz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ybahmgfv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ajqoombp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3iimxewmd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yrweewpx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3djhhvjzt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mbtuykvt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3lxosiiut.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3jxpedsyc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ijaktews.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nudnfkqr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kvuogcwz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3yowhdhii.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3jlorvndu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wgdmodhi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tkfolvjt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3urzbduak.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3nefezypb.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mqlsamvk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bhqcjsgw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3npeiffzo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ampapqvp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3fmrjbvyq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3uskqaetz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qjkjbmad.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qmlhaszy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3vcfixzsn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xjeqzivw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kvkuxxts.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3kzyoiyiy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eojfrorr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rcgsunxi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wzpzhboo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zrixtrai.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fgaxahol.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ehdfhqcj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rwuavgef.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3apommoaq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ampphnnp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pyhhpjsb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rjhnaxqn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cksswdpq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jfxjeoqp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3vxftrgxt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hyuwwnij.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3yodngise.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kdtgwlvr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3qvqbwfjs.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cjhotpgx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3efluumot.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xdajddvk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ltqnfahy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mgzmvhvr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3fhlhwlpi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3syusswqr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3kzodvvee.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qpbslvjk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ucewuuyl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3emlofsky.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fcafcepk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnuaklvh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vgaegnsq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3mrlptyxs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hkwswtfy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gukaxdvz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3cpotgwsx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ggwnscqw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ionjhapo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3bhqpknuf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gwivygma.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pcceyavg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3orpqahpu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3uttciitx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3swgqzryr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ivwfivrm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3isrxxuvz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qkrslsjs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vlzcmuev.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wdlarhwx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ehjytvki.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3vzcxlgmx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jvmdvmom.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dlqgfqbv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3keowbpxk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gmzqgkpp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3pmgbuler.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zkhzabod.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zwbotlri.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jcjjyxej.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3xviudjtl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ugtukpzp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3dtvphtfm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3tfcmodds.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ucvzcukg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3evlxkqgh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wxqbtivv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mxhvbmvd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfwvjmyl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qzkwjney.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3olmqgmbd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3bwofsmfm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3mdwxsxlv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3bmsggtio.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3blrpytbq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xyxhjrdy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fjmowdzh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jbgetktm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xsseoows.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3draqunil.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fyqaudwm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qfeomkjr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3zbnhexif.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3llzqxutp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ffsocqub.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3uiplwluf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3orfonviz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3xtrclfoq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3aliwfety.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hqivtxry.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3dagsppxv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3opylxdlq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3wlcyrmwu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfwyeqcs.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqradezn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkvatmzw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zhwdpkkc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3rgulxelx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3yloqpbcn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dnwcghkz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3gojyfdsi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cxpmdocr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mhjdthqk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nawyimzc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3midqvcxg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3qomdubxi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cvmrkaqq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ssjrkyhm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ontqrcbg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bmdbcfnb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hewaolgj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qlxbhwqa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ahqgqefo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3srexdkwp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3dvnxbrqu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ivohvxlk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cdzueyjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blntvitk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3hhiyybfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iaisuaqp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gypypqvy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3eahreuix.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cnmljvwm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3cwqtnkxs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uyamjoof.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3anmzwjhq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jvreqjqa.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fjanjzpa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fnvanqat.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jfolyfkd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3gxxegolz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3aoweywuj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nqldfmor.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcuvdkve.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3molvzrmn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kvehlgiw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3dndfnpfl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3lasgutfm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3gyblfezu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lpvhqbpt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jadlxgil.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qprofkiy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3sejfbxcd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3upyazshu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3sycerirl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3upzkolrc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3biaagwqn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ixxorynk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zncezuby.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ueeiaxjp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dnahvqey.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qayxvwyf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3chcqaixo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3exrojicy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kjrfwdyc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3eeqvzvob.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ykamlkrv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3btslipkc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mipskzcg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mdioprcb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3otlyikhv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zgpkomvc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3plzxygfk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vkrvaqlx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3plwbslqi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mexgmjms.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxpalqsr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3enuaedhd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3majcnfqp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ajxudbqd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tlytbile.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hvwzxlxc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qcbtnimb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iihneuba.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bhzumdld.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jracjxkv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fckfaajf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3splrwboc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rpquvrby.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lcmeshii.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ravhngdb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3tntsawuo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3pdvtzoge.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3nduhxfgx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ewtwxoty.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3mctuokew.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xmzpiqfn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vbgobipq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3atgrjpwf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3vedsnluk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3khofkirg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cmrjovii.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3gihgyqyi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqwpjgrb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xxsdlium.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3eziwhxze.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3adbcmyau.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tjfvhvbe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zfemaaoq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqzgzvit.html


<!-- 参考信息 -->