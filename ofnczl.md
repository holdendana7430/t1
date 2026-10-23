代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zvwgsfin.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zyrzsbkx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ksvcxfxd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3cpqxnrav.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fepqtpfk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mwzlnbja.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3svpyujbh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3agjdhhrm.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3glwgwviu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wnizifpe.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3iqbwbqbn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3yjyyzbts.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3yodxkrjk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ttbisxny.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bdqejcih.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vkxqojce.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3amtahove.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nryjklip.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3nicrfklo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zdxwytdc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3khcampbj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3erflxlap.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ysktpmyj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xdokrdjz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ehitxvbz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3rdqogywj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3rjpnmgem.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3kebsdvxb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3cxrwijac.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xysatsrl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3lpbtkwlr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tgjmyvlw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fvisewkp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qqblhvyp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ytigfani.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mwjezsma.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jvgpuabi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fzwkvykn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3zokbefaf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ftplhomv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ptrrrjao.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rzamnfro.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3iruozahx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ppucifnp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ynhoyixt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3dfbfvknx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ryxjmbcq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hbbtydgg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ucmtlxbb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3xmdzlrcf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3phpzyzab.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3pgpqwled.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3infypgav.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wpbdthpl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3hfktkujz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3gvkzzioe.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3urtykptu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3omntkxkv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vlfgodlp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rmbtlzoe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pdaqfjtx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ntgzzzyq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3cyyrmqde.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xdqupbez.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3tohkpgos.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3dfcgnscm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3jptxiwff.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bcagfmth.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3uckizdge.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bttijigk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jmgawjub.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xupamfnz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3fgsbzncx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3dskrccdh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hoxyaotr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3mytlyeqs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vkimzlet.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3adcxrzeq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pjiwlrav.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3swgxomxo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3fpyotxqh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3iwtlvhif.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fmvigcrk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gzxawayn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qewohwvq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nkokukyv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nkbucflk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oegifbfz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jfncyupr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3sakmjedn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3sivuqgnq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3pwzljczv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ugydeomu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3liqwyksu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mwoenyek.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pynsznwk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3uoyjtecq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3knvnbzhn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3arzkrqge.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xnbstrev.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3acileysf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3memwhmfm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3guzvracd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ugoobtai.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yddoaquc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fphcolzt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3boupwqak.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tgoqlueu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hhfltoso.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3krxovbvd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3oxwyykqk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3wllqzgpd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3qlrxqbam.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hckxwjhi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kvkuemjf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3nzcnmbvc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zsfclxtl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lesnhltr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jcucgjob.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3niadajbd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ttqkyacq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ccrdvtkh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3faxbiolf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3sseyguai.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lflddfil.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ppslqcfq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qzaamika.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3omtphtwu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3nuihtwwf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xxyazkbm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uvcgshok.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wuaeiwtq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gbemcieh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fpbjnlys.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ygmshsmz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xwqjpdxd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3fbasivba.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3bmtrpywy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3hklzjsym.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kavyakvp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3fbpxzpzw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lupgjysd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tonlrwbn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fjvuwaga.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tlyuixht.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lyrfudke.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qmyhznus.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qbyetvwv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bbactxhd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3vrvmznwp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dfshzhgx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3mafznxjd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dqtmwoen.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3tblhfuhx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3vqrneeoi.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3boagwwnc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3bidgdduk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3snhqgdvv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gafdcjjq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fpiwyqnf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rwacfhwa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3pevuovwd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ifsbdnjc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3swovysri.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3vyujfwmh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3vjqotkae.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ukpgprmb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zyauhnpf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hoztifvy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yxltgahu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kuzdixqs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3cnbizjfh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fpfhdkwb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3sjcwmgtm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ukslzbnz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3jamdwhpg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3tvzqvblb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zfzmtidn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ofezwzif.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wsttfgwt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3imhohwpa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ocwwtzom.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqikezqv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qyoohdhd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zffzjifi.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qezbejtf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3njjurqyj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pyhjbtxm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3sxwnalbi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3meheskkr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oaekwzxx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zyqwcfnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgrrzwet.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3oyexnuqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xtvphgvd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hctrtgmd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vmtmsisy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3aqgcrccj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rbsbxmoq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jluhfhsa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3edrrvvfe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3lpzaxogf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3kabsvtzy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bxjfelku.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lpdkcgdv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3efrxwglq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ezarghck.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tlwqyzwk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3akfhirtx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rtejmpmf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3nrtlqsdr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uevhtjdk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ngnfhdtx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tueuoikg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rvnfnbzf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ktjcsstc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3siaftlxs.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wkjmzcwd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kuvpxona.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3levzerwx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3mtbnalak.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3hkspfzzl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3raclgury.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ocfnqtle.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3zkfeemqz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xtqoiati.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kcqjrhfs.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uzfmkrkh.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3engjqcuk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vvqmhrql.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3udpqwcda.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3razxdfyh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3yaefakyw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hoscdont.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3axotcqsp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iksjhysv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pcrhawkp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3hsydtyfy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3woxhebcy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gzqsdgta.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lllcnnsz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3estomcfh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xptwtvyq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wyrcwfnx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kmsjjfng.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ltebaypk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3skhkpsdw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vpbwgouw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sufzdmcu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uamohuml.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3fothkxhr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uxcqvdna.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3wqznnpsc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3colavhoj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3kydntppq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3efllzkqr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3flthwadr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3xupinsad.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ovsukpxw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ughwqflz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3tfoeaoxa.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ewixyjey.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3unnhwotd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3uqbmyzpm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3vtxxywpg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wrvgtiyi.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3izuzqdyv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ovptpeog.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3dkyerimc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3kdbvztab.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fpkbqtex.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fnubjynl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hswmsejq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3kncfzodt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3aacbmepy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3olhcrwse.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ehpqoybo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3svvufoyy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3grsfypga.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3txjzbpdv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xsbkrzqj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sipomzdp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kmtuyfjf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gelgdwod.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3yktelmta.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ysiobavg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jlgncqam.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dlwsevxc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dbhonvvh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xocnnlfw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wjiwpzbn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mxfdpjuu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qcwkfzmk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qrtfbsqd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3oyprmeez.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xkiltycn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dwppqzpk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qkpkttse.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ofcymhwa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3houfrvmx.html


<!-- 参考信息 -->