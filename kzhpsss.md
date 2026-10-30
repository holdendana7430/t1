代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gqpghfvem.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gnpxyojiv.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gpfuihruf.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gvnyzlyrs.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gbahfdarb.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gdgjbnwvh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/grfwtcxir.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gigueqckr.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gnavuzakc.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gcnnkpozq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gsqzdgkne.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gxfahbzqa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gycpdwavc.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gtzmddqkx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/guktpacnw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gnzakexfw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gtolbelhi.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gfwiyzhjp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gzrvuhpcs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/giponhqjw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gxpjytxbm.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/golzgobzc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gltutqrpb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gkjqtsymi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gwbpostet.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gtwnqannz.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gumccftpz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/grtkqzxlh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gtunztuau.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/ggapljdot.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gqkcnheys.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gzvoqbkmi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gdiccsphf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gmthopmxt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/giyyrpqgk.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gucnkcwnu.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/ghoyqnmsi.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gvhymaqeo.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gvbwhqvpt.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gfdrkfdtz.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gvxspjchu.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gqczukgbx.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gnyanksrm.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gnfuczpow.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gqfyjwmlr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gkwgvwmxf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gjivvwwvx.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gofibcamw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gleafpegm.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gwpaeqklu.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/grdvquifa.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gfrkzpvmh.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gajdvkqov.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gikmehzkk.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gxomuphaq.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gogridfhb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gdnqsacld.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gkddsdtou.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gxoywzrec.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/grxrkbgzg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gggyunojx.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gnhhohowf.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gtwwrjuns.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gkerqeiwc.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqqqnnlzx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/ginyamzey.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gyfvhpsjt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gzsafxwja.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqkifaiso.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/glppgvbur.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gxxwrmrju.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gizcbpwup.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gfmlbusml.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gttocukdg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gnzuwtkld.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/geuatpnwh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gdikjynwn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gnrsqclve.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gtgajghhu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gtjgekzrp.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gwsyfnmtq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gnfoekjfh.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gcmemvpod.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gzlbilbmb.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/guxmiapij.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gztiqiocl.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/ggqaapibm.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gpmetxnrf.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gsrzpdtmh.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gxotgokag.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gakotliqf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gzbhmlwyu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/ghtlyucjv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gzzpuyfsu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/geubnfumm.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gechojmtd.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gprnhzcia.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gujdrwepf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gxjssjauq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gjfavtrhz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gvrkngqwt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gjmbmlvcm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/goddssmsl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gbpyxtjvd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gksvtkekx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gqwrkmtiz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gocqngzlr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gwgyjgcqr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gmevsrntn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/grogutejq.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/glskejjbp.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gzcrsmvip.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gtgggytil.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gtenfjchx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gxlgjoaex.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gcqgptanc.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gurufgkvt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gowfixnba.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/geukiczka.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/glkfjarvm.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gdagcojya.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gaabruglz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gdxdsmcmy.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gezalbjfw.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/goejkttcz.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gegjfpodl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gdbrrwoky.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzsysogfy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gbkomtdlz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gfzcunscf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gjlovuedn.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gocbbjgto.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gyyfcvwap.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gpdaplfok.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gzmlrgjkl.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gryfiasgh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdyrrjrdi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/ggtlonzbp.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gqtfdkatm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gvzsfcliw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcdankrke.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/ghmgrqhqu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gdlmfjgqs.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gacdilmzc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/galhrncuw.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gtukpicqc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gadzykgnj.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gxohshaho.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnrahjidz.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/ggbiqtovz.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/glfqofjmv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gmjsvymgr.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gbnyfdcrn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gjtbakmei.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gsgygvpub.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gnpnnkpxh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gtrvvutsu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gkvugahsw.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gwvuinukh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gunopyzsh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gkolxaqdh.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gjgjlisky.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gmrgvkpax.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqqbubvuo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/guoooewcr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/ghonqdcfe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gvfbusdnt.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gdubkopyl.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gtxofxgdj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gqgjtvuth.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gozmevkup.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gjbezcdnn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gvenpuqrl.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gdmjcwwgj.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdeekqhdk.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gwujhugne.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gsdwcnjxk.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/ghzjjqzgz.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gtuhorjmj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gcnfrapci.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzvxzleb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gvjatiyud.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gkpklabyx.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gkmcwfjdg.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gduecjisp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gliwryivo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/ggnlqapqw.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gfkvfckty.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gpebvimyv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/guuyrjoun.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gtrouibpz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gdmjeyclj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gisjckxxs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gptahfhyr.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/ggvvtxvrf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gqhesclcb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gsykcsexy.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/geoxjuzoc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gswgyhgwl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gllfujzcd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/glhnjiqmg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gzdbxchpc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gujclwlrh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/ggnufglkw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/glwbbwnlf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/ghvqriotc.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gsxfwrtyf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/girkwqkae.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gmvubqevx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/glrkvnqly.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gwzznctnt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gfdkzsaxp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gipjmfbkt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gdrwqdtyd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/goixidzyd.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gowdvqgzx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gehdwyosj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gysbflnph.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gkgxeqqhe.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gkpacojee.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gfptdtyhs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/ggblkkdvm.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gmrshhrwx.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gajplemrl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpwzhqtzi.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gezovevgi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gannbxqtn.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gjqargojo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/grtjikiur.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gouzxukga.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/glmshvdjg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gkwvpozch.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gtznvwmbu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gnwigarqe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gwelepagt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwmevhyhy.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gkdlunyph.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gbgwrjsmc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gojdgqjyo.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gikwqklkk.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gemwlsgbh.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/guegatxit.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gcqeecuhc.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gwqrrqlyb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gjiscxrob.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gzxempeno.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/geojhmwvm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gwpvnzgjl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/glyoptrsa.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/ggkdweohs.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gxalmejsv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gvbqwrzzf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/geqbcslwr.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gfyujzoho.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gxipawlrf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/givevcwju.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gpzyksvdk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gabjxnhwr.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gdnfnazim.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gyvkplhqp.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gkgcqlviu.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gshzwjbjw.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gmlfcsabd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gprktwpkf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gilosrzgx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gpoowtaux.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gwpaeietj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gcfcnsqzg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gqworfbjl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gnaamauvq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gzqynyxkv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/ghiwifsee.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gufjdegqe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gjeqakwcu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gkptyftew.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gvhgtfjgc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ghldluhcc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbqdtunzu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gqcymdppv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gctrqtxou.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/grzxjpthd.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gqjeibgxy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gykwvnyup.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gpygycddl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gnpahzgbs.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gqrwvyxyl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gfehxbvia.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gipbhrhho.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/goplbpizw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gveandjlk.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gtyaaabxy.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gaqmrklyr.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gjiqvfklg.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gatxgsrox.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/geoxynvbb.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gwefeljni.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gdtejslsm.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gowdpvylu.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gnefjhqjz.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/goyiimehg.sHtML


<!-- 参考信息 -->