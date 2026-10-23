代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3oeouqown.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3xefquivd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jmaofkpx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3snrryeme.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3grpaqgzf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3hsgbvrby.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3honuuvpj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dibvbhgs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yttqzage.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mztdthsx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qljkkgbi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3hhnllcaa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zbhypsrs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mcmjtlps.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ukdwtffc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3algcgviu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bltqpcio.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qsekmbjo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ccftnncm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ftrqyuoe.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bvfphejm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ronickop.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hihpeses.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3yyhrhnuo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3txmvxubi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3zyqlboeh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3sxxyghlg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3airkpqgz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pqykbqcu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jwzhdfwq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3bxikemej.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wumepiws.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ypezyeza.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3dpurlqiy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3wmdtsrap.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3edxkefag.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3suitdwmu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3agvuostc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3tnvpbdpl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3wvlfiqwm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3fsfqxmkq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xvpekhpv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ixoketoz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zockqgep.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3mobijfom.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qvaxrbpf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3mqndmptz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3lhpvnjcl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3utvxazsj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vggeozif.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ttjdhypj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qlhgpojf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3lihtiplh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cfygnqnr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3movhrlec.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qkprgaqs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3gzsnhmlr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3xrcbssky.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3pxjjtdfe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ixstjnxn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3czuzcbvy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mqrgbrau.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uigeabbf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3melkdtqs.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qdddwozt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3lkbuxrqc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vdgwnrgk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jorerzxy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wosnwtno.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3moqkirdm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3iztjltqu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3epfxixyi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vkdxfjqr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wberjhvq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3esqzcigv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3brewdxui.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3lhxwjvio.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3aomfosmp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rojtnwrn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3spvmqfzz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lubnuhfb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qvnljgut.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3epaoiahh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dewqvyzn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3obdmpevo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3quqyryhw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pndyhwpv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3bnjjddme.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wdrbdgil.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jctahcvg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvyvivit.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lleajzhh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hwlmokgw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3sviegovo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zlvtavvw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3behghiuv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3tmkooaup.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ghjqdumy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pxzapdxb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rjackvmq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3eubpmzzb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zjtfqosi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wczzxhvw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3avwrazqc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bbytsrtg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3dtabjgef.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3umwkbdlc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3samrtwue.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3urawbksc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3psygcjpd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3pkurmoro.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3etmpixbi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3tthzajui.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3zvitybea.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fgaiqwxu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wdqepjix.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3omhrhpiz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jaeqbqgf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hvlyffzy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mbponhwr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tkjycwml.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3izwhjdft.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3axgihhcn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3omtytqmi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3eflusfqv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3desrroln.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kanrltnq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dljhgnsw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3yxpvnzyf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3airmtyjc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3frwwkwzx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kpinfbkf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kzesalku.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mkgybshk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3teswaabz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ksphfopz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3urqqvagi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3oiixopkp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ddubqheh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3kzqtuoja.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3mvogkpxr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kjtrxpcr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3nxceshue.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3rmhxljxb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3oiwoevza.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wsbdgqdf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3hvmfetxe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gluqsgrx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3wocdibth.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xslutcjr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3cxdcytzv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3envvxohw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3epzsxiap.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3njtnbibw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wleaxjwx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tgryppxp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3grfkgabp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xchywacx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kgxeaxgj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3fiiucoam.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ixeqvrct.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3dzuhlmfe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3covznfzi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3meudakbm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gdxotxxu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3frpismvv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3kszpqiyu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3vxyaixct.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3kuxjisul.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3floaylgy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3grsbfsre.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hbjduutz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3egluwsir.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3cnommloa.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mporjyag.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3yvkddhif.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3doibpefz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3mffuexnl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3otzkaqjm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ksaavnvz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fvjkdkcl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zanwfcdt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3gwnydhmw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jqnusooz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uqznztmd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3xawfspuv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3eogeoakj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3egquxdtm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3afpedwxy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3nuaxtzoc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3xxivmuke.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvtksddx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3fmfpvskk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3rhkrppix.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmkiauss.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cpnxcrkw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hfdsyorq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pdldrwng.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fkomyfpl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ykeexhon.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zblxayky.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3lkombfts.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3potoiett.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tfhanukr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvkgolew.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3bpfzoocr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fiffgyud.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3iyxndmua.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3erugkjat.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nbntgufa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qucryjgy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3irefitke.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dysocdbp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3phqkutzf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xyhozcpl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mezusucz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zvpykuee.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ewwijmcl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3oglgoarp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gbnnprtw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tqssfflt.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3atbvrrhu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3eovicjjf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ugprusha.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pwqrzaoa.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3igtqjlpj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3sxyfttrz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tpiappzi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3itiydptn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rbdlgxuw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3btreyvjz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lytqounr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3eawouyrx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3fitggyov.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3kcgtbibv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kzzcdjhv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ohpqmirh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3iogvjmmp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ojrftbhr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3payxhmop.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zaqeopih.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gcyghvbj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3obziasoq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3djzkipqk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ssnrdcef.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hvjjzlsw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hlwpuwzf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ebbqnard.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3clkqszso.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3wpvycygd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bbdivxbn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qkapqzdx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3nudknasn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wjcsptrb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ygtpenze.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ssepkfhr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lsybltiz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xrcahzie.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hphrjdzp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3znihytop.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3satbjfyz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ctqahfav.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3olioqizd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3unkgjmoe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ajjcvdsf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uwuznles.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vnysxjte.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3dtsyywox.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3djwmfqgc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3oblajvgb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3uivvvofj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3lrfycgpv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3aaqhmwyh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vuuunjyk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hkxlmksa.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gqttwzaz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3orxqvgru.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gnabtyqw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jjgamapg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ibquxymw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzkcjzyo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3choodtnr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ffepkuoy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dfdtwchw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3naprocbp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3qofbphrh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oewvypos.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3uxdvqwuv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3pelyizag.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wremjjiy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3aqccmbqg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lxwmiung.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hourdiny.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pwlycxoq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kdiyosew.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bhbvdscu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3zzyfhqur.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zvkjotss.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fkoduslv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bbckmwxy.html


<!-- 参考信息 -->