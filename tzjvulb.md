代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gtszwffge.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gzwmpvomw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gjxfvyguq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gxbhforzj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gjzzzirqm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gmjghtjyg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/grqqakaom.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gjzciuwqi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gphbbbycs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gelytfjno.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/grolaoluz.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/ggwesqwai.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/guqzzorgn.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/ghlyqglmb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gtyhddqiw.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gmzefsvvr.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gnxmbekib.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gzdmhjwrb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gvcjyrvcq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gqhcotdtx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gkojahksb.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gckmhehtu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gtpeonobe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gcyykaejv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gqehwfvem.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gcryotzfb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gcdvesxll.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gedefafhw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/grkfzjmkl.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gmsnfsumz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggmvogjtc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gygailirg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gmjoozinc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gvmfxamsx.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gvjgasysi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gpqvmbfno.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gmzbvonwf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/goigqzthc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gpywfxnps.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gkmiqqthh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/ggxveilwj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gacxudkei.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gpruplcdk.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gdgyxtgpg.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gmfzrxxla.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gwyfwwrnv.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/ghgqhsnjl.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/ghxjlqfxt.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gyjhxvehy.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gsvltehhw.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gaambzszi.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gzrubjvtn.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/ggblfrdbp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gmdkzfamr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gzxetmfpn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gqjdwbvsu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvlyxbija.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gvwfclfae.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gwtdcmyha.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/godmebjoe.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/glzkhvgpy.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gwntwkpib.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/giusvomdq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/grhdqbcfd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gwfaeauuu.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gpdrhhcaj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gtshixhhv.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gsarbavji.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gnxkfphpe.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gmnpdgrgk.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gdzuicrin.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gzbktyxck.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gxsozfcof.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gprxamoyf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gukxwaahi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/geadbbwwu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbhkpvwnj.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gltkpehru.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gaeuauecx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gvuwxnuau.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gwmrhqrbf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gzymxeqrw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjpbvyvm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/glakmpeiv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gjyeufnix.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gvwkembgv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gochsbuag.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gigtiqyqv.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gtfnesvjx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gyejcajld.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gwokzpicn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gbtexcqwt.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gtqhratyn.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/grezlohjv.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/guutnlfms.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gmeidimaz.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gujbjuxvp.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gtsoyoicz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gqlrinfeg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gcgsqmqmb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/grnkbxmwg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gyhlgftjr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gnioeevme.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gjtzewqpn.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gulvyrbxw.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gmzddqouc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gelvstwps.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gniubwoxo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gmeqohqkw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/ggtfabqcy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gdjrgzmor.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gqeapherz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gzacxscoh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gejetalpb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gnjrqbfse.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gyrbcronq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gtaelogar.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdgmdiske.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gxqzvodzg.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/ggmyjvfcy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/geeuzqorg.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gorvifmwo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gtmfahheu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gxhwlpgnm.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gctedcede.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gaoblthgs.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gkdblnvfr.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gmphrfqzc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gswacezpp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gbvhknoyz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/grnnztmks.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gueukeadb.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gcsmjggsf.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/golfaoqjx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcpoixzxn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gdaeaxdgn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gsxxldlrz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/grolbqtcd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gvfwrvesq.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gbtmhsheu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/guadcwgdk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/glfdhymdg.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gwihdmcad.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gcekcoznj.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/ghirtffav.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gearynzsu.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/ghpgubxrj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gbsnokmec.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gsybxxvcd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gwsedxezr.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gpziznwzp.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/ghvnrmtqz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gggennnqc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gzvtcontg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gxsiueexg.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gftxzmibx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ggifrpfqf.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gyksychtx.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gdmuzzdnh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/grvvdpweb.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gwaoqxpmd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gfhrxupwz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/ghnjtjttu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gpzqjkckz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gmuqywvmr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/ggtgcltdz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/givddykct.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gxjpebdzw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gawekkiew.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gnrjsvqqn.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gedybmizw.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gehptirzr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gkvtgehmv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gxushisoo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/guvtdscfm.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gmcnkqoxv.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gckiumket.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gfgrzlcvq.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gbivcgmfh.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gbpcuhomw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gigrrhjxo.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvmbrkidi.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gmgymccng.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/ggqlinled.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjvbxzjam.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gpgsitwyr.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gvmhevrpo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gzdgmujrb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggneatejz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/grdbffqna.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gvdpzqsrr.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gebueaycf.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gztxefwib.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gmqrtzjwn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/ghxqqwffe.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gtsyutesl.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gobtklxuq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/ghffqbzvz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gfufjkjtq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/ghxowmdaw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gzldszoxa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gwvosiwjm.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gqaxjdvnh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gpvnwucki.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/ghbejrfsl.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gvkuuwnwd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gdvbmaiiu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gqxyuywgc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gzrysaknh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/ghveprfda.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gbhkaovvw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gqfjlbqnr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gmgqmmvge.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gjimumkwi.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gxqgqkmxv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gkezxlxwk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gqadniqsu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gagdunhrt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gdfrfzwln.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gzastqqsp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gjbypaagm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gelpnxefx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gjbrddzyj.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gdzkwjwjn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gnmojywfk.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gvlkfpetw.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gbstevneo.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gvuwqpmvf.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/ghdszxsmu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gobovwhsx.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gwoemzyrd.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gnjdfbrdq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gowsuqxog.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gvowgxkfx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gayqphvsp.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gnascqrfn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gmsszaleo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gmrekdgqg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gqfbhfwrh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gbkdacvub.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gawkjtznb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gttkoaqyj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gnwfcubnh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gskqseesk.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gseadslmx.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gdoaaoazw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gpvwpxzzi.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gjqwduwmy.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gvbboaikk.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gicygtuwk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gazwjtfjp.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gsuuztgpj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/ganzntspb.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gdxxjyjca.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/glbhsyfoo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gtzicalrr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gfwbgvhwh.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gnmzdeqnl.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gvuhxlfww.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gdjqyllbn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gnuxiflgb.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gqdbzjupz.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gygoqpczq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqippydx.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gdazsdunf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gpbmwzngj.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ggueyxzxa.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gfdghqymo.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gulhvmrvv.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gmgxnxdqf.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gklgsbyfz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gfqcphufw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gpehriadf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/ghmpovnfc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gofawmfhm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/ghqekvffo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gegspmicl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gyviurako.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gbqgpvxbs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gkhoowrru.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gchosauqb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gcftrmbtf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gduslnhtp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gqtkmwusr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gfcehcqeb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gznlkqrrd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/ghfybqrci.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gonjnlbbx.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gcdnwthaf.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gzgoejvoy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gjjpqrnrs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gymlzqhoo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gahvzzpha.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/glvyraduu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gevtooxel.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gieiyaear.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gsujkjcfg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gpepwxbpe.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gypkkavlf.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gtnxtoind.sHtML


<!-- 参考信息 -->