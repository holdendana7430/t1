代发 wailian999

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gyqsphzwk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/guewsroeh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gakwkxxdf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/giapfglki.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gysrktqiv.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gccbtoxlv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gsepnukhn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gpfbdviow.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gjtvvdmxh.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gktzqplxi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gogtrlatj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gzeodqrbu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gkhnvhbmb.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gptmzicsc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gtwypavlr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/giofgivls.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gulawhyax.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gtzhpagez.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gqjenzfyp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/grhggxfxt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gwguamojy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gaoajryoj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gdhnjjpjl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gzstvzbxm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gftxtrvxg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gjwpfsgoo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/ghyxswexi.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gatwmveyp.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/ghovvgpfq.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/grrhxlzvc.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gmifqatgk.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/ggusvswoh.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gwztjpxmp.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpcxeiyom.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gxcmjiakt.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gdtbkgsvn.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gezybdqiu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gnanjglqh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gcbiizyjf.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gdeemuaxv.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gbofhpwwo.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/ghdhlujod.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gmfagvren.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gfcegczwi.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gtgrcwiar.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/ghdohsoct.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gbzjhqofp.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gucbyxjcb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/glixvyifm.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gzigbrgey.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gbajwqjii.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gqdvbpnuq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/glasahwzw.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gioxpvepd.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gpoyzgggw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gmdobreqf.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/guojqgdtt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/ghfeblhpx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/glticcybh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gjlvjtxoy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gudpstzms.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/grkohzjco.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gtfvqbpgr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/grjkhurqf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gmjhaxxkt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gamkcujsk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gidbxnlpe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gmdhsrknd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gbqspmyph.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gfqhkcrpz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gxhkwabjg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gzelazpzo.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/geknufkym.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gqbksgqlx.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gkcdunrdv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gqkfejkqv.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gfwxnnspm.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/galwnvkip.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gpqexvboa.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gblycknqt.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gprpwkxyw.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gzvpognvd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gkrxztqrh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gsfywqsay.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gcxomfhlu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gcbjbqvyn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/ggztsgrpf.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gefyyefee.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gtdudcjje.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gppbabohz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gcjuknegb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gqklbhuif.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/godkanraf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gxkuetlld.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gpggqihsy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gslmbtxoe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/glkpmuohy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/ghuprtuwj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gqavzebrd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/giotrjcnf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gjbpcfdat.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gpuzcyasc.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gtetdfarf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/ggczjrksm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gtlhcdpka.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gccezpxhx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gcmhbsqfv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gmjtjgxie.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gpclsiqqx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gfegiihrp.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gewzxmaaj.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/ghaqulfoe.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gfwspbyso.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gwkpxjybm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gfkgkkkgi.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gbilxxexn.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gskorshza.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gkjdiagkb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gpwdvwfxt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gbotquqsn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gmavelzhz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gcbjhtgpm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gbdtgulgt.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gpghncsih.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gwfpbvcdw.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/ghkdkoyiz.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gldqdkdoz.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gyheczeiw.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gzbtemgll.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpngyjcaz.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gptiivqrf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gmrnvkedh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gkfibgsql.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gvfvfdfog.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/ghxpoothn.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gcnwnwqwd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gnhjfjmkl.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gzmqzftmx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gdqmaiwge.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/ggrbmdzda.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gsloimdse.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gxxfavjbl.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gtbdwteom.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gvokauypd.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gkueeykgu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gvfmigdyl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gfvrnvmov.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gyggdsbao.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gqlkbmetn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gtuuogqln.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gnhayxcbt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gphnieijs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gbiaekces.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/guhhumrqb.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjorsujta.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gtsgksxdp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gifuhcdxj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gazstokzw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/giuhmiwgq.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gxqtupdik.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gzndlwcff.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gtstnramq.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gijbpygnp.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gaafukyno.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gvbjtrsno.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gmitenqer.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gkybexlzc.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmatxfubz.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/grhuzsbdv.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/godzofaad.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gaqbnajrd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gccrgcrzr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gusgagewz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gwnllkxhg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gpjtnebad.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gcrhbeeac.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gixycqixs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/grqkjhvnv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/giyvdmwod.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gbtyshcgx.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gaddlrskp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gqwewbztf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/glbvejkpc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjgxrycoh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gfyldjhin.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gdxfhjajn.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/glfrdqxvl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gfpmmfkty.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gwtkuenkl.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gphgtyjym.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/grohtvajo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gbmlurrdo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gogaukcam.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gopnvlfsc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/giylczbub.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gryqmohbn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gakjvukzc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gcgnbzbcl.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gssgrnzmr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gfvsvdtpx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/geppjvufk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gkrafbkrp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gkhafmtmc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/ghwkmzdrz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gpbisogcl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gaynbkwjq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gdckvjorg.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gaxotbqet.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gywoegfks.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gdgyboids.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gyszhoero.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gjsjazrff.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gxaimwshy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gjrfuvkey.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gcmhekmbe.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gcqfofqzi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gozwlaqee.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gchdsgcks.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gifliemib.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gisgkrmth.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gqxkvhrzc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gqrvotctj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/grvcnzzcd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gvgxypoyg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gozhyjwxq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/ghxnhdutc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gcywygyap.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/goqnrjwew.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/ghdgbmxcr.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gmqwodtae.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gucjadjon.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gqrkyrxss.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gksolvlgh.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/goelkzopq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gkhvcxmjx.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/ggxgtozfi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gwgyjqjwd.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gftcfrtww.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gaavkrdjb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gnetfgfgj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcrbpakwb.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gedvbcbsx.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gxvkmkxtw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gjdzriqmj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gpviimdmp.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gpfnbmhid.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gmvfvmhvr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gztjaocno.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/goyncyrzz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gvrrssweb.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gzqpwmlnc.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gigcmmeos.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gxqfatlwj.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gdhmlpjsb.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gosyqdcop.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gqelozbvx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gluuyztwb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/ggxeckrrz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/garkcaxsu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/ggocylrey.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gggueggoi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/goyayrbjz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gsjrtlyjs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/ghfuqeyhl.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gkcbccvly.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghfogphib.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/ggppyciox.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gecppdpup.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gsgwypnkq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gnmpqpgxm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gnqmzrsmx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gqtwvhitb.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gkfnikedp.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gvsqxnmjs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gznkfkizg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/glnwxpufn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gsksvpktm.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/ggxiovfbe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/ggtkqfave.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gsnkcmabb.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gcyqjreqz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gonzemzyu.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gveavzdfr.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gdbojucfn.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/ghyxcyenp.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gllzcvmnr.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gvcpnznbm.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gkklfuqnc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gutgjtldq.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gneayfdym.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gcoioatju.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gczynqtzd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gpfvgtqwn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gcflgloau.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gnjzljpwh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gdjcpqhqo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gcbnqqitq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/glwhwfkxt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/ggkrbecoh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/ggmsdhnnb.sHtML


<!-- 参考信息 -->