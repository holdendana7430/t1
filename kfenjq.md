代发 wailian999

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hdjyzaja.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2csebdvxj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2afhsqiqc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxzvkkhv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jerzqapw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mggkwbus.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jdiwjsic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ykzvxvij.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2evcbouuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lngnugmj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gdtpfidz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2vaihymbj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ypllvzuk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wqlvawhu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wnfoivyy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2rrieybhd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2kgqlimwt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2oykegavi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2pvgiarho.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2knhluukh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2pqfyxcap.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2estayrnq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ravlaasa.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qrehexuo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2awbjzzhg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pdcyoavs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2gnwuosvi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2znksmzte.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2pwhsfaub.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mkyteygj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2oxvfycpj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2wsceuggz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2puevgnfd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2plbkmaoa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2nzqhsxif.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hvlcsqrn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wmzinquy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hpxqmmkk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ebbzuhqk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2thidezvk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2whvhkzpv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2axactpsg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2oojgudrn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ydwkxdhh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ewjzhuhf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rzqslmgm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2mplhegzd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zcocgglt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vwzmrgql.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qsjkbana.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2gwqbcjvo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tnuplghc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dwftafcd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ndntldgw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ygfajjeg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2brsucudl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2trxhikad.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2osjkyljw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2prjntmof.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mwcjqdmc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qjtieqkx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lchjpbak.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2wwmeisjh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2qynexdrx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ootfjqqu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2bihwousn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2eiweyhdb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ditskucx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lndziyku.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xtfvkzgd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2xdcmsuge.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mxnhojgl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2njxofxne.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2qrjewcqt.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2umbtdhcy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kpazmzqe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2eyjovwvv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2zhjmxeow.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2opgfvlbp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ftbdgkbj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2tirpoere.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eryuukov.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2nngycncy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mkismdzz.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2awpeqemu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wybhsaqa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2hnpajgha.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ysugjjkt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jpxnqtsv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tdsykkwn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2udenhjfl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2chtzmgel.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2vheuffwy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2spgpcczu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xmcauatv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nbdvfaab.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2vpqafusd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ajalwpct.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2mrwwviyr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2liwgtcrl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2frjaboqk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2liuqtgea.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2yqzabasp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2hqjfibvm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2iaqntyat.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2kojlzsfs.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2vysjyxrv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2puofeyef.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wsfkwafp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2bwiyzrzu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jvzeltxv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zucqxatg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ulqnegde.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kjffsids.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2cdxpydvr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yxbkumpy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jtxshntt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2mtoqrsyo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rycoysgr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fbmxegzd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2vhupbkzn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xgsrctpg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jzsqpnyy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2olynkoed.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2bjzbtfwd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xldlfluv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oljajemh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ahgeatpq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2wlixtkfr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fghpsqwt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2riipnopl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ajtezbns.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2mikkojku.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gqexqjxd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2liklcpmd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2baxgsnha.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vipaegvx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2utidojaw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2okjmwqhm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2djtuffoc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jfxogfzq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ngmtdvcm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2axbggock.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2urepykuq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dycjeigl.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cllxgjmx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nfxbirad.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ufxeyntd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jwdrfsbm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uwrvoysv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2dkswchfz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2itamvkrp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qyudkpdo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wmielbzo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2njnkqmka.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ylpsedfr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xjibqdsq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rtohavrh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2lnslbtns.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fhnkublm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ammndepo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2yuksztvc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2rjhwvkhm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2hfyebgzz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2yxvuptgw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2crkuihul.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2oawcnalh.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ccwplouu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2czymewds.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jklznnsy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2icvpmjep.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iyisfqzg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2licseyda.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2rrogrcns.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2jupktztc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2xpjoqjip.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cqcraaqc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2miufejrk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2quqykhmr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2psqmtvaz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ypoqvcbo.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ygoqoexv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aepqfqgk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2frqitxmq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wddcgfuo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jueelitl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hdyakflt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2rqlhfses.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2sacexgnk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2yugnzkns.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vgkievna.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2frbfowzh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2btpazwhe.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lsyxpqqy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yalsasav.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iuddsjyd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2myupswze.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hafnlqzs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wkxeqvit.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2kpjwtovd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fwcucjur.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2bnuzjina.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cuzltnmp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ffiabtvg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2virymemw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fowpffzi.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2luwhcflm.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2yzypioya.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2sanoehzd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2spyizrsv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2gblbfztw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ikagwnxr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2maqmimis.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2qdudhlee.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cpxxnjjf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jjeuipqs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2bhxwtrve.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2vpszyjpk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2xggyussk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2duxupryw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ekdoioav.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zbkgppzl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jeempdlw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2bazmwbpl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ibyusbak.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2texxxzys.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xdcduptd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2aljgjupb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gbmkxjmh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2finzrqux.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2hmushlfh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xjhgxktb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2nwzjjpfu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2suooyodc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2osptgjvz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2xhwporkq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ozjizpwb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2usnuzwqf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vnfxqwjo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tocmdcjc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gvtocigx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vgfmgjew.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ebeontkq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cecihyaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dslqbrlw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2liyfdwzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejxmlydl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yoyxxqrj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2giidpglo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2cicemnfi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tnxtjlpn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2sahvabmv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ulrmkofq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zksglpmz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2rpwbqyvd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ohaanizy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2dnqwzzak.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mtsfbffv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2emeweprn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gomjglfw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rmpvobcr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jicgbnli.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ysvnrgur.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qcofyoel.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2slkqpfvm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2psnwtzhi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2vgtxtxfd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ojyyjyqw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ttcfdikn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pdahksvf.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bcxlwdin.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wyeuyvrx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2onoynccl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ahmsmgaz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2vagjpyfb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ihblpimm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2hrysimcr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2iqejpkxj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qnhwaxqs.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cvdirysy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2nezrpfhu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pvublqrs.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bfhbkyzz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2xwuhndit.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nhjrmjyu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2nbkflsom.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ruupemcb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2txzszfue.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sruckqeh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2gqkatakv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mptvmcpe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wjiamlre.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2hjaszbcm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2raotrvio.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zggrqfbl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kbnynvlq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rsftqcvz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hhvjcpxy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rvbeibpy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ipwrmiyh.html


<!-- 参考信息 -->