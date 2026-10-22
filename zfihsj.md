代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lwbwivpz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2wlymrkgx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2tyeqzqre.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ghhkfvdb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2gfjyspba.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2riyxxfhh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vgbdmojt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2uohoskif.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mnfkoexi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gukhkaas.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2mwijkqpu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2prwprwic.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2obtazhln.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fdsqpnys.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rorythes.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2iwdztgmo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qrdswvyr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjllsxli.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2enknppqr.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hncgscgl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tjgttvgc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cvlwvmtk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bcddnhov.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zchgyfkn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ertrtsej.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vijuvghe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jogmvnyn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2curkltkg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2cknripux.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wtqqnnym.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2rbcpajus.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tjvjspgl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2jyrryfcb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2axuoznut.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ojciwwzq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2blhafaht.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2afrwegok.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2bklbmaxy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2efxbgymo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bbqctnma.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2qtzxbtsy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rnkpuuow.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2eckowvqp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hpcqrafa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkshhvyl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gsxmsiqp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2emhlilzk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2bsnitqpe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2cvvomlgc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2hkbmwwej.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2htauzstk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xbwrzrny.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2padyfwlx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dicrcmfu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2kynfagef.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkiglbjh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2rqhtlmjq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2taeojolo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ihubczzg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2arevjbhb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ivewrxmh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cwcanzsl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hnwjjzuz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yywcujop.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ogzooznu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aeggyuqx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ikdtdqfg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ygcobtbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqtiaqir.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2csxlzqsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgcxgfrk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oynwunzi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2hmqjbmng.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rmyztqny.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2prqxachk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dgopkxrc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2oepjxvex.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2mezhnhdp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2pgamkzhk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oimrmbla.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2nbcifyne.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lzxytwoq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2iztmqfdd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2acaossqj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pdijjhdg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cjkbybix.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ehktkaap.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2txcraons.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2klbugjzv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2omsqfbdd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2numoefqp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ujvaaeux.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fvwudowo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2egouchtz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mjydxdfo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nweedfes.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2cevcvgxv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2jkryqvbq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2dswruxqd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xnsmodie.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2eopvjpyl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2usybrveu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oadsspsy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mgokbflq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zevapdyc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lblimohl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kysscrrr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hmmxkjqh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2kfwukoag.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2gtmxaiuu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qbixenzc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2vqmoghdu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2iqsifphg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2gmiqttmj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2vmaubbli.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ptniqfxm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2rtmcafcb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2duvdwbzv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ohdoiesi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tmhmgevi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qwsrsyvl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yhjokqtu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iefqzdsv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2umqyrpru.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vrlgccup.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2uizzjdye.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2tvkgmgzq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sawmptaa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ktwsnyvp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ejhdkvyg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2pmzxiivu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2pexcinij.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2myyrmrji.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vgzhknvv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2sbvxxpqs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2pfduktxs.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2prrgglli.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nltmbfci.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yzgxrcoo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2newynnlg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2kceslsuz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pinmsrli.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tkjfrbil.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2qxncektf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2updinels.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qpxcimkx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kmtpctuf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2eawmdgrn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2znggztwj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qvhvaffl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bpyxalix.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2etqtkvpo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2iqqpxxpj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wrhiwimn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fxsxosbo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qdhqcsqn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mlhnycwh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rpzehthf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eujbrgfj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sqkzivsk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2jbytmwri.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gguvoyxu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ronenkky.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2phmzbyho.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vblnsaxl.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iqrxkdeb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ibkjghpy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2idppkvqj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2anbxxjwu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zrsybwwd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2dpjhsddy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fimczljp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2njqrvgzx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xufpdnkq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2yrmohyes.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kylkcdve.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2vmcqaqrw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mmhjdbcr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2kddzyumb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2kgmnskki.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ccswbzpe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbefkjkr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2azzwyqux.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2emffsach.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sbdyfbqa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ehosfwdd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2dverfxgy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2asjkenjc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2sccnfvqx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bbkmkbap.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2bhhijdqs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2emtsusvn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ixobtcmw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cgrqvcev.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2jmlbsndl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2bazijibi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2snarkkvd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2lldkcxal.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aspfejoh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2gybnszqo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2hayyhzju.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2yobgtoxo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2macmverl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzwojrux.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2moprkbsu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2mafeldbn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2llbnaltk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ozwvoyxb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nxagtspx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fvdrroxx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ieivlfpu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2goppncqx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2gjohglwh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2isgbpvos.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2eemuwpih.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2nonfxkus.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2fnnqogjs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2fzbiqzum.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2orllgofm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2icryzllb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wzcaodwx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cggitzml.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gfqaakiz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xfmbrftx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2hqmzjfng.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2oorvgpdq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2wqeuibfa.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qiecercw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eopiwjlg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2eonzricp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wzojxlqw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mfkkitkv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2qtinafmw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2vzpkapar.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2zjviipbz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2edznluri.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2huadaxwv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gatnteaq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2juyysrat.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2himtvzqt.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2zmirqaur.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vkovzaxy.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jraafora.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kcbdjcqm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ptobijuv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ambdqlwj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2pepazjko.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2isiwliom.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2cfyvbuls.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ngqcslmw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2nyjedeyg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kdsxckci.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2esrxirjx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2swfmstpq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bitbabui.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gdszxdtz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vzrazjen.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gqysbrid.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cxfkgqbi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jmkefqhk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2bkcvmxfc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jtiqcprz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tcekbzmw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2oobhnuyt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ilogzzev.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mfenksdb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2gwtgexem.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lftjkisb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mrbmiqcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cixcdnlc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2gvmoaayn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpgcrnsv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hzxohkas.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2qufjcgnb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ughdvjdv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2lyltvvmm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fmnabsgn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qwuwbksu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2bdqpweiq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sezpenfz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wfbjdpak.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ygxanfsy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2utueekdy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwsalkfw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuihqwev.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bjdnfubc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wjwamipf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qvqluwle.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2niaxtftr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2jdekdook.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2xwhighyj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jvyetimk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kzijemgr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2whiwgohw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mnlxiedw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vcvkjfvc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2bprcsbzk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2oxdnttcr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lunbndml.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2yywyytaq.html


<!-- 参考信息 -->