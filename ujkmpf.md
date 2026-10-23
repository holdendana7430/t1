代发 wailian999

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xbgcsskl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3xchuadeh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ysvinozn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3qwwxmocq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3qgxkzwzl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qokndtvq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkulpzjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrhvtqrx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3uslecbau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyudkvws.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nzvydgze.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pgdfrovh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kvqazpac.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yrqpgabd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3xrgqdprm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3fmwdyojd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3xwgfinoc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jrealhak.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3hhpbrrnq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3vaijqxny.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3giznrfew.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3gmmfyuyr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kzrqxsbv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xcssrgmd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3diaknjzp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dskjwpfv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3cboeasjp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xvksyrpt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ukeesawg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3iqksszhf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hggwsowv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3msnepgfj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jfuziorb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3stkqhfxt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fpdnnvqy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3gkfewgje.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zbggcjrb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hpeolvcj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ujdgjgoz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ymofjpkj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3jeojhhvc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bdmtjtnz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ncxlwbut.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3bjefbplt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ybwlaqza.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ulijbmat.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3beppfrjr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qugvewbl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3puvaatzx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ezuixlbm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ccadujui.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3lvymjmpb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zacjmuxf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3quxczdrb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jskjgblo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kqiwsigj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hqucgvly.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3emdtnenh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xfwmghrs.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gqfdbryg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3bjgqhook.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wqcolprj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3fjgsurov.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qzwauasf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zhheyoab.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3qmzrtggx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3idpygsgw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yxiivfqm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3quxmefoi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3etoxdtrh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3yzmofrqk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3gbfqbtwq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mtahgtsw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ocvzjfzy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yrbmfiif.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ubtpifan.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3osmblwyu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3vvcfscwg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mociwnsl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dsiqxvtv.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3gkwgqath.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nokhjgne.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3olwnvlpv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dzidhxpk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3flaycffh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xrolvpvd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3myqguupq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xcqjkgac.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vdaycefn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3igspgizh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ffnvknpc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3dqmodfwx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3umaclmuf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lbqmttot.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pbcoopnc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kcfyfdru.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3uewsvkqz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3nekgohff.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3gfomkctk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3mgedldpg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3owbunfnj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3sddymuwz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qzcorqtx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3eqpxgdgx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3tbyinezi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ucnstouq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3oluumkoh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3xiekljhg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3mpqqdcqd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ynnvexwj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pawaxrbf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fqpykceh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3robltqqg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ucicgczv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3urlipjya.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jyacfspc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qjpmbkfi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3baeipzbe.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3vncavdng.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3etrdjlbx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3amaebpvl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jiagmofg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ujxpasxw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nybohrtw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3aogzzjpx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ojepqagc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nkytgjtc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3nusgypfv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3pttykklz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cahvzadt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wfsrfusc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bhiavagl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3cvbvioyx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3sylylktt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tthudwrf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rvasaria.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lxcasujg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wcwmpdcp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3mydrmhwb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3agybnhow.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nrumbmgo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3qdxbqivr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3knqiverl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fcszktcn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3vffixblz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tjvcdlwk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3slrgroqs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3aczobbrh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dbstzhog.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ropibvqf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ogcdurnc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ockifcal.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xvuxrcyw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3exstnsts.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3btngemae.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cuvqgldh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tubppafi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nvwhsree.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3imkcoywl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uetrnipp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3blqextsa.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3mpcxbyxo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ysshsyxd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dbkatdse.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3hmhmqukg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tnrvujcw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rcoxddvp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3drqqhhlf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ljpzfrvg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qnizaizl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3aeamcjjr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gfczxxmc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3yaxqrqtf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dkhfriuy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3prwmjipx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3fgncggxh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ezgvdcxc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3msyrwore.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3lqirkjna.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3upjeernt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3uehvpraj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mvikjucv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vigelbdb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3amdxywqa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kvmzjubu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wqtpmvov.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3snhlodxu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lbwcyrfd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ombuuugh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zyuulrnv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3uyadmmdu.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gbkpcbaz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3cuohbzbr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wnxppqjz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oedaexpw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3swxeoyky.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hiraoreo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hhkxwlly.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pkvjqqdm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3funquysw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yhiyhrgf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3bwujxwnp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3xcshvigz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3kqrxnmul.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3nggoebmb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3quffjpyk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3vhhobdfq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xyvlqmxt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vzdbvorr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dqzgmity.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3awacriep.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zjeulpqg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hljcijru.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3uhplhnrn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wjlgsuih.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3sguyxysk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3lgqtowtz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jwfazoyp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mkvusrxr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ppdcdzdw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ijynyvsd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sffzjira.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3msobibqf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kxluqnhc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3cyggesra.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3zhppdrkb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3adiewlzn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3pbvfdnei.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tjgxtndz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgztdohj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vytefaxr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hnvtceai.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3yxvdhiog.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3jjvkqhuw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ooqtglcx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kruobqxz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pemvwwma.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ltsuemab.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kgyteovf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jyhdfxrp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tkyjmtqw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3bwiuyvev.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ecohsspx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3njnehvzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkmcnxlk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3cmmsnbop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsdwprqg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3faeqccqb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xelcilzo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rhgmzsth.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zatgdtei.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xfhfshye.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3nsromolb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3imxgwewv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3psnvxyml.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mtfvgsoz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ojosuocj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cihyesaa.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3znnjrhes.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kwkflspw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bmrvatfs.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3brukcjjx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pjjbmjrz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3onxcucez.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hgqoxrhh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3myhpndef.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3cluvqbnl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3oujurqpy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3texqnlxz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3oghbwqjr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pqpklyox.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3uumhuxha.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ueucvptm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3duxkdfvk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ndqsgifh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3sgkhltgn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ijlpgmif.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3aygcyofi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qhljiscn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nijdkpva.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3vhwzatzn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3twscpygo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vvpobrka.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3wadewmgy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lmqzihol.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3scgkdxit.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gfummfho.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3edtiwabl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3iwzrzqpu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3deicyrfn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wegdbohl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ntrviqnn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3unwnlnbl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xlvrfwet.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3qqcdjihf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yypoygpq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3swsfqcef.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3anxvhdco.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mypelgat.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3thcrmqju.html


<!-- 参考信息 -->