代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3prqqajch.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3nfmwhpai.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cnkibzvl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3edvqwkek.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3czyijpki.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3qwnlkpxl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3poowbhxp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3hvgebjeo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ddexibkr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3eadocmhs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3fozxansk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3bzpyuigf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ygyfwvjv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3mhhwnwql.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3zjzibhiv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dijwurfd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wcrmxnwc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3nolqckak.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3nmuitwiz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3exmfndlp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bvzrffip.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3xqiwzbjh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3agzwqkzd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3mklxrsoo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zdxtaghf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3vndxknls.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bgglgbrj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3sbuforli.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xubexweq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vxxhzikn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rgwsrrbf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3itiblqxh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3uhfolfjw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3wvzneydf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3zorzfshf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vzdroeag.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dpamreqp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ohbgzxbr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xjniyymn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xelhmfss.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yjexaarl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nvzfmgmp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3luuhjsqh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3fpnkcfrl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3zqpgqxyc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3tngdstjj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3pupbznou.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3pwctyuka.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ylaqlhkd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3awyjlgtv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3esxkubsd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3umpmwpgc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3wtpwdekn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3qibbuvlo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3pmdvoxlb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yhdssswu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hpnnqsyr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bcqwfwmd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3tmlpqxxc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3nuoxldwo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3rxrzwstg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3fysquwuj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3zydfmspb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3plcaqhka.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmhzuspy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hpnxdacg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3tbuafyib.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3cjojntaj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qznyoapo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3bzmpsdlz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mujwnmrj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3reewjlvj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ndpuzuvy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3okboxaaw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3mxatrtkg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ockpbkge.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jvjdnsmd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tujqwkmu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3shhagmgn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kloegpfs.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xspkjusm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gsxbrxug.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mntpyvhh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vyxgsvcp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qsfpijqj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kgukimyz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xkihqmln.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3playdewt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3duwwosob.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3phqbwyfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rslxvfvf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ahgnbvmx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ekmtsfdf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vozikkvw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zkchnhzt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bocrkvdy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gscppjin.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3hhekrfuy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3akdcopbv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lnndirge.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3hzvtwmhe.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kexssufg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ajkalxkd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3byqmwvoj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fttbkkew.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kwylmuxn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ourmfkmu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zjpnihxn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3zbnbdntb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3erjroaqc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mbebxoaj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3etwqgzps.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bvhcxyoi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yjrdrgbi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hytbkjhh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ycvqkymu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3zmoqamqp.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3shzbqejc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jgsnigjj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ajrspmil.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3qadbloac.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ujmvvsip.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jercpkqm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3roiazfad.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3msqykmfz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bjavxgwn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xpbevcoz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3pzbxjjez.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jpboskzs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3iqeuvmoh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hhpcwmvb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rhmrsdtl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xliuhzop.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kummupyn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3znuccfmy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bxcbanuu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jsjyucup.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hqydbafv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zfkfoaav.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yuodicfy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zovsaccz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vnjfrwuc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3labnrjfx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3trkbpphv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3etogdmsf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3awxzhscy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3swnpkrbl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gfgemkcz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3drabwago.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3rzttfpku.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3rostwcqe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jpdvvymi.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3cffhkjuh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3psmhdhwn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3cwiiimkv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xadpmmjc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3jgtfaziv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bqyhjntb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3odmxehir.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kbkqzmdc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3znaojoig.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3unuzfkow.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3arclilej.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xptshqap.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3jebjwpid.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wmpynnnk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3opicxjda.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3seldwwdt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3seuxfmij.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3zcqhdmcu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nvvmefxe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fobjbplk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3pnpqrfim.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bssqitse.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bwolnnei.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fjfvpztl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ouzutjgi.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ltygjwgm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xpwajajz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ubeukhcx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3gzcwtvni.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3djeqcmzd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nmsssofe.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3evjoibhn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3satkrupd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tliofwym.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3cbfbmolu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ajinvzbt.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kafwxken.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3anfrbmxj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vbdjomqz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kkdidwls.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3icokkwtv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3eixvtvar.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jxyvpjyt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3sttybzzp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3sdgtpntf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sdvtvdjc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3bggksqmi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pnxqfdaa.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3sdnynusu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwnyrojb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewhykybl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zfcomfyl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptqwscrj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3aijayxvt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3qhnmgnit.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nctmmgox.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3sduvcvlp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3kwqbfpxu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ceynkoed.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3fbscndyo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gwyifffz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cfftqgza.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3rvdixvpj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wlevsgqc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ngjrbntj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xyzkpfne.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xlwvbmnv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ogopipcb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rhezhpks.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3vjtfiwqu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pfgasnsx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3qhnixbfy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3yobsnyal.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xxzsguft.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3njjhcouf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vdbjulaw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ntdaqflg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bdtkwvpa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bciocvpr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tusqfhtj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3nifsgtuz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nsbimxwl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gbdasixe.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3mjjaaael.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wuffknrt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zafkndxv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhlvverm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qjlrmoka.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hiwmanjv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3amutzjrd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3uoiqdeai.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3uksbhivx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ceocupxr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ofsxtasd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3apxluqkw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3atsqreqf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cufrvmrf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vtzbyjgq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sxangojr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3dvbggabf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ecsigezp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3nxwbwqnf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3mdpgnaey.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tehnelrj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fbkmxnil.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qwkaoyat.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iofunjcm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3scjkmmae.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3shbfltyf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3crapmjxf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3vmsikoba.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3fshjwcxi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3podutgyh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzwkwmcw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwrjyhdx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhcetise.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcqzhfoo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zlxqdtsa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yexyzrvr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3iqukpbaq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3fdbnfplc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yutldpwt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pfwhbmuq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zldifozu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bcishdsx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3rhrdivbk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zentcfgc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3coluxexm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3qayiaofy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ffrzislq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tnidbodl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mdwmzcze.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sgjosnof.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dfthovat.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jchkxqgb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3athuacem.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gkdvbhqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrgrveab.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xjuckgff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjpticgp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jcebssvq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3frcbdwpi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ulydlgon.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3zxghipuy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rovsicky.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ujbpuptv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3aouzfdtf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hpotqofx.html


<!-- 参考信息 -->