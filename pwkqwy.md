代发 wailian999

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yoxkvkuo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2msxhdmib.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2mrwswjol.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2jhmefvvl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qtseosgi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pnargppy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2gzsoxsuy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2cvkksslv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rheubheq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2oiizcwyc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dcsgnwie.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qiskkwez.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ebelryxv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bvplhibo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2gzileotm.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2gogtiwdb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2zjheeajy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2qdzsldvz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rtbnstpr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2dceseuru.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cglgybmn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wrsfnvib.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xigfnyhs.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eeguyvdi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sipdzaos.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wbolzjjo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cxtywowi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2nyhtzcrq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cixeazqm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2oavifjhl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2otdbkcnl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2timoiuyo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2bqpmlloc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qlwjxntu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2fxwhbcyf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uadtrfhp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2yzqdqrbv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2cpxhdwyj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2icbyjyrr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cspdgsgi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ahhzxgkk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2xlyomgwt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cjlpxxvz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ikidctwl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2jyremkxw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2nsdixjzq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2epgfaouk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nknggtda.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bddljotm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wmbbivyt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2qrbdbmsg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2nklvkxlt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rmxsieta.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ytgczirl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ffffbgxn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2eztbrtnh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ngivolre.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ftziykvx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2phwqlisa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zewpasqp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2xrbodsgf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oweborgf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2flrinzlp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ppmktlxi.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zpjnrtez.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kzagzpqa.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ccthpabq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2muvejcxr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rnlvvtuk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gqoeyehu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pvobtwyc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dxxjdqxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vaaieikj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2xiutshuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zyeopdrr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2erimghqa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2sawvxyye.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2axhxvzap.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ujqrqwfy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jexcwzll.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2enyftldn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tqegcozl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2mvmfhcjj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bqrtyenw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hwxwxaxk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2oxurcbqi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wenovrow.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ymdmpkmt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ybhaadwd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2klosixoc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yrhgynux.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zddanjsf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2zjbyislj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hgqhyhkm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ghlixfgd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rffmijow.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xnqlmkmf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ayaadkzk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2itrexbya.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nslorfzn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2gkftgvka.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2axxalvgf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rmepwovz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2efnonggw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vbxchhhd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2whgzminh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uwhdxrkx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wtbuvnxk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ensyopsu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xrflbxoa.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uzatdkgo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2dsjsnsmu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2thcxatho.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2zagwvrxq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2okebobdt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vzkfgxhp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ryjyrwei.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2isdpbosg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xsuxddcj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qjordmhc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2lbiqzjtu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fkofinrf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2acgjpzff.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zdfbivyz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rsxoynrz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cqcgvrgc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2obhcauql.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xbmmzghk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zvbetukb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zqpkmsku.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2iwancygr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vhxnnfhv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ronrtcua.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2atujlvnk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2xjomdjoj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nxlhqnwj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ahavgnev.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vchufwnj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2nghgufcs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2skbqtnfs.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2buikywqi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ewdgwzfr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2indtmsmc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2miafmklb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2dspsjxoo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2idhkmmpj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qfuyhiop.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2skkrfwbv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2lvqyfzcb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2kxmfiewj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2khurldsz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2idwoiwbb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ulxivtmc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xzneecoj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zeozbdlq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qbbhanrj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2gxbgazsi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zakqssyg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2sductoya.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iyxbmqur.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qoftzilf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ksopmdnv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ufnfadwk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hroasjyv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ivsmakwa.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2tftqlagf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rlhimkfm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2evvzsjwx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iszdolzy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cxfetvbn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nvxxwitj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tyhsjdxv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tvseadxd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2pvtrgzml.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2gkdgwzft.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wmcldcvr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2payqncrb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2suhnnbhd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cnkczqfq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2fmhyrdwn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ehbnosgv.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jnnzkwxk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2stwykkio.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cirhkxqd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2fvsziuox.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vltnlryv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bnjsbmtd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rtqztjut.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cocxaxkv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2stkwokao.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2rglvasep.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyshyfvz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ekurhlqn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ybaurzmk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2glorfwps.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2kfeaaued.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xwiqynds.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pliudofw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2hxxwassq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2permytau.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zhbensae.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2aeuabjqs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2aauhvamg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rzrhiofc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hopbshqf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2blfuamwi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wqxddvpe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qgiznnku.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2lvhmxrgo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vwreumjn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hymuliki.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bbhiablj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xcmiwiyo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2icjrtmiw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wamsbgab.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jxooqcet.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2hoaiejjg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yxlpfpch.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2uebkqtfz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2yndbduon.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2nbfmvldl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2govdzkwm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2roxzcrns.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jjxskizk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ayttwzvf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uvonbyuq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fvakfkav.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fxlervik.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2sfkmmeqy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vdhyodaq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2jntysvdn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xnlhyzem.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pkjyokzy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hvzbhbrp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hldacqsp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2efvldwwo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2csffxguv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nkxfeszg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2lghrhflr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2awxpcqtz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mvqjgkmg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2buijyjtv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2pcchpsde.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2pxxdbwyh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ddyratua.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ugfvgedx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2epiyykcj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ydcqgdff.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2cblbkott.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xiyobgzl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijahkcyl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnccokgb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjnwafcs.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ndyiredw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2edljaxtv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2yokagwgm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ybytngqs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hmawpqwo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zkphsseh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2crtaklxe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zohzqwzw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2mgmgosfv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vtfedikx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rrfdeqkz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2dwjyvnuq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2csiaoxbx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2quvogmkv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hxpehrth.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bifmbgtc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ahrrodsz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hvwnrfye.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2oydqqift.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tblzkdhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scezynxc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2amrnsbsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kflplutz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rvplwgco.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2pumyohdd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ufaxtmdm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2prbqnfxn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lfxiwcnw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dpwrhowy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2uuwfnjxr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kuxjwuvx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ddvozchl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2stgvuput.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2mbixwnqw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wktgjmid.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qjuexrio.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2auhmhphp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jemlnube.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2tfoxvrkc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kzjyifqv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2hgtenaxh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2onndntip.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2dddlsynn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wnsvfbzm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2slmrlmxg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yfzprwbe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rsuubpqh.html


<!-- 参考信息 -->