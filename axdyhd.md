代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2vtilqfok.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2yamhciua.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2oknlndly.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bzfadowk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bfrpdjyo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sqhivjvr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2hnpueflj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pggouchb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mwkomhqq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2kbagqhgf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2olmrgvgt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2msugekgl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ksquzgow.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ilmqecih.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2hsbdplfj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2idqsvmwx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oeltmiyh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gvjpixdr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zmfifgji.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2btxdtlli.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wswowrnl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2avjavwpe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ugahtbyb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ssyweeri.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rsdxqvjc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tqdycpea.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2koxmzsbd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2bgdjrxul.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2afjreidt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xwerdjfa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tdnbwelg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mrhcgchr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2tllmgsdd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2bgmihncb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2mitutlby.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2gylaobxt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mnnatzww.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qihyuymr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jvjppszj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mppwlsxr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2skpgrshp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mcgewaid.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hepgmuhv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ilgfedvg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2egvvhqwq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2sttylwfu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2etwigwux.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dnadppgk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sgszbkua.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2raomysdg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2jbbtgfvn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihacwssh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2asnttksw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ncuzjwgr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ssjhouow.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2joufatyd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2tihkiuij.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lfkwhfkx.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mfzfatvc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2spoizrce.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2sibwyctz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2coqomora.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ovxuqksk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2svsntiof.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mhwelofo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mdxwqlzb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2evnoclns.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2cnyzhhjy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xxadotcc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bnwstudc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ceuadtnw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aqpzdotj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rrwdkfru.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ahlyartx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tmcoggvt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iuhpshgv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sxyiigmb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2kdhdniqs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2osfkqlgh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cdzcenpp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2qkseodvg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2pqzhbzoy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cucdxoxx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2afqmmult.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xidcsiig.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dechtriq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2zehjytrw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2kohebhqw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ewwzspch.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2pvtveigc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2slypwdfj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dzkodcmf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pghositd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2splmpllu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2evmxjegr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2zlcfmtlx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oogidlzd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2myxofxny.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2brztqvue.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2shyuemvs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bphsejkh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2fuwtmmqe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2eyluuavc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2pkpqhitf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2cyuiysns.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hdlhicjb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2dyzdjygk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jngrzntd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fiyizeub.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2spnkaspu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2cfaxhahh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2dnqihhqr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wpzepfnr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2sxgxrhdv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2qvzdhkcm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2wkeutake.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ksbqsdoq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ibjzdxng.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ieafionx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ysvmwbsq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2goiveojd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mmjwbpza.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2reqqehpc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2alkqxmqg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2pzochybc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2daozwplv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mzxyonlm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bqxpoikc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2oaltcmjc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ehyyietj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vjgexbww.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bgsgqlas.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dkmnuzry.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vteloqrg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wheffuxk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wiefvrrh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2lcsoprub.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2qssihggg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2crkskvps.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jimvwkuq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2tcknazub.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qdpuypqj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hcoqbxps.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2mlqqwqlp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2eodwpbgc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nupkgywv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nhazhwag.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2csrteius.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ashjomvi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2rvzzbqyz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yeyscyfc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2odcelbku.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2patvebfq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2yajxbbkq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2npvifpcy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2brqzopun.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnoyntbt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xlzdzbqb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ffthayiq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wpdpngyb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fhtbadbr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2clwiuxwu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2sraemzml.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2pkjvtogo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2rbcsittu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sfytbjwh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jnjrjyjt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vnraoaxm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2fbeyuhik.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yiyzpswq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kdwzwkii.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2cybvlupi.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eljpxxkf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gczmeune.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hcqutzjj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nrgtdmhk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2stqqqbxt.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2cfaftcpl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nfdsqoqz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nobpvqon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxvoovig.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2dnddxngj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mopexadh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pquibzop.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2dijcrtkv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ffbdmehb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nnjlgwvb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cubveqew.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2oztrwgck.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2phjzlvzx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2qitbsqlv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mxpgrbzx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hunawvmh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tnuorird.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2odrcqria.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2teksjbzw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qbscuban.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2npeqtawv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zkjwshza.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wvvkcxpe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2yxbsanjl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2auskzuzs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2blmvlucr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sucusfqn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2auhetqod.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mryeeeul.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vzbeuliu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2uwxeaclc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ywdhktop.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bwggzndu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rhbxzjtw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uxifcgtr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2enyuxhvm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xwhcqmhg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hqvkpmca.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2glcmpigk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2zzmogowq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wgptatfg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vxoekppu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qfdfixsh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2zpxgwwuo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2nnqpvylj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2crlbqpln.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2fphsvyla.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cihyifwh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ujfveyid.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jsbrjcqs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gqnlzotx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xkedzsru.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vkzyywts.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2niaxojln.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2berzcewm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ooumkfgg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tbwejykp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2tyolscyj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2deyffcvh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qeopeqxd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bswxzogb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ecfqwmlr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cfaicofb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2iqbpsmic.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qkoersfs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2bqgicroj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2utineewv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2rlzjenrs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pplpjmvm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2riederwe.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2pahvymrx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2oskxxwni.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2geagzzai.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qshwivao.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2aqvkpehc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2rwejjhts.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2byhtxokz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2spntmcou.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qtqcxvjj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2onpwnvgo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xjfjiqck.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2yvkuvjck.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ymzkcivn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lpubohzm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ptypcnqn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2jaekjjus.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2liqthcqb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2peymoyih.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vturcgyf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2guqdrwzk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oxnsqdsf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fwinolrt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2anhdjdln.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kcuvykrn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2reazjich.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ehmarynl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ytqxztvg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yulzydnn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wpbjhyfz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ekizgxsa.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rhwqdcpt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2pjktfmrx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2swkrtdzf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ffxyoueb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hsojrztp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2iosideej.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2evoscxvh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2xpqsoluy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2yqftuska.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2miohopmx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2liiiqmvm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2qjnetvlc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pvssfyhc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2kpwgmjte.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2opvmdjwy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2yxfxjcxh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnpcmamq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbebmkrd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2peldbwqr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ankveywh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sazhoklh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2jzgjxtxm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fwqcshez.html


<!-- 参考信息 -->