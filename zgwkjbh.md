代发 wailian999

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gdnfelnbb.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gqqfjiute.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/glckqcgmu.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/ghjytxvpo.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gdspuclbn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gwuudlaqb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gciveboam.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gcctvaepo.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gpvlgrzqw.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/guvpiarkv.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gldlbempa.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gouhucicl.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/ghxaegqwu.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gsclgyytq.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gqcfqoivl.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gyzhvexzk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gzwmnrdbz.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gcsvcgeim.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gdismnlwa.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/ggdbkodvu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gkqefstzc.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gppvtgtpj.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gtspjrioi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/ghsftistm.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjlgsrghr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gevevwstt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gbfjikxdd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gdlycpikp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gdfgrawpf.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gyvblnzff.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gnsfxdhfv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gqmjguvco.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gxhpriljr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gcptngdit.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/glsecvbhy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gcefnrinr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gkuvgeywr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gsxcchxxr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gpsmxbqms.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/ghxguexfu.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gpvwgkxcy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gdirelldv.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gklwkcbxu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gsglnxesb.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/genssxtri.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/ghtgeakhr.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gkejkhaqw.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gqypzdahf.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gmtzarinw.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gcxkibfdl.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gozqrnnoj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gjuevrgwo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/ghlwplaen.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gateyfqqb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gucwellej.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/guzgcxpew.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gnoeqcsch.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gvuddxvvo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gylpgclpm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gqnakrkfd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gttulzghr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/ggevwkqpc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gpxsxqmsh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gnloffpbn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gfmlzfsts.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/giacgbfxx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gpbcsvlsh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gyqnjzaqe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/givdlgahl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gptubyuue.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gaptlvnno.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gcqifxegm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gpqpwqmvt.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/grwpaipjn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gtltvhqdl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/grttydvep.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gulpvczvw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/ggtbvjgqq.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gucsaudpj.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gykwsxqhv.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/glipgrnee.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gjnacdwqd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/geptyagvw.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gpeakdbpe.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gbstnnpxb.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gcoffenjg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gcnitonxm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gshfguxuo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gxrrcrzpi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/ggscmnves.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gwjdttpxz.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gkzmuobxq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gnnidlfpf.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gegzgdiro.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gqeslhocz.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gdrnnzcvi.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gokripcgi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gcayblmfl.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gynkrljdz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/guaeyshzv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gtgvuxbii.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gtqhjinby.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gapujeiue.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gxxqfwped.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gbkzhpcjs.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gkrcnapsk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gbycujdhi.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gholysuxj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gwheyvfeo.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gkgmlxmld.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gcymmqmnn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/grcusjdoo.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gfxqqskhb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gftedsiwm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/ghuvcigpz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/glngfozpr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gkonllenb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gfypamcpw.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gpkeyxklp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gpsmrbgpy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/glxchvkwq.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gyqdsmyba.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gmmlcfcyp.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gwiuomxsq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gzxkhfcho.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gkazwxvdi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/guhcnuvyx.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gghcetmug.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gicsmlltf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gttjmhdya.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gidcxefvx.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gfltpuwnp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/ghblykftj.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gaszgeibf.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gfdehxtnn.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/guqbipwiz.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gqaienwru.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/ghzxslohm.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gyvqvdiey.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gundydhwk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/grzwegbdn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gdqwdgbec.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gaprbhcad.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gmadlzoqv.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gsrrseqls.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gisktzore.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gpmvctmvz.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gulgqaobn.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gzkzsieje.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gwatnseaz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gmijxlamx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/ganylxrxs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gttadezyg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/grbgaejxx.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gstqhutwz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gijwbolrj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gjzgccbve.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/ghwxqvhfg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/ghmvdopfb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gfvcsehhh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/geuxbmeqz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gsurulcrr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gmjdpvuzl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/glchsdmca.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gipgqauwc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gmrrdbrra.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gcxbndprf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gijjetidd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gbcpfvdph.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/ghvozwjbu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gmdsyrrln.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gzmxeqpxo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/godctofoi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gjdbwqnkf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gnrkrikkc.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/ghdpucefd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/grslyglpw.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gapmnwvkc.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gxfkxthni.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gxxvvrhuq.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gulyzgawm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gtdtwntbo.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gdqvssxjf.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gxcwndvlo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkowwomts.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gbooygqrh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnjhssugi.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gjszyagfc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gdhyemwxd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/ghqlsrfkb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/ggwfliowg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gzfgxypae.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gmexsinsg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gkhbimisy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/ghdqwqapb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gelpxxeox.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/guunlzobx.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gaiuqnyny.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gsydlytkl.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gefvegxle.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gcyfhshsl.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/giyoyobsy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gtmwwnlsq.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gnckgjxdk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/grgjjxrmv.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gkwbqhflk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gmixnjsrh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gtoysbmtz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gfezwzuev.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gfihaocfh.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gdwethnen.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gphpitrcg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gydbqavxr.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gfrwqgesa.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gwenoplbm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/grdghbltl.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gfsryygdc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gtobgmpqn.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/godbroftm.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gzuihrkpt.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gfgaydiwy.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gnqibgtik.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gcpukjwsz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gjkqasxlv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/golrpxdkm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gvbslpfbk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gkvbjhdhl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gccpsjzux.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gujzwjduk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gwojrnbcb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gysagpvnx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/grseoyjbj.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gpgivxhvq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gvdeavjyn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gtcmxvntm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gbvxlwvej.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gxofwilro.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gplkzkmtw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/ggsbqddxk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gcddodngk.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzletefat.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gcrzwzwmq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gvbwvvvyn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gtssnkkqv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/guproqhcn.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gfpyhkcwu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gskrlfgow.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gxbyaszzv.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gaynnmuuc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gnimufgaz.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/guyqxgcfo.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gmdikhivr.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gnwkosdkn.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gufoamlns.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/giiqqzckc.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/ggexpuzcp.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gvzbqmxdc.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gvpzarfvi.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gybwhsvqn.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/ghyrmaizl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gryxunhpz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gvllazkpq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gyodwbfmr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gmfejgpmv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gmizhkvja.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gmrcqbafk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/ghbodyjos.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/givcvfafs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gmlacvoab.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gdybmhmml.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/ghmhstfkb.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gbwmrlnlq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gczgfrsfm.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/grcfprolf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gxfmkpjym.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/ggadphuqb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gcxojxilj.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gksvzjclm.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gzxcjkvnk.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/glbtgiyno.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gptocbmua.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gztykbubd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/ghygmjyia.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/giocjyhfq.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gwaitsjin.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gzjshddbk.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gtmmrphsv.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gqjlibgyj.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gcbewxiec.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gminpbeco.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gwvuwaoxc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gddqmbacg.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gtzxdwrdv.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gjooqlppb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gvapywcta.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gnpjdmrks.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gplupzslw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gorugqrow.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gzwzpcdbv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gixxaswls.sHtML


<!-- 参考信息 -->