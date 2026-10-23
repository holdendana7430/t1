代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ithqzwtc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dzpqnagj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gqxanndd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yjlpdcgc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3inktgryw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ylnckmba.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3wdbcnbbq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jdvhvgjv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3smwjmvtt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3xgjflsxh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3izkfasil.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vtchtdny.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3fcqulyko.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3vnslmxra.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iwoujakv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3wrohnpvn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hknrvakw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jznbzzip.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ktyfqasz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jkcfrisx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3uswjbexq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3fbmzgjqc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3zfoynlya.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3eudxwyto.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3swsnnemc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jfriozuc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3zoravqwo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uvemyxbq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3bvunxipg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ppuovlpn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qzbjgomx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3icggvuox.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3oojymvfy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fjmcnwlz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3gmbypqip.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3gylqcgnq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ysyownod.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3eshuvzum.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3qxzehwse.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yibpzvbw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nsgdowqc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3uhilabnj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3wptwfnnv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3bitecdct.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3unoltvpe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3kqxudwqi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3vfrkgfrz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jremzbca.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nwvohazo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bwwqrrmw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vmifrmmb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pyzaicjb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwhdmvoa.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uipfrwgg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wcvnmhcm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3qvzxevpz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3glkmedno.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3lgsmclbc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3arrkmgho.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3dqwyafbd.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zbgugdgd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wrngxhfq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rthqoipl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3swzukjch.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3heunysaf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3oqtkshkb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3kzwrfqfe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3smfnhmcl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ocnrjrtz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zvijzhfw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lhrmufps.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xieybadv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jwbykxeb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3opkdtkzq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3swbteamb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3mkpblbgd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3pkvovkkz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ysksjuxc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3agqekpru.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3hufqmces.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ryjhdeyb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3rmfhebpu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fvxawxtg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3glzmqphm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pwpjgnhw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqwtehwu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3sngfukau.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hcxytrnm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3xqltletk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zwgzylrm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wcbzmbzh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3wnehtywc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fytigoaq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3scbehpmv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eghdctbj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zitsbiym.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tlvjhhyn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3eqjxvvjy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sozfevha.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fimtsnfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehrmsajx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3khuqlqkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zikrfoht.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xjmbxbfk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3hxobijmi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jwilngbb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lhpogloa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qkhmymsd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ywihtuhd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3khgnakdo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3cdgpopka.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3udobrtiq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dtprktck.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3oxxisltv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uhvkftam.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iuafellc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dtkoyrkq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yucnybrj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oqsegpwa.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3enociqzg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3voxohxvc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3awifooxe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ugvykanr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bfmraoke.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gjzvdrat.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qmnxzbpi.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zghtlkza.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3btlkluny.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3mcbzhyuk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gddhlupl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3iuyhxcyi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mxxyfdxp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3dbvexhfx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3jwkjcnch.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mkqbxqdb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dlhgxjrc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kvcdcarm.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hpsmzxtp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nqbtxoun.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ncmkekhr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3fmpwhuto.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3aocbykgz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zbevbiuc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zdukocuy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3holpmrfc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3djakbtam.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3iocgqyve.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wfluridb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3bzfzyuzs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ocsdmkwr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lpdhxwcd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bldextse.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lrgscqrz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jsugrzmj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkqywwbv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wofcwrlc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3umgozuxh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3qmfgvwev.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zljaizsc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bzdgekiu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3amxhleis.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3qeukymsf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3wliqjdsv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3hfttggtk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ojhwayff.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3deotalsx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ukigwujo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3cyomsrik.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dhynyhtr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3utgzyeod.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3htonpiif.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3detscgtj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3khbvgljo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xtjghtvf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ywkkspvq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vmkfrdrl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ueuaivui.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ipoxkyti.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3amzdwwgj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ebvcqjqb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lsfbolok.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vfjggbhb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xkbglxfc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ozpbpbze.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3govwsfvi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tbtjyvwt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jecuotav.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nbudufti.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rcytrzeu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wjvmpvvp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dqyusmew.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ivbjuzzf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3kvqevbfk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zoafwlxn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cwgwhzlo.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gvihpwhj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vahbzwsn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ahvsgxld.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3esfzgtbq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rgcgcywo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tzzrklop.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3isfsdqui.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kukzssrc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jonfyjki.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jpeowcjd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3oabhilyt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3masvljpy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3wjqksvib.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3bpprzvyr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3scizzbiu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ozeednwq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fqtdnwlu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3uygzksqg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3lqiqhqbt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kczfeelk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtoyedib.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fcrxaidd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oazoxgod.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ijytfrkf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sjifefry.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3hblkeegi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3zuqkgdln.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3owpqlckh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3byeowtgb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yjjuudad.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xnoyaudf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tvigivxw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ffqqijrh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yncxuxwy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3odaxwqhh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3vwoeafdj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lyqwczdh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rloozmwx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3qodbqwgm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3unqmxhsd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zgkmupoe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ksyusujn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bgwqsdak.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kmgcgkbs.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3qzutvwzn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3litigoyt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xhvovvgl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cpmanwxz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3crzmmzqf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3chiivcok.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fuqkhkpj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jhkjnegv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3aiytnimb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hmbuoapj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wusgotny.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fbrjhhjh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fzzcdvby.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3sgucksbn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qwlalghd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qogyoile.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ccafbayu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3iwbllyng.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3fcklywuw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wxtcrzbh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xijellmv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ppdeqaxz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oviuaasi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hgpgnseh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3imcxummv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xosbiktk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3xdlisocm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3nmurtfyt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tibugimr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hpyqmcsb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3inciomxe.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xogonpze.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uhakfujb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3lzwzjsdk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qjyoulhg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3zkehufhg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ajcmuwus.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jacsnqcs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3aitewyfl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3wemszzsx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3flnuirhf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rtvqakhf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3plorabcu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwtvyxne.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ruhhjqgs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3qroqbwvt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ruyzzlss.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hausgtxg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iyudukpv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3brhqmnzl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ibjtuhht.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eqkdqanw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3unzffdju.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qlrsemhb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dotofovg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gvndeaen.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xxmxkaom.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3phibcpbu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gvzrplid.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3awvtfwzc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bgkyohrp.html


<!-- 参考信息 -->