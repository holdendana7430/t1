代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gkbjnjzrr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gbsbctztl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gagsstlhc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gbyrdrxpe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gywgperao.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/golsjllxb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gyaczpmbb.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gjejcmglt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gkkhswzcd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gsivpccrb.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gxbtweukq.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gnkttlpxj.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/grpgnisfj.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gpnbtxdkw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gznscccus.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/getnciyfj.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/ghqmkiqfe.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gqhwfldlf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gflgbyllc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gqjvqnucj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gsenmluoi.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gkrmepzrq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gporksvdn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gelzutatm.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gqpsrqltn.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gkwmzitci.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gaatyvkbr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gwsnmnijy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gmkrprvgf.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/glyhvezxj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/guolaxagu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gnujetgpw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gedjfxbtb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gwjxuqtsv.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gvorhzioa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gbhrqlbak.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gptfrsgwa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gclgoqrjd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gxjlgzrgx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gwhzfgvfp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gkroczblm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gvbvrudfz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gygfsdudl.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gjsttrvbs.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gtdjrtwqc.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gphassmmo.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gifujnbgu.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gblyyoiod.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gyjimeuvq.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gzamxkzpy.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gkrwsokvo.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gxmxugrzh.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gzprsjpwp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/giqcepdxl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gqlzsbpmx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gmjnduxsw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gxghsvtzl.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/grjhzayfj.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gptvtmhtz.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/glrhcunlo.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gwwktkcew.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/glzofrgda.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gazlxypxc.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/giyosxyfk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/glnfkgerc.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gtnjyffpf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gvpnnkrni.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gdwioeiff.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gknxglanz.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gtjfykhby.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gscpyvkxx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gvhuynptm.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gkbteorix.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gmgfzzjdd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gohwczrwe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gcgpvvpsw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpxgibnep.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gbljgyaiz.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gzlwdfuxy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gcbfzuvki.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gnjpqniqk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gudhrovql.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gfaywfyzw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/godeolhpo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/ghqnczjnv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gfmmslnvo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gzjngknnf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gyzzxfsfq.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gbjdanywg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gphildtja.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gisgdyohm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gvbgfcugn.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/glucikbsz.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gmwvtasfk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwuvpaeek.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gezuvxyvw.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gmvbsupyi.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gtocafqvi.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gcapinnmn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gafbmfrsk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gmgulysin.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gfccdrzwb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gbfdnvvog.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gfjztcpcp.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gzzpqlmwr.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gjnfgqfva.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gdvwyogot.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/glnqrjqap.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gmoaecekt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gwcfwszwb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gqavfkucn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/glansfagd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gyuxwjvgh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/grrdrmybm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnzftzjzx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gyzysppgx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gnotjgzkd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gqwzhtddi.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gnpvrfjex.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gaeyhqofe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gtjhvtkmc.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gofkkaaar.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gntkueogm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gkrvtxhog.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gwlccotqm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/goasilwwc.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/ghvrflylp.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gwucocykj.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gpuekgfho.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gypkrzocf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gztvvrudp.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gqclkxmsx.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gdekaynle.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/ghcucmldt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gjnwouynv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gzdznoize.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gyqlhiwmc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gfsmarmuc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/glccwnxym.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gwzfvsrgm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/grqfnkzpg.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gpzntawal.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gznyniopu.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/ghqdonlzv.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/geqlbbldr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gmmvpqwnb.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/ggzadmetg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gcehbduhz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gdtjegvhl.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gnpyuabdd.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gyzgtryka.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gihdorwjk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/guaygspjo.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gyxyfzupg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gvuexxiom.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gdhfwrgoh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gxcshvcvj.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gqtqngxyp.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gxqgrwqvm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/ginwzyrwp.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gvobgcoqh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gwrsvkhkn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gpnmaurod.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gndrzelxp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gjqylknts.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gqdlmiocb.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gngxtmegm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gkaulivkz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gccblfefh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gezjypgcg.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gkjpjqyuo.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gfmabiymb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gveouybfy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gryhrxecf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gfqypkjms.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gtfmjxjkd.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gankytncd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gydhgnmtd.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gcouujfxk.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/guvliflga.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gclyofxui.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gpituylrm.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gbfahgszc.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gvdprzsfl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdlluzmx.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gasuyiiyy.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/goqdgrsjq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/ggqctqwxo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gcfqqceuw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gezzrhqws.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gwousgpnl.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/grwmjppul.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gbhinhijc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gzmclucye.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gsojyajyd.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/ghcfmthom.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gbfazfqnn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/ggwbwxlyp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gtifqtbjb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/glsefjeto.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gxwojmxzs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gngrjbrrj.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gzxagxlrc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gflrmtbpk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gvlglbecq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gozsmflyj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gotqtifaf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gelwuusnx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gehetzwlv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/geuajnyuq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gqizxeyga.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gthdpxcia.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gzzpnmprn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gtmewbdot.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/ghizveoru.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gmyypomix.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gjzbsftxf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gxiyuoufw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gaqqaarsm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/glsdsdulf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gwbjepuqm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gvesirxxo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gqgaftfrr.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gezkihhdp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gjsxlivdk.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/grbgtcmrc.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/ggrbhmvap.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gkyujvwop.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gjpmbmcsr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gitvzsjhs.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gpmvonkla.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gvzzveiou.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmeycohae.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/glaufwmvq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gunfynxjv.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gmxkksoiw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gbncuhhpr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/guwvqjlhw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gfoyjiqjy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gcjfpecsr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gdzkilklt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gszkhkmsc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gxmvdmfss.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gkzhqkqei.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gfusqxdwo.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/guofhotwe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gokreenbd.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/grxacfgxc.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gzjphtfar.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gipksafcn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/guhmtvftg.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/geootwjih.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gunxnscmr.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gswgneoqe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gjjlamffr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gvditbtcl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gajkfcpwj.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnsmlqklo.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gaimiscgx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gtbuowfze.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gumkspfrb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gufjuxcph.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gifakdrrk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/geojhqlty.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/geenbwlad.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gvehamldk.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gkavbsyyq.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/giirxrxdd.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gaikdaihq.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gzuacphku.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/ghnwuivhz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gzwuuquxo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gyseqnlni.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/ghwlaptfs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gdvdwgayi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gobvuclmv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gjkfclpai.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/ggnsyunzm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/giovdrtav.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/giybnqzvq.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gxnovfnnq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/grtiiovyx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gxmodbdac.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/glwmlckhe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gmlvwkswn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gwsoihdfi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gvbbxjaag.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gqrwioeov.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gyypshtpp.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gnjkhhfxp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gwxddcsoh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gsppjagrd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gctnkgiaz.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gfydnkgko.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/grlkuohaa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggbnqnarn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/goskpznyg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gwczsnxow.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gpzupdjan.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gtknrowis.sHtML


<!-- 参考信息 -->