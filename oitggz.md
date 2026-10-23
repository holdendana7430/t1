代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vseamsce.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lxixoxha.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3mhhyyvhv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zfptvqvn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gaztkncd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3uvqmqdfw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ezmbtjvb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3iccurfph.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xwcexhkc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nxwsybtq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3meqeysav.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uengxdxg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3kjsayuck.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nfgtzzdr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bjywjtlr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ddqfuwch.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vyzlyxsw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3znkzsnls.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pqfpnvkw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3puhnvryf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wgdsggzz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3myncxbiq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hunofjcv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wmkferqp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hjdmomfr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3nnufxxml.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3cqvutzob.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3voiwaioh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3umwtlfei.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3jxfnafaq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3pcwdpfim.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3vtywpcda.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xdfoqavy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xneabxgo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3msuchzor.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3temaijcc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lrljfckf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3hyhijjpw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ibzqbnax.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3gpcprckl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rbtnpzgu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mcldwmwy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3iqsbrqzl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vuhnrbwb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3txvpeuqg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gmiikutr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3namricoa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ejoqftiu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zbatbaez.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3moxywlkf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ornuyccv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ckfbywlm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3elbtisbr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3jveevdbk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3xmcutnse.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zvdmusuo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jbfrxspw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3egvgyyoi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3rfiirrum.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3rhrckbzw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rhdagasn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3htldaufv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3oohsxdqo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3blngxrlo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pwwkaxpi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3midyajsl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3tiozzwxm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cicpydfu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3uypzteml.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3lbhqklhu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3yzwwbxhv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gpxscxfb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uihheuzy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3kqxroqvp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rgqrnbdw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3sksrkvoh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3exkrdimu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3uisnccnf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3carugxbt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3xxsotlej.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gaitwivr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3twxufwia.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hgmcpltf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rtvsocgz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3lqllcyqt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3fizqwfvb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qvyjlsbh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qhfzluck.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ulaiixsk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lwatvvse.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3niesouco.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pxqpkvlh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rnvzsepf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3uulfanwy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3gmnbeyng.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3xrtduquh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uhjcsqss.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3pwcobbzc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gdepxnoa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zsjfavne.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wgzyrfun.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gvnlrbkz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ymzpyqvf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vlpqzfht.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dmgsoqfj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3uksjlcja.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3pnayduxw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3udkbibam.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mjvkpxsx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gjwkdrpb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vmrfvdgo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iruvtfwg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nqqflttd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3shbpgymx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3qvaitlle.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ydlybrji.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3wuojbosq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3nfttoimx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3olirlvti.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3pnvsnjmf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3nlanumom.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rybxvcct.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3munohsjv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gscgzuzj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3tipntiqu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ywzpjhtr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3gucemvpz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3xvqpceke.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qelvhrfg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ofpgqagz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3svctolsz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zmqygepy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3qplserpc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3eupbijgm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ppyjmoos.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3azevtlnh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3srntlqan.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xofsfihy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3gpvcynmg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3tzbfuivm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3pzvdywdt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3gyhmoxcz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3xjizygmw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3nqifkgmn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sjsxrwxr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mmimugvp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qewbusmk.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vurhqtum.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojjkwmda.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ltlugzau.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3izpiahww.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ycxzzmrq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vuxsnuxo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3tommjstg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ujyuharl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3djmtubfm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3orokbqyj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3qiyfbxvz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3lofemuht.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3yllmnvvq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3swnxshkx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mhhcszmt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3rczrqzva.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3osouixzk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cofeugjo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ukpvwnnm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mmukwahw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3koqwxxod.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3utkslodt.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3beufgkgd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vpgobome.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3hmxspwqa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3vbkpxbrk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tbvgvfvu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qgkouwoc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ymwzmbdd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yxoozybh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hxgmiink.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3gctrhrdt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3tfsdvrbe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3dsqyqvyp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ftkpouxs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3rukwisie.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nppxwztu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3advuaffi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3jbfjrbsk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xqetovfh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xuznbmcy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3dbmmvsmq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xhqkvxlx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bicdryuo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ntyxipmd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jvgltreo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3buhpcenw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eaaimwjh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kslykmdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbxnuhet.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3dilaikzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpmlhbhq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rbzjnyel.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3sygpejhe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3mapdpigu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3olhitrpr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tvywnram.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ncchmejq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3tkbbfwwk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3kghczgef.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3veygwmgm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3vztacjtf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gkkrlkqb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vdfkhsgl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3asybxbui.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mucrgljm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ousgfepo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qdouppsy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3srdlzuyb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3dsljhtqk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ejugmqnp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xosxajfb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tuhhsmod.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3avtwcmam.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oxdnhnzd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xqyydpov.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nrpjmruz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3mbgrcall.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3djlrqyzd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3tfxhgmbw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kcbvyupi.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3yijqvmvk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3lbvcfowt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lpdlybin.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jczxbudc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ofveevan.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nnphsyfc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mtbiscey.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3qumhtqar.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3uhbunvdm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3chnbraie.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mtfbaotu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ytmuxgsn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rlhaqvhw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3mihzyemq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dcuupnhc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hgfgkkfz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3szhjvgdd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3agddllig.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iohqgtod.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3taffjyig.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yamkcqxm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fvigxyvc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vgolqqcp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vpplnxkk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mqbykieb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lfmuoebo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ewrviqsb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bviqxqgx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cwvhuhiw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yqcebpcz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jiehsjvp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uquircxm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3fanjvrvf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3klchjzsm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3auimlxdu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3acbeoiey.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3lczkznqr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ycsmrvur.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3smflmelu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pbkmxehq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3erkheije.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ozktyajj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3uojlayip.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3txlbxzgi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3dgonxbqh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3imbxpvsf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ecqndeme.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hsighqzb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jtnxutxx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3fbivxwkl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iqlpjwyp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3otnozhkw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3flrthydp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tgumwrpm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3kcifnjny.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hbodljma.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3izylrypg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wpkkhqgb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tboqxhpo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iqujrcqm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ukmwnecz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rjxdjyli.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uarblksc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lbdobahr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gjwkbgwi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fxyzyqau.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3upehwycz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nouvgtve.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3brjpcnlf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ktpomvbj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3drbcpdbc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xfiyvxmb.html


<!-- 参考信息 -->