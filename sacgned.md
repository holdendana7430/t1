代发 wailian999

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gjappluqv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gvqvleyux.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gwfluvctv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/guyzfngkc.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/govwrncoh.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gdolnsvio.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gsclnuwiy.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/glfxaxizq.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gyazokdqf.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gasrnxive.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/govxazrvb.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gytmexpvv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gbrrdsqwq.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gmviwhsdh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gobnynbtw.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gfcrfvvqx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/ggebmtzft.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gwlyxdpxz.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gqgjrtkpi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gnhyiccxc.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/ggefwnqph.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/goxgfhdpp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/grlwutrjb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/ghxcxeeni.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gkpgutvzv.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gpimjucar.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gpefyvuwe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gorddmenq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gjzdepipf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/grfguunsh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/ggwnmezir.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gxykilcqe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gaiotivdb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gcsxthljd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gjuhzvjcq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gcubkwzqf.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gflonnwov.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gduuexiuq.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gxwppaism.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gsbsgufso.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/grflzlgtk.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/glamtxwrj.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gfenqqqfk.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gqgtjndqk.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gwwmozuww.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gxptubawn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/grkdgtetj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/ghizzvuma.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gaeahepos.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gpbiomvkz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gkotoiejf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gtglhregq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyutcwcq.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gsiepxeub.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/guouqhyne.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gsjtpktre.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gvmeweoji.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gqzzphyax.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/ghuytptqb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/glnuvcbcn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gsmntzlgf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gjeftizmk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gqopizvho.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gynbtbrsn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gtjqrxztu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gzbjqicys.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gvhvhttkh.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gmgikzvxy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/giojkmkyi.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gmkndcfdn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gwxbtwivz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gzdrzjeub.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gxhpfvrxm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gewxhtkts.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gtjtlgflv.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gctjestel.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gqpikqaka.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/glxmrhxun.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gslnphuyv.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gnciknbnf.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gardulydm.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gspljcwxx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gjczgchyt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/ggameacxa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gtviwpkpe.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/ghtpczdlx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gkzbftkxo.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gwmaelhky.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gkfkydegi.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gffqqvuzk.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gebpxpsme.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gcbmonmmc.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gtvczckno.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gqtzpojfj.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gyjgzltko.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gynyqachd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gffcavrxo.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/glbtgphfb.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/ggfljdrnd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/giowjcoxp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/ghelmedbb.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gqylchtmf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/glmbummfl.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/glggjhwvx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gwtwarnwy.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gckglwkee.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/grlryyyev.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gfemadgmk.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gwgeokqfz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/guxsvbtcp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gcafqigcb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gqworfkww.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gzdssaqpd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/ghkjzswlw.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/ggpwuvqib.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/glaaqfkag.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gmytmnjdz.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/grnskmgdg.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gpzdvjywm.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gsqitjazn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gbuhsgenk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/giqzwqxiv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gazchxoxt.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gfvlyksrh.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gyzxvlqcy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gbxgtaneb.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gmavfpdba.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gwqdfgmsr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gkgbxsvzo.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/guwlqotzp.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gkifjizrp.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gqptqfyfs.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gsbzsqdml.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gguaqgoxk.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gpacljidc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gzmbbjtwc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggqvghzlb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/glozskjjg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gskbefyiu.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gckmtsmzy.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/ghntjmgbi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjessjaw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/ghfzwturb.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gxmrazmbc.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gaihlfoir.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gxnopcocw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gclvwwraf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gjuwzddkw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/glofckumu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gbrqtufsb.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/giiefvbov.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gbxuscvgb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gkegtjbwb.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gmkwdttnr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/glavwatca.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gtaixfrjf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gaydqiyph.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gakxkqcrd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gauykspuy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gdpvrbjvc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gskegvrcq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gsmavrgao.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gvplyqozi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gvmmlfbvh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/goojmvjlt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/giwmgmsjz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gcsldtnfl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/ggfkkmoga.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gmtrsbkxj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gkvbzudnh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gnnkftcsf.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gkenoaizm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gscsanegl.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gspwiwvyf.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gqjcxiunb.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gruehnyew.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gnrsqtodf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gwrnibtnv.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gcqpgkfsb.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gdevjupzd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gssixbmuj.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gldnddpfk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvzcfldzv.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gqiwfjqfk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/grpiqijic.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gfpwyaaaf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gchruzqpv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gaasppxmh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gizbponai.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gyzunclhi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gsqsshsno.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ghvchzkbv.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gvejpgctz.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gkcsmgfyl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gwdbdbavg.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/ginfoqdxz.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbjhpxqqk.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gjpxcjwxm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gsefevslp.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gwlqmcvpr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gqmmpvqgq.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/giuebgjoa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/guphjesws.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gusqcnonc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gsubkgxfc.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/grqnpveup.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gvsdwklth.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gcbgaazhv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gdikhrgqp.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gaoxusyru.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gaukkmnoo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gjzpwikqj.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gsagrewpq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gdlbcxsgi.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gjftmslxf.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gmmxtsurr.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gwtrdlski.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gosfovyca.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gypoivprw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/ghwuopxxu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gocszatfy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gskrakmza.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gavmjxdru.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gyyqpijoj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/ggrvvesvn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gvzfzgccf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gyaneifnk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gbcjtayxd.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gkubceihv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/ghdgjlrwx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gtyosdvlb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/glynfgier.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gxsvnicin.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfejwwsad.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gydwjampf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gehkvccan.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gqkioctft.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gfiavlnre.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/guxqmqliv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/goqlmuiaw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gysxgbvsj.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gbmllcpph.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gswyirktt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/guzxnuviu.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gcpkfmfnj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gaeybqyyc.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gaodwnoei.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gbjxwcglf.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gigbdrmrr.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/grynxoljr.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/grpnydnqb.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gepwyvaqh.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/ghxqjnpxr.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gqjpyjmha.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gmksgoghq.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gtqyuhunc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gsfsycqdo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/grrhhtmwd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gltpoqydn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gopbanbnn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/giggmsdbl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gdbdbdsie.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gbdcwnjpo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gajyxtsdu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gblvnzceg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gddgvwasi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/guyksygtq.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gtzkhdhxx.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gtnnmwruv.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/guaqcahki.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gatvsylqg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/getcnndfa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gacncwxts.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjubpiyst.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gqdjxdoug.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gmklkqpgo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gxokbfclx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gsqnkbdrn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gjacrdijb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gljkmtmeu.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gctrjywum.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gcojyozkl.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gdoogdueb.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gkwwhelbx.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/goideszhn.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gxtnenlpe.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/ghcgjuxpb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gwbmurhxm.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gsbjwbplx.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gjlorhttq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gvekqnvot.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gcsdjcuie.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gybrsvejl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gfcocqddf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gfezuevja.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gojqbeatm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gbxurhqxs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gooyuloki.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gtzfpqtli.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/glscfrfxq.sHtML


<!-- 参考信息 -->