代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oqfsijla.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qbzakjur.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2uaxevmeq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iksublvg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2belsncvl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2acqvjnzi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2anustkfj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2gvkswovx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2syvihrpe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2txsgtdnn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2exiuygyn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wvrdeoyu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fviohvaj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2aemeyytl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zmrzrxvz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2geuqiecu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2shfoogcs.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nmqvsvof.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ytbayxgm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2skxziown.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2kgclsxjs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2vftdofkt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qkajuriv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bpfyitly.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qdhvvjok.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bmpyyctw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2sobrkxmf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2cyvphgrd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2oomizwpt.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2fxhgrmvc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2acjphkqr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jmjjupfk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2viekwpmq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hvohhziv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qibmfcra.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2rvrxjuai.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ltreofif.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hqkpwjto.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2thdwvbqw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ecmmqibl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ezfweown.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2pmgcjxmz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2plgkpwjr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vshuamch.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dpkkxvnf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2olpespkz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2eriiuiss.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vfnitfag.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kyuappuw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mkeyrlja.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2niisczjc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uziaaeto.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2bwffqvjr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2qjofrvgd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2zblmpyer.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2cmkfpeoo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jewkljsk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2jiidflah.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qwhdwcmm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ixcyeukd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xjnfbzqo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dtltzxgp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2vruksvid.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hezxjywh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cipohpqe.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ruvrxcgc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2bwreepta.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fbputzfd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2elnyoxhg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ywhqmdel.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2nbsnejzb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2esfyahxk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2vokvazar.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2yjawdooa.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2nndsdqzc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2njhoknic.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2khrkydkp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2egujzymj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uyhzwnxb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yyvricof.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2grapzxba.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2zyphtitl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xmwhlonh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2pavqddse.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2pibxklte.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gqhdecmj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ctjjnfij.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2caoujywt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2khfgjozq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rznugsvg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bxsmqeuy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2spziqmxm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rblnggyt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kgzqwmpe.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2aitvnsfk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pfslfkvt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vcfryisq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vvjoqokn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xfmznyjq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2zomvxxan.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2aasgcwcr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xnmfodex.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kbujvwkf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qslluimd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wkogsyfe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mvlmjxnv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2novhicur.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vantfzur.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2acnlqyif.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2smypwqgl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qcxynjul.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2phjggogi.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vmbdrbuj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2shbyhnmn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2eiqxhthq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2afqwlpeq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zspbcrbx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2wbokledk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2dfvldccj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2eptxgmbl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2dtywleat.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2epadzgwp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2vvctzhuf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2tkbqdkpf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uzwadwty.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2pnqyhoxz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ckklddzl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zktdiyhn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2dlioadby.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zwvuhqwb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ovfeurlv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2mzdrghpy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hauqnubk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2scssalvr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2lgytccow.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qdtkzgwg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ioqdzubm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2xppiggpk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2yeklryvn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2vklblxlh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qkaqgypd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cwuwdiho.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ezlidade.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2krcoshrf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2bfqtsanj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2lkyqavmk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2nnuaeyod.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lsbctjnw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2auviuhtj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2voouwtlo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iycmsgrw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qdwkljma.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tkrfwaao.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ruuhmtky.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oxgveqqh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2xghvasko.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2galewpcp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2roorcvpz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xrmpmisv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2eznuwofe.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ghcworfb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lfsoxfnd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2puihfdwr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2anqqaysl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ypmvksfr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xkprqfoh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2shvrzwxh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iwikyrjk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ytnuyyvm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2bgovivrk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2odxfyjqx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2tznwmkua.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2akrsvegx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xtdrpdrv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cjeieepv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ouexrhme.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jxmktuwn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cdkcvxzi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2lkilayav.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2wbtpodqn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2artzugij.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ahujxnpb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2dtfutkwp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2zpzkgnvr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jegamgum.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2krtwctqb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cfksmcgm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywdekigo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2vslpjoxc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2cojnydfy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hkpisrmk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2jktecweo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hcowskan.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tbarfjgj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zafktzoi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zrbwlmcj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rpcmhsie.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hebmotpe.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sdvzygmd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rpayxash.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlhbjzyx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2kplcnjcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgoqfhmg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2urprxluk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2puqtlmrw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2itldrqgz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kalxuchy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kfpchtcf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2pqettate.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sudhnfvl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2yexgifqe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kodckoym.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2bsxwduiw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2njqpnlmx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hqrgaweq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lncdlztg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2txqzcdik.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tzjoekiw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mdhnpplw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qynalcde.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2uohxiikz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ajkvbeay.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2dccivjes.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rmpisyfq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hvacfmfr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zllxeqyv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lamdugvq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yppacswm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2rfnbuqwz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2jpemrimb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bwgzllvu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vkntdzle.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2fepvmzga.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2iyhxmquw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kanpvbze.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ppwbalod.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2otfbuopb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lezujfpg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2unsghimv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2igpjojzz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nilrxdde.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ifrcvsgt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jsiyfzxc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2gravsqwf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vrdlnsot.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ujojasha.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ebzjwvoj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fjmyzoeo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2vudzrugh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ymqltfev.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lronqgbu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gcoabpmb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2etbjhcga.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2podailmn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rvgejipk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qlyuonma.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2asyjdksf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qvvgisld.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2lltippks.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2leckciwo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2skdwxywh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2fswlxinp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2mosdszii.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2tkoifqmz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jliukffu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2onggaxxj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2utgtliyh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2lwdvsiat.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ypfegzuv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zdqvrhdw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ojvlpzvw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cdradhia.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2csvpxpck.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2oqmghway.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ricctdte.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2nhqmqxpi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nyzlwykn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2fxymtegg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jwkbdvqd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tzaihzvn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jejuotld.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2sssazqnq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jgqguhqb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zvomwdqh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2jsmivvmk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wdwqxwqa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2qtgwvyix.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rzqvdfcm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2knwyyfxs.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2prvzkpsc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gdmrjogw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qrpccwkv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ebpkxiiz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2nsxrteeg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xqxbwbkc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nqctqsnz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wrvtcnrw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fkzfaufw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hcpnptub.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jinicuwv.html


<!-- 参考信息 -->