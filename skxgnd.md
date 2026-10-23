代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3eklbpfxp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qdsayovc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3slkgljgl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lkfmqbsy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3cijyqdox.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ezphtccm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ylvxqsbb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kxgpdbzc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fklukkiz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rihtqnzr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yilmxhlf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xmamwmru.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3eptiahyg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vfqpwwpo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qhurfgnw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ohyizgzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjslhkzx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3atbuyzjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdzjrmya.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3shiivdoe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3lvjyskte.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kdnglrla.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jcritfuw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wpgbrdgw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3tnrowbpy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3gewwcgtj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3lvopukur.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3svmtjdtm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mvpbyfun.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ilizitsr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sijqkxbf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hevczlpn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3aznjbwnj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tejhlbal.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pgjhgdwd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rwsgltip.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ecznsfny.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xwuitxbc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3lsnrsrls.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gmdpgqyt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mjgxqmcr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rhyijxrb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3efnyuamj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bonwormm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3vgovffsh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3wzranjat.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3njiohskx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3usslukvz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rvzcqmhq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3wbxjujtz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dqiofkfz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ikqzzlef.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ftooricz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3amsgwjbw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3iygdcsce.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3oitvofuv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kcgvjyfi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3sddplxhf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ycdrznob.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3opbefpeh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dqzodyoj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xyrgcvvx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ohnwnbwf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ueblcfxk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3yzmfmnuo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fmmthtvb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3lxglwxil.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mzrehswq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bhnpklwy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pfkuunir.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hcskmtas.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sclujmzt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3smccnkde.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3hxsudjgc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3mnoqpnty.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hpbfzihk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ykbwbfvg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wejxkcun.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vpydulaz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xpdujzbp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3kzliqtkn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3brjngvae.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3bclyxzzc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3loegvcut.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3rduuzddx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qeplknsn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uohhrols.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xqgdooua.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3uxhmpnxv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mzwanjlj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3otznpmia.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3qlusoewg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3dopvwwnl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3mgzlkhkj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3adutdslf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3djdfkgyz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jpzcntii.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3npvxczkq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cprhruwd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rfrqzucx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3caykolzp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dlgtlawq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3halomjky.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qntrmvjd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ojncurug.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mvyfwvkg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3umbizkih.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lusgwfol.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3beqouxju.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3odzgywfk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3riatibio.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3byecqkxu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gyjbljgz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mhyqtknc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3konjcrab.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rzqneqtn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3scmxyjrc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sjxeotkn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ctcjntru.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nzlmxsaz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3uhzhvpuf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3luvvsxal.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bqgrgcoe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3hkazmcwc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3tvzfwzkr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ngdxzfjr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lysgyzsm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3nbkunuft.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3upzmbpxt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3afdrclpy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3esdsidcw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ffcimwsj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3edgcgojq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3telpkbzm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3mosyncgt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mmhnrtdk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3zdcuanhe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ydhbanid.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3uqhatbsl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ipbtmzes.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3frphnhbk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3khojznmk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3dlkziiks.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3eppsfbrt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3szqiubsk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hsdubegs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bobvwiuk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3oxcytbwb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ctzglppw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tpmosjhx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3uwtyberq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3krxvcgjl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3lccieeuv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ltnqriac.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rpipfovc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vfnhsvfd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vyprsmwc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3plhbrcij.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3czkcrufv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xmnuqyxt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3tmycjumu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lkbexzeu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3psubexgu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3mlrastci.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qxrbdjel.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3otdtuxwu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uvlxoxhf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lrnqwcbz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3dqptihgj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3lrgkaqbj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fuqbipek.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3gcmotfcj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3fzpwkmru.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3zmwrzcqr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3nyqlddpd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vwecoqlt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3arqopddu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hbyayynk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qzkubsvq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hjmcihcu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cojupynk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nitdawky.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tzppfhxc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wteitzuo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3uqqyrksq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pcguvdsm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pwrzoxkk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jpbmdhzz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3klnpvlkm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3yquyusth.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3gxltbvzn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3lpixfdhq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3cwnmirmz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmbuvmuw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mwegtwpa.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvsfczez.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3smymirto.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3dhksztac.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnvmiuud.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3npgrekjx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lwtyibuy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wlsnejgc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fnoqauhw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3chqcvmym.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nyyarmww.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3kkltjmlj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ogduhkps.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mdxcjhlv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3avpykdoj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3mumwvrrn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3buygvqcz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zghqokci.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nqzmyzcc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dwsloocy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3cvkixsqe.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lwcormeb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mxlzxopz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axcdysjg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3kwalfjhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcysncmv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ehxamtfh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3iagwshrf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3olkipsov.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3fckjqszd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fqngphnb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aiohfhor.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3knxldvoo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ixmkhgot.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3limtkytl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rbvkpfvi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ujuyliig.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdovdgdp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3iulukqhx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wxnzbujj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mhwtxfkb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3zcrupsat.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3diwleksy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3wkvnnelm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3dpolumuk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3hgmedvls.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3luqxhksh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lffqtruf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pasfyfyn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ryjwnppb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3msrlocxt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wzytxopu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ggwjzzsr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ygqmgahl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zexkoggf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3yeteivma.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nsujojgk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3imlyfevr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3syfjinsz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nfhrekkf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3uxafliut.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3eqoigtxh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fexkktlf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3doggtvrx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kysoivke.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eonqzeps.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lftdlfnw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lxphtwgz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3nafitnvn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3obfpzvjs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ybwkqfso.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3huchkrjn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xsawizij.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tsfabqzb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kdhixhxh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qrgkmgeu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fjrqguwi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3luoecyqx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ovayhqep.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3drhrsclj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3iogikime.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dhhsqeuw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kwtusfcd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3sinspmnz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rzisbtnm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3inxrnrxv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3sqyugnkc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3uuqzipeg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hbnblrnc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3lojjrsrz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jgnxuwgi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3unozqmgw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nevanilx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tjaqnxqs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3thaxnhrx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jywtfotx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3inankizp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mrawpths.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ezoitlmb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pszhwqxn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wmiiqwhh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3axtlzkws.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xudhglst.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uaetuodx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3talwhpvo.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bwphqftd.html


<!-- 参考信息 -->