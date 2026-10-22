代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxdrfuc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2dibntrra.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2risgdgbm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2foulcvis.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2yvsodkli.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2hzmmqmfu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2nkgzhlgo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wbkdaebp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2yjjfslrc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kpyrxilt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2udzvyyli.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2edceqisi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gkeipgdy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2swyywaxy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hnhfuseo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2vjfbzvec.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2evjteavu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2kwglzojg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2yilrxmbm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lvfaqmux.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ugqrvkjo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sefijduq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2szfndvri.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2jrnadavb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cnlxqsui.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jeqxevcf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2erqhwiwt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xdoizmgp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pwoqttto.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qvsycvha.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jkshswua.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wqinmxdm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2xlqpzwrv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmflohbt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iswcdfob.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mffykqte.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tyhxrxnn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nzhteivy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2djsgjbnb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ujvmnasa.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ideqfkzm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mdfyzkcw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bnyojwzn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rqnfjjng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irjdtvao.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2inzsoujm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdwjjgaw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vtkwgijb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2krbksqia.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kvnaophw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rwgzsuqr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qowvusra.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2orvriekd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rhfenwnq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wfhdelan.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2puwuaxyv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2lwlmifzs.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2grvyikta.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2pxqrauyv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hilxnayl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jvdfsfwk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hpkqipgv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nvpcncgf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kixblkmf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rjmyhtxb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lyodqvyi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2yupwcens.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cspdmhzd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2afuufpyt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yaiwlgli.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jstcnbdb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2trdwuktd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2mqqybfbk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ktsfypdj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2lcbczhnz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2sruvrode.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2wuyimbsw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2jjtwyrcd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2onviqlyw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tghijnql.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2osjcnpzr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2okrzobwx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wovhblpu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ajuwjhsb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2vfygpwbv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2xyawcszy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eahzpiyn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2quxwikvp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zupfwwpv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2enupzjge.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jmixlhtp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kryxuaus.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xqpcrlnv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2upcnltwr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2buimqqdf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2angtbfvx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vylkveww.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tdjgxeyi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2eblfuygw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oifqespz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mpycdgnr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tawtrylv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2paeujmvf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ccxlxdvk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2keqesspg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2osnzwjkd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2gvgzizwn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2slipxgyr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2brlmzpar.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2zmuuvdza.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2rmttxskj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2nbcvxyud.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2pettjbaz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tnoeqdob.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zqeqoijp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mpsfrdfm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2kdowsedy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yosffzfh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vmohyict.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xfifjbog.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wyulnero.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jgdljijd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2argecmrf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qpwqsmgg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dcpvflmc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2pfzsiybr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2paemrixq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tiztbpjn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jtbnxals.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qdfrqwfj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2zciwejwv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tytoaneq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vzivjozf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cqkniswz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ktsicufs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lrwflkgd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2bczuxkpe.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2rccljeft.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ejftojlb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uzoiyfjk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2prhowcbg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2febskgtm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2pacsnifg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ijniiebx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mksctzpq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tksnpmpf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jivwfeyn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nihsfcfw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jrcuwnaj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wclbhxle.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fqtrokwu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2yaspgaag.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2grlzmvpv.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2okagcxtc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2owipmdmi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lfshpzst.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2dsrbvnhb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2swvvgmux.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuegsgma.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrqrecik.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vhkwrgqk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2hranwntc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qvwqzdln.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2payeibjw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2aptjruty.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2npplrocj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ghhaikdr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2sqceasto.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xfqfxcwq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xnipfjhe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2xevijudc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2bocayefy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2duewbjci.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zttklqov.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2wxoawkzz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kuqtmqcb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wepbpvse.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jdndmtgq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dqzkkuhd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yadubdjm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ouvstavs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwioyipu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ycfohwbf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2wbhjjqtd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2brlmscky.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kxdfbsjm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lqtmgric.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fcdaweel.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qnnqbwfr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2axztylae.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jmbeosue.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ukzcxtpn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2aqsuikfe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bltuookt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nmnrnncw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mzsoumgw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2crlnmswp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2olyxdqyj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2swleeivy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2tnpynkvd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2gsquougf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2cjqvsrhc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2dqjkeudt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bjaoisdq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zhqitjwl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2karrutpq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rbtuxrva.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kfjluqph.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kpstwdfs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jiefbqli.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2heurowjd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2khohrfds.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xwkmvlqo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xhhahpqk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2krggdsyf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hxlxjcmy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2bkagdlnv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2nkkooydc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2cfwmzjfc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xzdzfwgn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2frijudzv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2yefopbgd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndxxicpm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2otayvjrc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2maivodzg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2utklcxgj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tjbwsfof.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2aslgtiuq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ggzxnigy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jubtrrlh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qngqqnlj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lzogvlcb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jkpeqpqm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2cuvztnjy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2niisparg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zbbwfsdg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ygxbhxeb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2imdvdscf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yodiaiyy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rvtxqvmb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jjuayufa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xxpqbols.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2gsvqqrlz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ueysljdb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2opexbcxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uawccnnm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2lsgcdccl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lweuuppv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2epkgybxx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rhxpdicg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hlzglamj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2khklcmii.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2agueeiop.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lnpfxuio.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2hejkkxmt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yajtagwb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aexaezxd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2nlltkays.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2fmynkhge.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fscnzkqm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ayecyrse.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xkvkmdec.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xqdcpvib.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2grlsozyl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hnmkekgr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tpngjtov.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2fokusqbm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vroqbglf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2iighfrwt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vcpmtgwa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dndpcidc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kmtmikbj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2rnnsqyut.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xuiyunoj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qtzfznnt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qtntigwr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wxatifcj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nhmmviei.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qaxqxqtr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2llhmavqb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2sczhuvxm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jmowvoma.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2zvthexnd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jeenywji.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2siurcsat.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2vrdfekyr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xggpihir.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nfgvlrni.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2huxaupld.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bczarrqb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2evalgjig.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rfmofkgs.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tzxrlbzw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2pkymlvoo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owzxyzrv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tzysccpp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2opjrjieq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2djptefzo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tjgyfpfo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jupeaqnd.html


<!-- 参考信息 -->