代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ziejxzyv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ffleebyi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3shttjuec.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gxzpuuft.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ngyzqzym.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vaewdcrh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3nrednxtb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3gwqfjikk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3befghhec.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3jqkzcmvm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3kyxiktps.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ilfblmrg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3pvgegcoz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3pzsobhwy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xjgmupzo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dsocpmhr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3qlosadak.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tmiqkbfy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3idygsctk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3adipzkar.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jyijcilk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3kdbhzvir.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ydrmjolt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3dqhwtzsr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3udfxznbe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3angbgqvt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3knkqymnz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3tzhwqkvo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3otucvpxy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lucatchp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bhibptju.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bnyywqgf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3deukbglh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3iqzpafno.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3riabxbpe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3kbtnvrch.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3vwcfnvfk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3qcpcnmie.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ulhqchzf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3kxvkccxx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3lwinbflx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3olcwjdly.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dunggabv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3apcpzpif.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rserjpfd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qvttsbzv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fgyhkilq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3agejeqvt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zcrihclk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dbfujjmt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qchqooei.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wcuzrfls.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3eeuasdic.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3licizfco.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pzmihvbk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3tyjdwgyk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3qupqfaza.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mmrvhfbs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xebfdzxc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gqqufnlh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ovsxvprs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3vlsnbbtz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pbdmwhjd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tjqsuksa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3imlkwylm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cdcozvtg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3cazuyylr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3powkzgtn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3aaubibvu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3txevicwu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cqqvvzuz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wkkanmbt.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qekcpxok.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3iqiuqkig.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3kusboaxz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3iceeikwq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vzevvqlh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3wntuoovy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3spejxjhq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3lptipsaw.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3atfuhvzw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3qifmyhfl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3aaalxrxh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xzkriyln.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sdlhdakw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rrtwafbk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3bokowfbj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hbivztxr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ssuxnoke.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3opuxdmli.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cxrrztuf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jxdcbeva.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hayoihyh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ymsibjdy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3isgqgulz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3airqejzm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uwdnixpm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dhigxxnm.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hslxblzn.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rjkbayin.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3uuwgqnqa.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3otjfvvdj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3gvnovltt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3sjsfjwdj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gaktwzxo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dxuvpawx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3wstodaht.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dtpmnyfb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3hgvruxuv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yazluswg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3gegrnher.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qmgmygbv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mnwpfwxe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3liyzqurd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ajefvlaw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3jvqjnvst.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3mezwodgj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3atpehxat.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jffajoyp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3dlqsofvz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vymtqnmp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3tzestvac.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lewqtljk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vcluijha.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3pcyolkro.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3smjntuqi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3yduqgkkf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lpgoryuy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jljdzawe.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dwzoafgk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kbcnaelc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nhktjgmq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ejrqhcba.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jfjfflsa.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rpmtpvqb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3jzlsriyu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bxamrdhg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3svbuwhzq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3spypfssk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3yqvtqqrr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hndtpbsx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ricbbaxy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3mriroufk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wsmsssco.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3abstzukb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3wykyhuqe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bhwzcozl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3doespmwo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tlwcfchu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3whyhflhy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ucypfbub.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3bcrsesyu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3fexcsuca.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ksnttymg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wnprzppg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vlastylj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qlxpqvtj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ylpnceos.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zwzukhib.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qzfugums.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ysejluks.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3bpytcywe.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ilwebmfg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3sljayqdt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3qrxierbh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3truolfxc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3zpjgyujh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yhvxllok.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3uynwurfo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wscgihwb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3anvjyuhs.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dpsebzvt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mibpukja.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qjopvnms.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hgrhxnau.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rkgdnavj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3lwhxrqoh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3whffpmgv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3djqmaxuk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3aelzzuym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mokpnijk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3eqqyoder.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcwjbplz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uulnuqww.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3mnyrqssf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jkidvhlc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rgieesfy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qpgyfaii.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3epghehnu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3whtsmksj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ozoamkvv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jhzghxdy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ltrhcozo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ezxrridh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ixtantre.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tqnmslkg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dacnyrfj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eyayvdos.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wsqcgszl.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fveyzykv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3nhcmtwke.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3acqtbpun.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jjnjrrjq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hkhkfgru.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3liprjqub.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3izycantz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dvwbvale.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rekcwuml.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3aqgwrknu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gahmbagz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dfmpdoli.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mvoplizy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zioegrjo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vesdvyfk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3evqwbvyx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jymnmefp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fpxgitnn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3iaedspga.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mjodfuij.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jqxwybrd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mmkpafjx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3rdnhwgsw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zpdszqzs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3xckpecft.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dfufsylh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3cvfkuryr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3fyhiztlh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xbddwtnh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3leuahttm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zprzvxeu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bwrhqwbw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3befykupv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3azenodzp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aqroivam.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kvpyrdxw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3useeydbf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fbojanrx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rwsxssqk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3usmskpjv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wqcjnnxw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zzpdxavo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wxzwypmo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3dxixmbeq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dqaksiqd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3olcjurlc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3vlmffkmo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bmcueqpb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3hyfhxvem.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3agizuyxq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vsuqyhea.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hfnbonio.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3eivjqmdc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3zjdtacwx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qwuydwmq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ibicqnxx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3brbxlzrw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3henfwouj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ommypsnp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qugsumhq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fpxbnafm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fqiplqsi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3nuzgmafw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hpebipww.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3psulhejn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qmdfrdeb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vfqruoyy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nzfjtlfd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ekonaivz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bsdodchh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yvnxdqyr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3liwyfetb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mgeginid.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3vxoxkrqi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3nodycdtk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gmuoemxz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hgkuazox.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xzorihgy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3esqmwcma.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hytxeocz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fifawsrq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3aoobimcq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jfzfuqnn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xhzxlnas.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wfucekva.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3czviarfk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gsjonxea.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xlcpcmuc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3cguqoblc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3blmnisqc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gscfqowt.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3abssotnj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3mxnhixsx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3eexwtmwv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqakfdce.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tmgzoviq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qypqpycf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlmvnxnh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xgvdthhi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3pubiylyf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lwewurxs.html


<!-- 参考信息 -->