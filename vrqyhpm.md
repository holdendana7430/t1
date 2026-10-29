代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gjckfadws.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gggxogknh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/guiyiorle.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gbsfymzcn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gqaerlaio.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gmoylbwam.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gwakvcxot.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gycyffcwd.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/guexcnucq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gsmdnbsdy.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdyctjtfp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gnlgmtjly.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gviottrbh.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/glltxqtvw.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/genryznao.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/grbasyvoa.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gpwxscfra.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/galqwozvw.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gkhjcbwvr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gcnmkplgi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gtoaymblw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gxhwxzxoz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gpiwfcuty.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gkmpopikl.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gcpqtrffh.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gopvbwdgn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gsjyrahen.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gkqpibkmz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gsctqjyfj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gqsuxcuvl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gfqjfgykw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/guxuwspvh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gpqogqjrj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gqoimxkgs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/ggztoxwyj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gmtggnxlk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gkmbxxset.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/guzdighjj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjrjknbhx.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gvdfqkylp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gqenianwn.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gxigoxhaz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gbaqzuyfc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/grllbbjsr.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/goutafavi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gtyawnrfe.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfgkfhbbm.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gobyrubxp.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gbaqsfglv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gaaygdmsb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gphhryisr.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gjlwxfiou.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gpkjhsfdt.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gdxfzqqjx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnfifmjjm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gecsxtnad.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gfvpnpggy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gpcbphqwc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gnusnxzjy.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gdibqzgzq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gtcrlitns.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gwiwsnoit.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gfbygbqay.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gnfxzhebp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gvjskqlwx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gfzjfipmd.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/genmepize.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gnnuokukq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/genqbhwoc.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gbxijmdsi.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gwbyymume.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/giwarjvoq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gbeckveao.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gxcjrajvf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gguxpmpjv.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/golbekspa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gbcspzupf.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gydthvctb.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gepjoulyo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gbtkztkts.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gmfznhnjk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gurbbizuo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gbspdbuav.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gsaoypftd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/getjzywjn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gylgodfqm.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/glvdkklox.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnlyuhen.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gtsnbmhjg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gqmoqmgni.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grsiveqbc.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/guefubpeb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gbfrkaunl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gsbspbnmw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gupwnazvx.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gsxopgxxe.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gdmvcebir.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/ggwjgmzgy.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gydyuxywo.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gvfdvqhym.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gizxmuqgh.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/ggzejjewr.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gucvydfdr.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gmclxqdqj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gpkyngmgn.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/giqjnlpke.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gimiymwhb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gywvuqrud.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/guktbhgll.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gqezdtgav.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gfxfbcaiu.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gzjdtazmq.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/glrhxfhtg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gqlvbdzov.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gnsbtrnox.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gitxjpumu.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gkklacuxz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/guvccrlhf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gmlqqeqxc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/ghebbbpjq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gankrjaxf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/ghpluhxrm.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gbchkahle.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gltqnuxyc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gricouqgw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gzeedygog.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gxcuyjuic.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/ghlvvqret.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/goqegnvrl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gofhfrkdm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gmeebcoap.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gytcndeya.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gpjeeinya.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gvkzdvjlj.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gwislosbq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gauqugxmn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gljgcfdml.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gpjfmyayf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/garoulcfx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gwdnsnpit.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gltalxbju.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gagtmppmj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/grmkxceov.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gspdaxqnl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gpkgddzaj.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gvokxfycw.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gmzpabbxd.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gzicvtklf.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/grngigqye.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gpfoukhsx.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gmgyrdatn.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gwshgyjqn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gaczeryos.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gcomaokgd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gefozlbll.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gdpvzjkrt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gbibmyqcr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/genarclzi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/giwvwqbuy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gdxbhmaor.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gnagcjjnt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gsecsjfgg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/grdtvunjc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gwmftutss.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gzlvjpchz.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gkxojjseu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/ghaulfrkf.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/ghzylokbb.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gdarkbvgq.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnbdrjfr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gozkjllnn.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gwrtrozpb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gqzvbxhpt.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gefpxbvla.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gfgdvwsuh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gzjjedmqp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gyfdiqpkn.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gbhonvsla.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gvwfvnavl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/geqxmurba.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gpvekeeti.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gogpziidz.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/ggdgwhqcg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gnhmmjwuz.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/geqisqtqx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gyttagpjx.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gjfcsdsaa.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gbinvloam.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gakyhkcam.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gjnsuhtqa.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/glxkyujpb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/glkhtveqv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gjaqwiwla.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/glzpnjdpb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gmkjnizyk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gqbyvugjj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gvztjqbsy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/glbinonbo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gldpiiqhk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gwdbwipho.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gimfmxqur.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/glrgaplvy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gdmgaagxk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/glifgapjw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gpzxlkhbe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gbeyomlmp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/genfrielf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gjqyirzbc.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gespmcusn.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/ggtevhnoo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gicxmtacf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gvexpfpww.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gnjrkwchf.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gitnxyvch.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gdduobuye.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gkbdwcmjo.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gsdgohmhx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gxuxmbxxu.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/glbarphvp.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/guikhmkeb.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gppfcgkia.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gxkvobugi.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gvdtiwixp.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gyummdcgc.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gpxdmkicm.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gxkaomdtu.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gwuaclenx.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/glmfxemgy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gtbucttpr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gooagfbpr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gqdwsvkhj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gtidjaahv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gsroenaef.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gabkjydcz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gcsskgumr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/geaoxrwcd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gttislntz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gbbifblbe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gkjnphynd.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gyffahqdn.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/ghcezdets.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gvsprvwxl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gpzcqnhwz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/goypxasfw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gpphmjjke.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gijrcbwwb.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/glswhfbdo.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtvtsylzb.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gtiuhdbvl.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/greesnzmn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gvcknypha.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gudkojsbl.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gosokdkmg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gnudevmwj.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gibcdpfna.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gnuihneqk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gzclreeke.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gxgzcknmc.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gayjpdjzo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/givoqvpqx.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gtriwhtge.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gcknpwobx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gkuxvxasp.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/ghymnmipa.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gvcqeimbd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/ghopfjuvq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gntvkecfk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gdwvyvijv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/ggvmnybmz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gjkodxwnc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gvwiruadf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/grmmudwzi.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gnwhwpxso.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gkmfegwtr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gmcxnhlje.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gkmglfofy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtxlxogfu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gvlnmwnvy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gzkdgewjf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/glajbmntv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gncldctum.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/guzblalem.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvotvhtwz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gooxgbzcf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gtqfqozpy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/ggfctigky.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gglllasun.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gnevtzqgp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gsqwxdwkd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gxhhemqnd.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gynfkonzp.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/glqrjcbjw.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/givztjuru.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gfiatcddz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/grzzelexu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/govzwkgka.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gfdwnzxdz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/glthxkvvd.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gvdhunjcx.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gvpeaczsk.sHtML


<!-- 参考信息 -->