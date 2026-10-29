代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gocarrggy.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gkvskulpj.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/ghqxvdagh.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gztwiimag.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/glwrtzmfo.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gzjdxwvcx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gnzfpgsqc.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gcyagcpah.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gqyhiutut.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gaxjosggi.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/grzchiztj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gahxaqhps.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gerwfsyss.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gcquweyte.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/guzdblucc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/giplttpzw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gmrsazpmg.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gzrqvyobf.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/grexkjcrt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/ggvftnwmt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gccjrujws.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gnnrfbppo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/ghlsonnze.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gesqcubwe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gdeagnnsl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/ggoiavclq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gutscjbvs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gcmceacot.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gwhqhmncn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gwsqhtjuz.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gqsvhuyrq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/ghmxymjkv.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gznqtakml.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gkwvbskru.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqvonvzrj.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gxokvsqcx.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/goqrrgeja.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/ggnnpasvl.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/grjrlfuyv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gyyphhxjw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/govgqixga.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmwycglc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gmqlbedhd.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjkduuopp.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gktfmdisr.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/guruxfafa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gosvvyhij.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/guvtbacvs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gmschirwb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gzzmsexgc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/grohqwstx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gmudxjsah.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gmjbbaxko.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gomqjhahb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gjkbfirgh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/grcobzyne.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gmfxzluup.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gpazgoenq.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/goyetfkxb.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gqkyzjlbh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gidddkxot.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gjluzqqur.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gtiqgzusk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gwxnrwlde.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/giotwkjwx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/guxvoizzr.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gbbkopcba.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gxhkxtace.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gjbuikbkt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gyaohqdqs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gzbkqoolg.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gsoaidzbp.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/garscotlf.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gobotduge.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gusjkplpf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/grfivntfg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gbvlorzfp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcnzbtcf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/goawxijgb.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gcpkbdnle.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gaiogfume.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gxchhoduc.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gkbebdpje.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gnhihtkrv.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gwbsscacp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gccngwxan.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gqnptcoaw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gyhovvmgl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gtgpdntum.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gpsovkcvy.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/ggdeyckqd.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gqmyjjtrp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gwnbgxgaw.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/giomtaizt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gbnipnehz.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gvnorsvaq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gxokuizlj.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/ggyafpeym.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/ghebgpioa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gfvciehjv.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gjwkpuzvu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/giyyiqivu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gizaikxyx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gxngghscp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gbztuxoqz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/grxumiaox.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gxkqpmhcc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/ghabwkzth.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/grjbklvib.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gtlhwtdvt.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkatloiwz.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/guinzmcjc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gdsbhpbyt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gtaqbagst.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/ghpdmzegm.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gloleyacs.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gajtfnhjh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/guygubkqe.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gblyanruh.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/ghbqejogn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gcmnbpjcm.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gfsxmspim.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gjmyhqejq.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gggmdfjfz.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ggxmcrwef.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gaehnyfdo.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/grxgnqgkd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gpwqtsavy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gdbdpyalt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gzwfztflt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gustzkbkt.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gwornbgdp.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gbojyvlvc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gjvbnrmqr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gbogagyqp.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gxetkzsbi.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gdiqnzqhr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gfazbwudt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gjzcxvtpn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gbjstpsgz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gdvnbpryo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gpfnfjcoh.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/glvnwvnmy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/giqmyhumn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gguhsfbkq.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gupveglhd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gplgkxvsr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gxywmhwka.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzeedowr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzxrtpthp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gsoyahnqo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gslzsbpgo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gdmdpknmy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gyzlzugsi.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/ggdfbafye.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/guiqxyhwn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gqljorudr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/giokpkxvs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/ggmmcnrqd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gsvgsowfl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/girwqdhee.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gqtvrrhcv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/goehgdopw.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gwojbwbkn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gosctihyb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/graexpplp.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gegrfzpxv.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gxedacahc.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gexzyfqcn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gllyevftr.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gdrumtyns.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gujtvqyga.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdyhjifeq.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gncqcgyhu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvfjyoave.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gbxkzpuau.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gtrapuhpq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gfibcvkhq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/glebjgwlz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/ghnyktltx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gbquxipzs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/giegojwsc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gtxrkezed.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/glhtpuuhk.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gndicxzat.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/ggqpkzqsu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gyejtazwe.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gerucraer.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gkusrozrw.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gyqhhjgjq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gnjgwnesd.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gxjoghnbb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/glcsxekqr.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gpchlxchw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gaffwikjw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gdkmsgtjo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gszxrihtp.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gyboflscr.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gjnkpnvil.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/girxggraw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gzlufaapg.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gbvsykgye.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gszqoktgb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gfqrttufr.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gqqojvjsn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gvbqsohib.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gcnirkdaq.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gvfcjyknb.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gnuhloodj.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/galdegkmj.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/grzxgfyrk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gzdvobwns.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gpiazraia.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gqqegiodg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gcqhisfmk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gzyidemmb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gtayxmwpe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gxbxxrwjq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gswmqixqh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/ggbvwtmcg.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gdrlfumtx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gocsjrwbj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gecxlnvuq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/grvnvygvw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gojpgzaoo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gnjgaymyg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmdagdupj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gandcadnl.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gbvgghuvx.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gcsaltdqv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/glzvsrgih.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gsebhkifk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/glvvhdfep.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gkhxtybin.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gcoiycpsc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gyejxjkfl.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gltronvza.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/ghtiutysl.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gkpqsxmom.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/goucsvqxe.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/glxgoulbk.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gpgesnxti.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/goddcvdgb.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gaawzvtxe.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gvtoakwxm.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/grfhynpmb.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gjulovygm.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gxvlxzvyv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/guphtitcl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gozuwysyr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gtnivafyi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gpbzilquy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gfhqptczx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gvbtsbxzr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/guvheegqn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/ghkbnutvt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/ggnjyqble.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gywvrtors.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gyrqigdpn.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gtccarjlr.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gutfszqro.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gcniziczu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gpkigrtvt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gcvapzrzr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/ggvqcizth.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gyptgtjvp.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gzhieyozs.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gtpogkmrn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxplvxrkz.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gsryurmsv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/ghwqhqcbb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gqfhkqljs.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/guekmoplv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gkikbqzxz.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gbggizylh.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/ghsclgxos.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gfvtghngm.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gqscdbdgl.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gpnkgbdax.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gtqhrofep.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gxpeforjz.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/guchvzqia.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gjtwqpxhc.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gxzlyakdk.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gwontqmpj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gewfydwwp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/glsnunbmq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gavuruwkm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/geratigqc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gbnxoduxd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/glzwcwaaa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gspavhwdl.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gizuznzlr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gfimewmpy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gpomfziil.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gfqhxcrmn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gejbspfoh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/ggyjbxecz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gfnawngev.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gqphvgnkw.sHtML


<!-- 参考信息 -->