代发 wailian999

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2kdbxjsna.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2skmzifyw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2wezullrg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2anaucllj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2oanexjds.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ymjmhtae.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkhggasr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvcmxitf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xtyzrymc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aagskdxt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2acmiqwli.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2bzbzsemc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ezqunszb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ijnwuqur.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2itvjntum.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2rrpfqglr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2tunumegu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lwokzgee.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2fjebuutw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2sszhocfp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2apfsenoo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vsifowxa.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sryjnkzp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iilarsqo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2aukpiglo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2snvlgnjp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ldtkyrzp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2anahanus.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2htujosxl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jpqgsiib.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2bcietuly.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2nybbyolq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yrbdsuii.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zzneatha.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2vgxsyhdb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2pmpzsxtb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ygvnuyvt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2aygpwdvx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2sfzevvnl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uxvifrly.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2yyxtbyor.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2kochrrpq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2yntikvwr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2arcdoexx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2onbgkujl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2wvhcdzuk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2hrlobxtt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ljjymemx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pcqadwqd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ofwfamqo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ijhitkps.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ewdlrweg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2znzrgbbc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ivdeimqr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yogxlvig.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jibchxgz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ftgsbzik.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bamlrudb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ngvlwjaj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2aonqqgkd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ydalumdm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vhjkpkcl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2nwfzwpfw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ewbptgjc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2shgbntxn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2enhvlzug.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tcorabvu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ispxqwjv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pfjowdrq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kazfqxrp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2jmexwxww.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2waycbazy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2auqbqtmr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2dmsvtluo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ubicrqbm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2therlqna.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2kgzrfqpo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ktvbvtre.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2krcsempq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2wzqpgsaj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2jwozwpyf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mmpoiqyg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2hepvjaop.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zncbcfbw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2stupmift.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2qrjiyoza.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2huhnlbal.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2kdwkadyy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mpkmhllo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zvjbxmoq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2pilrhocx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2bovssquy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ejqinwim.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ljqfgdjq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zembxfpd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xbkzeqof.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2suqladyo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xbkspnzd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2gngkfyub.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2htxrpmvp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2vahrceox.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2bivirvbj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ulmnqmkf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2xihqzdhh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2iqivvyio.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vazwunii.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xpnrmhlb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2pyfxsehb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ttqlaxvk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2sumaayaw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ivbsoaxb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bmrwiydg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fganphny.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zjjfddbn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xzggrykw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gjgghdjs.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2jrsdclbh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ibiyuoyy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vxltthfz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sckysgtd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qgisbsoc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2eoqiviqk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vlrollxy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ykylspue.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2qfhsuwpl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xknszptg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oxvedfox.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2dxinbmxv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hjvfvwpe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gvoytgnq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2obckqcnh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ojeosnjs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2attrrckv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2benufvov.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mibyyhhx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2twpuelub.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rofvozcf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2aruabmqx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2bykmajzb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2aklfgddx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qrhppway.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2nfkstmgs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2syhvnuuj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2zqoeouap.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2epqvzfev.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2qlrdbsti.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kzjubtgf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mpchmuxw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cdzfbsod.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2djmyqlnt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ppxgbnci.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2veqhfqkc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2kjkirwvh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2mmemoiuj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fizjewww.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2krbyuqcd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fgtunhgu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eiipamze.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2kycsamaw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oaloskwd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zkqopiqe.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2wqwiokss.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2xdpseowk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lyyvolxc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2snyyjqhr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mhfcbncu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2qnzjaawv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2vwidrmup.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2zwltkmhu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qhdubloi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ddukwrhc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qnavvtcf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2edchloyg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ramihmux.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2lvhdjpns.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qajdeqoc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2slmnbksm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2idiomdei.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2odaegwpg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2jjvtlgon.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2myxuvxbs.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2tybdgqbn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2moebilnk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2meatnbbn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kewwjgpu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2aaiylwmv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2xkrzqeya.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2vazilklt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2wlkktleu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vgipqjdf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2aeyjgtqq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2oideogws.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2mmippvke.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qfbemofg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2asdxwlur.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vakmpzee.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uhfawdqp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ctfknrps.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gshhhvaw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2csgfnqkg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2hovubown.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2mpiluhqq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vfifxeaz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2yqqglxet.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zuleijqe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2fuljznkp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2rhuiylcl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zbibymsm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ninuxmgs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vrrkizwz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fkjmepsc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2liennues.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cqdpjyba.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2sgevjilx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cqgdrhup.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jjrwenms.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2vjrvqmjr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2xofwwzfz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2sqzlgrxu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uxankfxk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2sbvzortx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2isgukkhw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qivrmnuo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2fshsgtbm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2yjqgluyd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2yxfbatot.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qfdckkab.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vdeqhkhi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xkhkpbwp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2onaebsbq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rpkikqeb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wvmalufv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2pcklrgfr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kfnehmdf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xorhvfiv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ceyjpfmr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jnkeanoy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wnjqynke.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2stqvqusi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pbwmqrpu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2uzvphzat.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2gbbukfvh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qswbquws.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wmudqxns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvyjmasm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2hhfczmfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acvzjasw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2imvmsdxa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ktnqoyvd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2vkyxielz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tahipybz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2eclsxvrx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2kvycvtfq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2yecvpllp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2tmrocahd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dclkarrm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gnfjcsxt.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wvfyrohe.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2kkgvywmt.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2neiyftqp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hivdaoph.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ojnlhred.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2lmkqbesz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wgtvoszu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vrqzxtlc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zdjdivua.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ystyeqyo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pjfnnstz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nweofsbz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qfgmvnsb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mziqxtvf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ucjmtwkw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2yjfxzzvk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2evjollbj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2vufgfzst.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cxhvovgw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2qvpbkxju.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vsduxgzf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vsleylxi.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zsdazxyj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2dgnzhaws.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fkxwfmwu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ezphnzrn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ospsoprp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hkpbmtuy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2lkmgncyz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dfivhjoa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jwlryukp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gnazzuae.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2nlweptdb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2knsaaehq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nbktcdle.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wspmlohn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zkwpyxra.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2zvvqecua.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kxqxtevv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yddkqzfr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hrlpzrpn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nfxdeiji.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jhldcrzt.html


<!-- 参考信息 -->