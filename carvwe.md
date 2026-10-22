代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cmhrvivy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2vsplkvrs.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2nvsbrkdi.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wsckaxgm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2bvvhtqht.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pqdzfjyj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2kairiaql.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gmkxhaer.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rjwfhgbm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2cjjcdebl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2uyvvqgpi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2prupdgmq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tybrtqow.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2wketbuhu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2golsisyu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xmwoxofo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mllrahhk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qfwwzntl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dntnspbk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2lziyokll.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2apokvgqf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xuppnykf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2jbchzxby.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2kclxykfs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2llowkcsg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2gqyxxyqb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2lbwzwfsb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lcdmrrwa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2oksnvxsr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fycexhhp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjhpogqb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fskhxqzr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2wcxftazi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uqptsema.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wicxdcuv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2faajhxhz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lchpkygy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zblhiwdr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aojmxvgn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2quakkaoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqmhmpuk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ztwpvarz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2peugetdr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hsgktheu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2rsyordjr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qugcgwnt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2knpdefhc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hmkqlmto.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rlrjtkpg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ugtngiky.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2reenkoxn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aodaxpjf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tallatul.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cigvjrpe.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2eefzsqtm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rkuttjjc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vvbipakk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aenpbivy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2yvldwope.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gaqvkzjj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gochfahs.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2etbwhtrv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2zunobsqc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cerdqtwy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2flgmumvk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rritdfxi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sgmmgthy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2whrtdtlr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2oslbnhqk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2hioweuky.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2kppzphzj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fggolbzl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ggslmrwk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vxzpzcnc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ovpyjjcx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nqxmlgjs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2osxxuvka.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wkxvskzr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tqcgtvqn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2uhhcdxwf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ftonrmlp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jiincfkp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fsbrimqk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2hzhouumu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pyrihbmd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2haqukekn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ulnedonu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gwojqrdv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ksbumoae.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nkovahcu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2kvzmibjq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2awwawnxt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kfvaprkz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lauqslak.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2amcfcwjp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zxudebas.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dxbpeuvl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pvxgofmp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2fsequubv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cxdmylow.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tiswuzhs.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mtkcloqx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ckjkomos.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngsegrfw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xcjdgfit.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2sabmyiyz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2lhwcwful.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2tldalzua.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vhmlchbc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2szjfdwnc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2afohhcuy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vnsgaswj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2supmutnm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yrswdlei.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yxhxrecq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2zylymhwj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ovihcjly.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cxdptclw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2roajocwa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cawgbwhf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2avmuurut.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2nnhrsdiy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2fadbthkq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zssskipv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ttobazrr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vfpbhynj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2tbmzzvlb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2weqzwosr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yrixtzli.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2oqzhfdky.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cfliwuyz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2przzawqn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2cqjoqywj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mngzbjdp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xlncgwik.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hnptkggj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nvmnfarm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vqqnbkad.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qxaxwwkl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2duznvsaw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2parjstzt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hofjeude.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jpmarjug.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2voafmows.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ldcerrkk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2uguwcssb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lgllqlfa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ivinsbwh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2qaegqili.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jooqyaiz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2totodxls.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2egwjpubi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hsbrgxyr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2nvziwogf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gmrkgohe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2smpxhlgz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wppppuya.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nquuqyak.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2orpdzgnf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gmmmyghl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2aqbvxcis.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ghfmxhst.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ntpdupfh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2prjsancr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2dekzdzfv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2udasojqf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2dfzxvrwq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2moijwphl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pxjtraju.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2vsgsdsuf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nqlevihl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2adsjwpoo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ukgvothm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2nrdochmd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2qnjuetob.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2kxncxuqk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2fglyhwwd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2smgcdlsk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2teqxsjbn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wrshpmsn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2mdnbnhqj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pywyakep.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2alcjlfxy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zebgaxny.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2rhrufaam.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dlkxiwri.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nqwalpai.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2gpjjdcxf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wpykcexh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nztpxjrm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2upknotdl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxvusbee.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pfoykxyp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2kinhfkvx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2loqntrer.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2olillnwf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2cevrvpmk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2sfzxkaii.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ehxpfugr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ftghnanh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xcspmhmh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rkjiixgt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2poqrmjef.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2qstqfutd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cbbogvaa.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zxnzevta.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2mvcedcus.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2teuatzba.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kyozhoyq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dkrsbpud.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2pnphsnjk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2gwecftxr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yvilnrny.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2akzrerih.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2fgccuoec.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2pcbsqlzr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2iwjaplmu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ajlokcqg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzgcpmtd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgoaguko.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2stduixlq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2dzpiqype.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfdnstqk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vnsuhnop.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2tyjypoec.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aqdqkhxg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zunwrccs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lhzzxftb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2byelbplc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2yufdnjix.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wikncbgh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qhzdbrsa.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2dkdqmpzg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fzgtbhie.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xvjlzgxw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pugndmzu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2geabdqkz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nbkasnpa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2rxjeyxpk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2eyivylxb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2aqqmylyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uocovqgn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wdvcgoen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skmuwrjx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fxtennmm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2brtmtqwv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yzetzpqn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2gpajhaxx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2odyiqtlz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oobzfwhy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2wxktnbhu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hgiwlfkz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yvjeusig.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2lpabsvdm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2bcefwxtl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2bjwtyocq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghgtscao.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjpgsbbl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ulihxkqy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2yvlddtwa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hhabrwfd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2dyzgcguy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2unebbenu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2facacsqs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pbkfzkbt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tjtrsqoc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xcvtbmkq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2setgvwwm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ntnzicrk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xvwpciak.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ayyxncpw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xucqetdj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2djrqfgbx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2bmcxgamd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ojgqpebf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oectxvyq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2kvinexeo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cadlmxgj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lfyhzmli.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2tmfcvpjt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nexupluy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2zzmgprbo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ooaodguu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ejvnprtk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbzyydvx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bscvdmpd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2juldejpx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbdjhamt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pyasnojr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kchnsiak.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwxapvcr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nzinzflv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2isidavnh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pcgkrfia.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hvwsuhxg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xqxiumco.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qzhwjatk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hxrcmhnq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kixrjcdh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rdpisjqv.html


<!-- 参考信息 -->