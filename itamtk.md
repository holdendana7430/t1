代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3lbkexzgc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3esinagsn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3exbfkrpm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3iiccqjrh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3aaqeeivy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3zpibsklg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pmvmwxei.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3uwszpnso.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zkdczqiw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zbzyeyte.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3srkljeos.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3bpajrvvl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dufgbzgt.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3nhqizydn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3skkxgjvr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rhusvgsl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zqbagpop.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rmpmsprb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3wkfjjmsk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gvnntxax.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dfjvxsiy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3bgaenyyj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3dqlfwifv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3koztcefo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fwvxlvde.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3shenrxxp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xbzlhunn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3axifdbxp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3hofdvzcu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3jwpninvr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tgngicpp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3gtontjco.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kvdenmoj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pfbqjcvp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wybwrjhd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3paokjmbz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ijcdfols.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vvyvwvpn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ezrpflig.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fbvnavyn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3scufnfag.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xtjpyivf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3osaundnz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bezusbll.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gyyxwkzp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ugrwjybq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ukqsbqfk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3sffwqmic.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pjoiyzfp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3jvptzxvd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3efblfwjv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jvysmssj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nyjhnzky.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xetbhmxl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3cggoiyfr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ubjrkpuq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3eisqysoj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ponnhysv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3vnctyult.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mdtmtmop.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vvoyjfgk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3kwxylepw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lgoroook.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3sizcicek.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qxydupve.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hwqjbcbb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3howpgcei.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jywkjjwq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3bgymelzw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3qhqhlugr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3vyuyccwt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3rvuvlnzk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3cturavln.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3klurynsx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3zctodjtt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nuccrzut.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3fwcmikfo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3velhrkqa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3dtynrmdy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3dsrtspdk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3iwyjkgae.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3xamgjxvt.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3hpzacxmp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3reheqqtj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zbgresym.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3oehtyywr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3bikkxgot.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pbfobqll.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qiywotpy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nhlqgcwp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3kwwswqzl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3frbplhnu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hsoyjfxb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3hwftmzpu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3nnvbwowi.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3oyxzejzx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3wufyjjsm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zyhyrmvp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xjwjmlut.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qkuasngq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oafqcefo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3latlupnt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmyipmdc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3jdyjtxyu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iccjgsqf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3dfbiavda.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zhpuutwv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3eaotqmtw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3owpeewbm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hzxxkxnf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ovponuyz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pflmbzlj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3qqikpfoh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nwzzufeb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3chyrzbzr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3neesqssd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hkhhqdjc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3guqpmmcy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wvqrhytd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3vsvvpngu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ssbwmwsx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3brgkhnxx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mvjfbymt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3idhmwimv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3agfkqjhr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rrifmyrb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mplfxdpt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ynsltlqr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ajwkcxty.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3pptmnqrx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3tnkufkyt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3luhiotsn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wyyojvaf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3vhazkptt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3kmzdkgdo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oyfuoqfy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3iitoefhn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3gosjxsgl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbxfrllb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gqwddanz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fpzlxvod.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3grprkxro.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gdriiiuo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ujqczcmz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3sjvbdgsg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3kailuwoq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pthtmxob.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gpeigvzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxepejrk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3yrkvmljf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlpfhvaa.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hzvalxqm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3rglgtgyw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3njfyeiee.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3idrgkfnb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cojiybpd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3vvqdeejr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3idpfwuhc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ukydkkgp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lbgxkjdm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3nqtzsxdg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3brlzicah.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lhapmcyo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oifglrhz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sraxsvdd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3levlwtno.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3nwkrtcgo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ifukrrak.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ldyafgqf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cbigodvi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3izwxpzuo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cxqcmgij.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xxuwxcea.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lmtdteyc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ngbwtknz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yqshfkqy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3yxtrgbbh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3skgzqkim.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xsqxgblm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ynrwjrjv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ttftwvlb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ltibdqgf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hucskaxl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3truhwund.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qtuyplcj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3txxflozr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zuygknbi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3yeaaxwzz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rxarytsv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xtqnvcsj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sdgiqyue.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3rbbmbgds.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nxsamkzc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ngnoauxa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3itwumsdz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mhzvhkpu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3rtyojqgu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pglierdj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3qsaefvvo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dsceomep.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3emoypnsf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qhuxbjox.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ktxavcfu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3meacipcs.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dbbqkgld.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gtwqpdca.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3fsexwack.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zibzohof.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dmbphlei.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3tudlglak.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ekhltjpr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bitozgqi.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3dtznkafw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3bjckibom.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3daqgxodm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3lkgxpyvq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3znsphymd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3faqxvwot.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3uvoyrchi.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xsdvytxu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iatibhue.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bfqjaoer.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3egnuqydw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3cgzsnkmk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mpmmghjm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tjtcloan.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rcpnaavq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3blledbyv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tejbfmoy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ndzoqddz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dzfqjjng.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3acdqsqbm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ycmclfjq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3isbtango.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3bjmwzagn.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jxstlznp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hgvisfdt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mymjbgnd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lslbcold.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pxeqyars.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3fwamfdvm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nljhsbpx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hotqpxiv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jnajjtsj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3etyggbtm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fvdcmjok.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lzxbfwdv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dokdfzwj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ozwuyoir.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3brwgbdyd.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hnjdhind.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xsntwxxw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3xkeycgkj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3maituqmi.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qfamulkp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3blzlmloo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3lpcsqeps.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rnszclyr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3icumxiyj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qhyrmyhe.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hhjddzxw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwcdtkgy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3snzraxkg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uibwyyww.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kggndons.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3whqfumuf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jdjgssew.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vbhmmwqq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3trlyuftk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3puxowtug.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pqdiybuw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3kaosujgq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zrultkwk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yznztenf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3iwwjkwnw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ctjwulpr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3eqjjhits.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qlxrsfxl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mrfohxra.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3opxpdqah.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gnljqutw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hapcrhwn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3exxrpcwt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shjdealb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3pljcqigy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3drqgcjmd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qmcvwiwo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3xvpwlsau.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3nhhehdae.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3boakhijf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yvsfuawb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ovzpwqyf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wtmblldy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xsdyeoyi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3dkyochdy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3fwqkbgnx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3yhumthvo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zjsnjuev.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yhrdebur.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ybtzbrrt.html


<!-- 参考信息 -->