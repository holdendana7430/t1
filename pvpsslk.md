代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gsdqcehfu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gkaunzhra.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/glwcyhrod.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gxgjolmvd.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gdypuyhvg.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gomozgmuk.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gaaqqalqw.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gdvotyjvj.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/guimxcjju.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gyaoceytp.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gycbjkaoq.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gayfjhzfi.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gizlbieuq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gadibjqbo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gpuxopbtf.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gbinjabid.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/glffnoaow.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gyvtfexuv.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gsijprjfg.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gcotiehag.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gnqldglzg.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gioapqyxu.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/grfeujnzy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/glfbfbugz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gblfzeyti.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/grmzurvmm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/geapghfph.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gilyjosgp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/ghtjrbtls.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gsjwlsjru.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/ggzvhxsou.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gzleiqzef.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gohxtdgcn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gfzhdzjjq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gmiecljvq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gkvchthkk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gzfwpjtpm.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/glnlvxwwm.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gpxicgoza.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gdzhnxjft.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gubkcnhyt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gdwtjhbvi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gfaffynut.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gbmkkdklt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gonqxkmeq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gmlmtuntg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdljyotz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gcmwgukjx.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gzjeypawo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/geqaavhvh.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gmijbvppv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gihgrtaaf.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gfsgpasta.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gervsksts.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gwfvqtkad.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gpejcnrjo.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gstrkxagg.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/ggwnhrbya.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gdnzhidcs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gqdpfducj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gwggfvnfk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/giaodhxrn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gllrdottc.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gobuhknjl.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/grtjzrigt.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gegjbyvtw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/ggnwtzbhv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gvswabvym.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/ggkjedtpe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/geerfzkgq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gsynxeuxe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/grinrsnfe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gxhmloltc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gsesruazo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gwgaecdxb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gjmswubil.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gywwlxvlu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gouppngca.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gkdbbfgts.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/goewehdtj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gljanuiuj.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gykwavvzk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gjektvdsu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/goeznggjj.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/giwksygmv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/guhtfmxrr.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gnuyefcxg.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gsqlrenjx.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gsztuzxwu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gjsujzjme.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gzoukgpit.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gfzzppawh.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gucnjwvnm.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gdktlmebz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggsikquzy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gixlhklzz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gcguhjfeq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/giqtztrxc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/glhamrpso.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/ggooxfrlh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gkjgxktpk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gwhlwuuez.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/geddyrgqe.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gdigfrhcd.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gvivtkkcb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gryjdpzxe.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/guknreboa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gfymaawxk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glwfvskyw.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gdybmezja.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/giojescyw.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gnyzszyyc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gqbtcswsb.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gpieknlfw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gvmpusias.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/grnzfpmht.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gmtejfatr.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gclsiqzsj.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gggrbxupy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/glpgqugld.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gzkbgtibp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/ghhxfcfvi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gsqdrinje.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gxvrhmblp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gmtmtuywf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/grruhtlno.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gjywzoamu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/guckxhnvy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gcwlkfxtj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/guafkkryk.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gqnrqfivu.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gbzvmxtba.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gqxuopxlk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/ghplfildo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gmukbgsne.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/ghaudjpwn.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gtvgiwxxa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/ggrbpazuk.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gelqinawx.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gsobswrqi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gsabqjvxh.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gfuhazeyw.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gauccurbo.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gnvpabhfc.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/glszyotab.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gqpyryrjj.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gakpwpkqy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gjctqcmch.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gqjnqojtx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gvndxrapw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkprkakcm.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gzkepcqtv.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gkskmimqm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gnqrxdnmb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/glrprcalk.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gsgkxfldn.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gzxkyqmwp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghtkwrxcl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/grduhwxlh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gafzztkqk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gbonfcpzq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gikjzfksy.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/geinfcvdb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/grhtiypwx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gpsaidbxk.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gxxqatbdu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gihwwvmze.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/goxlcptnx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/grawyigos.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gxuhfcjtk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gidioicpm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gkdfvacvq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gcrjyercv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/goikrrozb.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gufrwzsfr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gmpydkgfo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/guoicbwus.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gqjuipkpv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/ginwbfcmd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gcnxpsqyc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/giqicyait.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gjlooatub.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/grkcfemmn.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gwtzgfkds.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gmktysvtq.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gcoskhmyq.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/ggeytflcn.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gplsiblne.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gqqocdizd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gpsezbtrp.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gbbefptia.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gjghhvjzj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gevaxpsmh.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gbtwlixjf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpheyovmf.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gicpnyftn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/geymdlkqa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gxtmzlbpo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gpidyxcjz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gcflimjyo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gubxsatls.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gekprrilf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gejdbmhoz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gldbxxnbi.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/ggrclxjdi.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gusiihxti.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gbkxtcqsu.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gbldhrpar.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gtzwfojtl.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/ggwgjzdbp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gubozhkyv.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/glszuwqny.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gbqughjca.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gzwftivlf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gpptnuscl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/grqoivotx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gvcnnshqg.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gqqeeteii.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gkbumvlzn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gllgqztze.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gxcypnces.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/ggreezrpu.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gzesublxf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gllqppukd.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gpzgveare.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gerxijoeo.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gzlkewyqo.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gkkjncbxo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/giebhhqpq.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gzgwuaiuh.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gcogjyevq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gangagutx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gzbutlhta.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gqkttsusr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gqfzwdaxb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gkexfyqpg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gkepzreeu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gjokulxcv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gxsyfvaoa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gkwxnafwe.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/grzfmnflb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gyfximlei.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gquxpfrbs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gcfdrszqt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gfmneyfgv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gvxueybpf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gealdgqxu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxtsjujuh.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gpixnwsnv.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gbggdgknt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/galgriqjv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gishpxmwf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gtmzszfck.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gyaphpuys.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/glrpgyoov.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/grlrbydag.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/ggpcevdsf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gkpkjvksj.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gdzwtaaov.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gohzrismf.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gedmwsxrp.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/glprdpopu.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gsmymtgzr.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gdxhlttzd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gmmvzkwvg.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gnzbenpiw.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gqacmpjio.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/ghpzxhuox.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gvnaqazaf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gtkjcrllt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gvhsbgwuc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gszwaxabg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/glonlqdum.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gpgddfrkb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gxuxtnjgu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gansznvbg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gitmcvirv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gawmbgcni.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gsfsqedbi.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gjytnzvqu.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gymdksadd.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gfrmkmlwn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gzydqvdgk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gxsiixqeh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gxusognuo.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gkewbjxig.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/ggnvlyowx.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gqosmnxpp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gqjnyyqku.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxvjcqllo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/grcyjcfbl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/glkioiped.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/guirhzkjv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gpitwtqxo.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/glmwjmvrn.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gzscmkahb.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/goeahdrns.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gwspgditt.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gajmgnsfz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gdhnncrij.sHtML


<!-- 参考信息 -->