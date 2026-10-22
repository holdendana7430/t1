代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2hpwuxpvx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2scgjkoal.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2sunamrhc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pckslfaf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2nntogckd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsqcrnrp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fislmgql.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2txfygmyp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pwijjggf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lcnjgvkh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ztcterdr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qnmhgjpo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2drqylfrp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qbbootwl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ouwtpidr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rrochjkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omvpafny.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2iqrzugro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igzlkoxa.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jlysbkso.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2svjzvxel.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eaygmqoq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xrwbicau.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gdykjupg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ylhlcapp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2fmlvuxiq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2kzbtwupe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nbuboxan.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hsscowzb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wwighnnr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2yylnejbg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vavqgstz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qakwjfxo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yfklxlxi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zlxywpfo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gaaatrmc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xyrrvfyx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xsrgaxip.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2tdmvkrnb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xdjjqtfu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zodgqqyp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kdtubtde.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ybcceyfb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ucgdmnbp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zwpztsdg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rjtrsxci.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2uadvkczz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2heeatqaj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2alzzchvj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2wramnyqo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xonjfdzh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yntyffrl.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2bvfyjrlg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gexznrvd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2omgutima.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2xgqiiofj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2innzmwjs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2eqgwjfwz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ntqkrbtb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cgbonaxa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2eeozesgs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2sjejzixz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jzpkqzhk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vifdmegf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2zizgcyyy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrtjhryd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ihbbdior.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kflhkfne.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tgopbnqk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gamdiubf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mbwmlmzq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kbssmmnl.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aevrbmwv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cdyypdty.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2gnvvtrim.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tpcdcwiu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2bmikynlc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2choanbxs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2dfvhrvhi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wkojuflk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2mbogiify.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2dgwcebgb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2xzbobbow.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zfpupget.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2dtpggpqc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jcwzbsok.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kclhqmpm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lyyqkmic.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2sjrkkwtt.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ppmedquk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rjkccplv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2mbtgsmmo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2agcewvro.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hvlmxfli.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jrnuflqj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ouexxxep.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2oybyqcwe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fljpbowr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2pmjcozru.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gtsbuzph.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2xjstfuxr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2quwuvtqx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2fwepmpoi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rjedpjvp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bzyzzijz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hsmxctmc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bupsabws.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eiexcfin.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wdwzqpga.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2hptkkslm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jrwniltt.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2haghyquj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2crzuvhwq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2geuacbwa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2mixzeufr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bjkmncih.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2egdmajmd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2luxrgeos.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ugtxzidt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2iplnnfaz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2lejfxdkd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wgmjboyk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gvvurgce.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2xbrscljt.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2oexpkhvd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mhwojpav.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wnadmurw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2kgiqegmg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2mfmadkdx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ixhfbotv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2owdiejnk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gnjaljne.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nltpztsw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2olhxkxzc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ifqhkfvp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovvjoxjk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2mrdsieqc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2dllvifeh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ngguuuip.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2lqqcmtjr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2rfuabtuf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vakcwkbr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2qgctqudc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mwseohco.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fhmimmgx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zmxbhvpo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pbpayelx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dvuvthgm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dztzglqq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2xtowcfbl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2kphzcdqw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2shgidfxt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2txhwqonn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qlbwkxhh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ugezkqdr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yjtjbdya.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2djrtffkc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ffgpwgat.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bbymjror.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jxogbkzz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2cmtfaqpl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jqjsnwrv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jmgngjoa.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2hkgwrvws.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jojknxjx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2agozormt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xhsbyuqx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lrvgmcjc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gzsqaceh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xlcgjeoe.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fihcrcgo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ycoaexdr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2oghmcieq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xdugxsdb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2abjrkqus.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2njlgcqdb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gccvywhq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yudodhgi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hkddgjkv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ecvauteu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zyjavlnz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vgdgsxql.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2iypctpir.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2enbtztja.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zpvwibon.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cgbdnnfw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ipzrlnjq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xxvpabky.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2bhoagdvg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2hlvlvtmp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2aximbwxs.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rttiphja.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2asewxbro.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2txfjfdfs.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2mepkkobd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opztyhrv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2avqmddhs.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vntrqlsc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2yzfzrxqs.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hwzsvcmp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2syiughlh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vplvaxyu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vcrhhvvz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rteugzlw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pvufhlkw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2pmrltuef.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lkxuhiqw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gjbrtixz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2sjzxmqbu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2cpqqnwiz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ekxipsay.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lyozazij.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ivtwglme.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tsdxvpsd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2kxnpacvi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bckwjcgk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ywdmmiuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wteyyddc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2fgudargb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qezcbehq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2rdhqegwm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2zmhotbby.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2okzjfqeq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2unxfwwwa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hfydzoul.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mvwrqecm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2uwvdnpqc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2byvxtymn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zvesluym.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2dbdaevau.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2afdkksmc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2alkbbxml.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yyjopptb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hxgmkeeu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xftotzsz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2gpartqvj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2wfpesnsz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kadviqhr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2mecqvcsl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2udcjpepf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tqmisqmd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2plszpwqr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lyuuppnv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2linllqvk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xccdgups.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ojlouxqo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ztduyinj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qcmhzwdp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pnxuqgph.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2berfpadm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cmsexxay.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ebalpjjb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2dshmshfx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2epgfbxnu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ikanlobd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dpxcnygo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xejnodet.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2xpkayeau.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qtpezhmo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbvyibye.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ncjeewpz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kilzpanv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zpttntmw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xzscmdzx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fszopcmj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2mqbbqodq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xbkpilem.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2furlvykj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2leskmrqh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kddhrdms.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eroyomyk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mffyljsp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2djkcsbbw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lzguaokb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xpopwpcm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2olzwxtmi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2nggwabhp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hnaammhv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ttbuxgqo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wlbpizkc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2vkvzkphe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2uetsmlzm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ntiqxpdb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2sfmwdtcp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ejcmewfz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpippfld.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rnncchow.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pgzqaetx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jyzkeasg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hxnnywyd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2dqxluiwc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2docnuipy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2sofgmtcd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fxriranv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2igfyttxw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vowvmcds.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2trayfyrg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rimnmmta.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2hahkwnoq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vsrrqhoy.html


<!-- 参考信息 -->