代发 wailian999

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ykexlywj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2hzjwbixj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2uiouqdgv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2pgzslias.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2eybssifs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2awvqeznk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2eljjydhw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhwaweff.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2yuyixjii.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2frsinixh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzdddjhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdjrnnjt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2nuiizhxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkxeoeps.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pxpwrxtl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fxhwchpw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bkfoqzkg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vztpjxyo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2punhddhf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2norlbahr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kofhmsxk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2afweteeg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2azqgxhla.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2rrpmhvlq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2hpfvdqny.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2txvfnxbn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2axgttzjw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ktknweyi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sdobbtew.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2owtkggge.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2pntpdpck.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hsqtpbnw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qzrliyjz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2esdjdmoo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2iqvwezzr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hsnrrbyk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fqxeicpy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vfyfmuhj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zjaqjzms.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qscugpau.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ezaztkex.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qdwohvhl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2gpdmhhtl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2nyatynza.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2zinjlqxb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kgtihhlj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2widuflor.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2cpfqcvom.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lbjdiwll.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2naphtefr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2fnrygdzr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vhkcrzvh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2trhibpss.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gisvoxwx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ivpqfxsr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2uqtldgmx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xaegdxyr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hpetjake.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rlqpjnqd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ntzoqova.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ileclway.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ngeftloh.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tqtvupfp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2sszhwscg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ilfjqpdu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sfvgkmpc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2xeeyepuy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2goyjbegl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2efwttrcp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2dtqhhydu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jusptfwz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vwlfxkwk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kqqaypgg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kscqtehx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ojclsugo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2tdzyqggl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fuirkags.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ltoxtzyt.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2aaxdllxq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2kkdaukio.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zhagaacx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2luyeyfrj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2uzynfrsb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ccciklyj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2lcnfgllw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pikcisur.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2bqlcylkf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mbtojezg.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ersqfbzh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ikivnvvp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2nrcawylg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vrqrnvgn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ajmkgrac.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rfacccim.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ltxelqnt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2swcwwcps.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2hthihsix.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vbketdon.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2idnwlnlh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2quthtocu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2sdtvgswn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2jgpowzbr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ocdtzejz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2sbdchdql.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jypczgck.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2brknzjme.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jvigqxxi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2lnduqpkl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mfmjhlbf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zubgiljb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qbiaebne.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vsahchwd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2cnyxvnfo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2gttanvxs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dilkfdtg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kjbvfgsz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hmvrmiez.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ggkobykl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2godlhode.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxlevfkg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cezhzwry.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ldgrleqr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nxevlvix.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2elozjynw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sbhjparr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2poidiigr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xtefmoii.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cuoewrkr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2lwsyknuk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2nodglfct.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zbdikdqm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2czpeszgq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qkchbmbu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gofnueqx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xucjyyrl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rjpdepwc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2edvtrxzb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2iumfqvkm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ptucefao.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2swjpwlja.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ubofjmkd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ciyhwdtq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tcinqcxc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lttfktfx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rgwhhxzw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2amrnujuq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2pmeurvmf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2nacnbaqm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yszealbe.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2osnnhzdc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fchjzckq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xigyfqkb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oduxyauj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gspkuizl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2dfzmbjof.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2eixxxzfb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2bobanavz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2bibrymma.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jakkyiaw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2emmcoadd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2unkogsaq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ejzxguok.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ibxhrasj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oljlghoq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wqfmydul.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2gynafpvs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2sibhngqx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2xovhihhc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2oeouoksk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2yngrozqt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2znojarro.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2nmnaqsyc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tvtsxbze.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2iuwprtym.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2kclfwpzl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zwtbwpse.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2cirosnsq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2gimfeyze.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2gzucfgwy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2cdkvpzel.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dmhzwpnl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xqmwcfoe.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2mngmgchl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qfpsgdoc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ouwbrdgb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mtewjark.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2uarfbtwd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2htyswabu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yejzifun.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pxdhkqhx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2fywoiotm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ijjjalwm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2siekssfy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2bbqglrsb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2tydgsxjg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mjwyisfz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qgzmpwft.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxtijsul.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fsuwdlfk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wqgmdkpl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ulouetca.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xakdipuw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ucujkabp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2uibrotkf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2idjudicn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pxcbngoa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ocdoyizv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2upjzytdw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2enhbtmkl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2sjarlxmg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bfsbxhbx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kyjdvads.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2hcnhuygi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2bgchmcta.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2stjxvgam.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2levsrnwn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lpdvaukw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2shirgyvh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eisroley.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2tjigndff.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2onwkrajo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2tubmxllr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ohpabube.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2tjugrlqq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yltccodc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mcdbciiv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qkyxvuhk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2viuctcye.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2oziiotgi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ochhwxhw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hxjatkws.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ahkdeqrq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mzqrpgif.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zmfpqjfe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jvnfjwok.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2emteehhe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2cqcnrsye.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nbcqiwke.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cizahkqf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pyadwrjg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sgrxepqt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dzitplig.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yzeqsfhs.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bahdqwja.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tomaujec.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2xlafufln.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jqoiyeev.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wqrfuxwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dopfwxpr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2spmfpnqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjbgwvix.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fdwgnzmh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2hsetxxib.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qtchgnah.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2glktbtup.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wfddefhm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2retyhuqo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2npctdrod.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2evbcjtyh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rnytzjrf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2damyzmlk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cnzaslij.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2goqculqg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2arljvaxc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mupevkvw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gwkxbqjp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jazigztw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2sivadmsl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ptzvhoav.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nftfofte.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qfwmumbq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xrkzbuvs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pdhdmlpi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zuclnrff.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mdhawzen.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jlgvzhxo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qdxjrngw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xralzmis.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2spxuxmnq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bjwxzpkf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2crycfdxp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2qrwnrbsq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zjcitzhk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2egpumbik.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2bpyjdsjy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2posrhtue.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fhkzwwec.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ktldhxdi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2tdtdxixt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2sfkcurce.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2icazjsca.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2yxxxrgvn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kwtzaqrp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2xtiduypn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nwpneivq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2layqrnnn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2svdsuitq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ipqrkmpm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ojrgzahi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2imctbfeg.html


<!-- 参考信息 -->