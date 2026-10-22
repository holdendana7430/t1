代发 wailian999

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2pcoslwec.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yypycidm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ugaqpser.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ecxnukai.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kzenmtsm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2xfpurtkf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2maikumib.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2yrxjtvdn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2xuukwarm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vejeobai.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2sykjfjif.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ykyljeqv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xiedwmwr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wltcgwxr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2oblrkcqf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wnvmjrpe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vjhwaier.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xlxqwfhh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2oqwyalrn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ynxxxyde.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2topdggsm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cszwmqiy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2hkriumli.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mjtafggz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2mrxikkug.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fvzcxsbi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmdudqgd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2rfwmzhgn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2utnrsegc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cfrkrxjo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qtacvtxj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vsxfgctt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tpznipzt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2keqhqeop.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gifltjth.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2shgvnqvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdftjaup.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2akjvahgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkjglvkg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hqzatjox.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2hlazjanj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lxauenla.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pwewgsde.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kgsagkvt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2pphqyksl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2bsmyqkpa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vioulqff.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2teshtijn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2kprnfymf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hoizwzvb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2xcjqazai.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jeehncqb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mkjacbmr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nhmrrgtb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2whkzpahc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tyzrghlx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mzfzogzy.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2iloymfjn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2rhlgykrw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dxlrjoxt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dlyiojob.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kzlmhhsc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xpxlubii.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vvpkuush.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vgbkrouf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jhdyrbnr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2vofebtke.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2obdkvsrr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2gjnvitkr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2jafhmacc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2sovbljnh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wlgoicjy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2mozknebw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cjrfksng.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ounlirhq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2nzanblwd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pxgrtica.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2nvgnztkd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rkycshmj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aajsxlaj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pzzeeyva.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2zealasre.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2vblnpzdh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ciiwomhv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2cijmymjo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kyxgycvy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2yminasuu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rwsljfjy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tuabffpj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dlflvfyt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kpugvubs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2djoyoftv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jlrnumae.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2jeijvlkb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2afhjvmqx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nwexwvps.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2clbhlaeh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jzhcahht.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ehouxsck.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2elzlhznm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2rhgjvzue.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2imedoxca.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2sriuqjfl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2sjrvbjvs.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2pqryyprc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tuejkwgz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rtuhkkdu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2szlsunfs.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mlibcybn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bxuuayoi.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2csjgwdur.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2hcpbnsjy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2esnznbrm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sjspqhca.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ucfgekoj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dhyuwokw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xhofcmff.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2iqnfwrcu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ubornkry.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2iyzrhsbp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2zvypeylf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yalrbmvz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2igbdsjed.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mlyhmwue.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2liatiepu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2atuetfyz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tvfxbtai.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ykxfhcvz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2pybmxfqe.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ytlrivsz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xdwnqtbw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2uvrhatrh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tvjttfxt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vfrfdcoz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uxxkkocg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pfxbvmmj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2erpsvkin.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dzpqecgk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zezmuhwq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zyrlpien.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2qnfthyab.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cbrigwhi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bjbpayeo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2nbljdgvj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xfjtnsck.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2chrsclhj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2pikllcvg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ykgiupyq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2cvryvqmi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2xgyljgyk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuxjjvqv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dpxxwyjk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehqagxpn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2sacgnghr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2kinldkth.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxtyqels.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2yummduuo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xtxyhcry.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2xrpehnxk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2twfazpld.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2fnewmytm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ckpffrkq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2taqikkuc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2bzrrawbq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qefgpjef.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2vbccacrg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ubzejdpw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2odffkchm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ehsgkylk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ifjpjxzb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2clrzfhzv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xyuvbnty.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wudnpgak.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dbkeoitd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2elqdrxbu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2fmwfwclv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2qtcpnqwt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uibeefcb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tmhhoexv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2irfdrama.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ldbpmzsd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2helpjgkx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nobljywa.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2qczjuqpu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nkpnrklc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vugzvsft.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kazvoyua.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qoufninu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2evrahjjo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2etveubne.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ptsskudo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2xthsvrio.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ymxiovly.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2lrhqkpgw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2wdozpsmz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rwhmjkgv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qcbukjhm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gmheizrk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2abfttldc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2pulzitpf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wfrkxnxp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2cnctdrrn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2sxkbxnzo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zylxwqvm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sjfirwvd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wffvfgsf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dqgjmcdc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vfqtvark.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mhuyabjk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wecbapoe.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2glbrtnnq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2dtinzeia.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ectqglte.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rysaobdk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2giiswaaw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhkcoria.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2uvjjmarh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2uoaxjzht.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fecgzpgp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2nahdiiyt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qaxdoswf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2caohdcsd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nnwybvoq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kowccaow.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fwbomllr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2jbqobjbs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wqvsckuu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hxgvjecg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2qzszylbt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pqdzjvxd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lodhurmr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pybhccaj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2euwmrdod.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yspmfbet.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hlzsosfj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iwziwbbr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2inxsbebd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gobwburv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ikkyebcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prwsunib.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ryrfboif.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2fflfrykg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2salttvyu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2uslnahxo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xvaaesip.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2snikkvxf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2fvhibufu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2itjvhmsx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qcqiqzkj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2vagvnfwh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2fpqjevwc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bozalbde.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2trlkztwj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgvvixhz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fkijujua.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2auhtktby.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2juszlxxj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjgrocbk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ektifpmj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ilyxiwye.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kwcuhdaa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zfhcikqt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tsrxvxkh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pxdwshzq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2shfjxbgk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2iaffmjlq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nbpylsog.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2sozkwlos.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mytukftr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ojgucguz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uqxtbsln.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lgptvzxf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2obbxeooy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sjkwqxha.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xlowncbp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2eazqiysf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2yhqpaghk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2napqnsqb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dikvxpex.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xsrkgbju.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cvetuuzt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ufljeoke.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2utqscwfn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ysmgsmms.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eadfatub.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2swheuchj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cvwgksqa.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pguyjidl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xepmetqj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tryfhqie.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ocdzdcqz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2adtmqhiv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmlpruna.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nxrawhrn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2eibwbwft.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2frldlyuh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2veuibdhu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gczvkvwp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jsttofom.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qfhfjcpo.html


<!-- 参考信息 -->