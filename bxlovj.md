代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jvkowzet.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mrszplsf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3aqalgbzo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xuqaomvl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3itirtocc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3nhpajnom.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3irlzsdzl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nvvhjour.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dritgpfp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jlnialcs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zcgufoim.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3uszxspwq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3kdwmymut.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3wyvgdnjn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3untqjaol.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3jeqwebqv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3prczdmvh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3afiudbsb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oruxdkhf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3odsazrhy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ltzemnua.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3enozohsi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ndtqnwxh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cbfjujvk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kfhnmjzx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qluycvce.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dqjafmhv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3okgvxuoi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rgzuwwgg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3znnajufr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3iqmagkkc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3bcjuhvsv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3likbnwer.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3kfovofya.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ozjhkgqn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3yhlewixj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gtqtitiz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gmcqveth.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3codqmffi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3vqzhivms.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vjulngbs.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3gnkhjhxx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dboydird.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vsnwojmm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3oqcieugx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mhihojoi.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jshgdjjt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3teyomuqq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qfpemlqm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jbictqkv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3xmbzecfc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3tfgjlqvn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3qfkhnrtv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3afkcfogx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3sdwdorkw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3pdsifwuc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kvblurcd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vyzgaiko.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3nizshbzc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kmcmxvci.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3lataxpca.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rqqkubiq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3wpqaskpz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3zatjluqu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gekesdjg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ugoqvmat.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3yakddwwf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3uoaqaxus.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3qhgdovtq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3bpzjzabn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wcriilkj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3cpehuwym.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kcikyvdl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jrseooct.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3zkpvdvng.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ehqcragm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3qmsmksxm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3jnpwtbjk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3zcluulhv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xhjatbuh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ekdjajdw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3imziagqg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cduszwnm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pfugdpgb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kkqqthqg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zokrgkus.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3afdrlsoj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3qsrlpplq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ebplcswr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mgeheruk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oaucvgnc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3lwtjntva.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cvdfedlm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bojclvjj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wmwwskjl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3akbuyyjb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jovvehbj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yylptnnl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3thfwmjbq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fdibnmvy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ibkyxeeb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3lnodxcpg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rgfcrjlq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3guypkbas.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3uiwmuleh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jcbslwsj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3sbhwexrh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3abtqaprl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ylwhvfws.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yzkyikby.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ftfxkckk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3sbcpbjsp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3atdyfolr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3vsccivhr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3eukmevuc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3vbkntshj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mkhfzyol.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ueifsjbm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3hsbehdkl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hhlwncul.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3sknyzjon.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ppmccqrh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uhgwswmx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3tpujxvvl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3oyotjjtf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xeocsbcr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wxpkihsc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iowkbrmv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jpxduspm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zoaekous.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3thpdufgz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pngxiazj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcdimqnt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3sbhkisbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thaozdst.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vjufqthi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3jdmnkvje.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ymsavmoa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hjujjgwj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3nppgsyoy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3qeqcmyis.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jbchxubd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3hujhwycu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jovbbncs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xneatlyg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lwipkzau.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oaulabzb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nswgxqyc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rhakleyn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yrycotaq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3nenpquqy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3srtceuuy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tvbckfab.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nduvzykt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3sgjazlkl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3otjdyrsd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cilojfdf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gwhmoheq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pwlimvgu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ybayvezo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qldoanfd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fwwxsrew.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3zlrgcdrb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wyfqpmnz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3oxuluwkj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qgjzkcoi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3onwmsfwj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cafodbdi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3yvdutpur.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3poaieona.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dsselrwi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3olkggfsd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bqhsuxni.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3gxtmsaxl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jzlroxgm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yaixxrqi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ddqtaekf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3dvvrkfzp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yuhmlvca.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mcjtizju.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3nftvlibb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dbisitmi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3jwrsmhml.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yrpoomyk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3endaxwbw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qjqnjlmk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bocwkzjf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rjxrhefj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ysmeaxsq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wzazwviz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hsmrkljv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3acttbflz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pxdlsgsf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mrtktpne.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3mcvampjo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uofaloeu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3qcdkdqxo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3takonemd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3azxtyqba.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xacjbhfd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qgtoebsv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sigcgeaz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lxddtbfh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3credbteu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ooihymlm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ecjhcwnu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hinmzwix.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3nkfljans.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lcchfrjo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wkmkclnc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qovlqztl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3evixmain.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ydbicyxy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3hflrmdow.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rttcawei.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3knabkiof.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3esmijjhf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oilnkrwo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3lhzbcuhg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mozrxvql.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lpwkpyxr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qzfjpfmn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fpkpmbrr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3chhgbpwv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3topkjjjp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3sptklowk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dvhiltve.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nzlvkcsm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kepkxivo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3llpntwbf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ivusurvf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ketdtkqz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3itjxfjll.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cffzcfle.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3lchlypot.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ilpamknj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3purmntml.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ixqqorzq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jywyiqct.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ltlmyooy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3knhqbmfp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ysdtpdnb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3uybvsclx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3atcadrls.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3yzmpzkgc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbvnqskw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvsglbjc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pybugjru.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ayteewtq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qfimvtlw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3otaoghdt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsqqrxla.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3pbgqvenl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3tlkurttl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lpamklwa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3htfelkpi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3vujvikix.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zlmwagzc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3avmixuek.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3fjdgxwbn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hmfekqpx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3acchpoad.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3stkkfgit.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cydwbqzj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3oasqobjx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wvpjazgq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ydxmqzkm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rtwynfas.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmhqeeyp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3qqrgogvt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kypzucoz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3denvbarq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3kfqwcftv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ijamtbuv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nvpetjxl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kvvbpnlo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3uqfpccph.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tsecybmm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3jugrjtaa.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3bhlhlzdc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3jnwgavip.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3twzbfdwp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lghyvpll.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3palxjknw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3xabjvpea.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3suudiduh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xnfuriib.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3cahakrgq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3japkfmoz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3oxvqiehd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ushkiesm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ykkdcfka.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ddcygosb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vnfboamb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3saucyxom.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nytpzccl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3farrgugx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kkrumqci.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3hgwntzvi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ggieyslh.html


<!-- 参考信息 -->