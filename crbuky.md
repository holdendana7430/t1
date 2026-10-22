代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zruogmjv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfxmnani.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ojobdvga.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jqemvnzs.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2pvdtdtbr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2odambvgq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2hudhqsfo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ppbpfskc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ukopiabr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2mqbhrhvu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fjrhsoca.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2uspurnpa.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2iecscwuf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2jqpcubhn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2huznpirh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2etoztzct.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2rinctjme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvbhvpuo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nxncckdv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ifgdvtsj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bqbgbtsf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lclgddyk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2yzfgzrxn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2dcnfdxtq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2dyubtjtz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2hlfctilo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2wnsozvga.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2npmxebcu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mgjuvyry.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tsvgockm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2neelpsbq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pzwgjfzz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rqohxiup.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qmwltvco.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2fotqplxz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gdnnyjsb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2utxyulxk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2psuauzqr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2fnarzihy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2zkvonjfi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nnooefyg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fxekgale.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2oizheinl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2eciqlmrc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ranaiwdv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wstufkbc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2cpmdtrxl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mojkvnis.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2gfykzyik.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ygmliofx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hcdwwkwg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2evtszdzo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2spllqgxo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2aigpsejt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2lmrepteo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mwazkixe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cmtqyvcg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cauobtxp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zrmxtggp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2emqzjrgc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aqsozyju.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bnfoclgq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vvawerkv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2otpbbhjy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hfxdihnx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vvkayylo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cwctfdru.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2oxuuantr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2kmkorxwm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2akhckcgj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2kuojyvks.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2tlwnagra.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jszavsmu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2bzxwhidr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2guhnkndq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jwzdylrk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gvmcjovm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pvmzwuio.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2cfnuekvv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2knisbesi.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ltiiqbxs.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2exmhlkzs.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2amvhsvyg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vlnljkpr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2wxifsadu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2gaebfqvq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2szbcwhbz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2iaawipub.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iapzvchj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kxsqfsak.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ycjmnkxu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pocidekr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eycjavxy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ijgyshka.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2irgwvgol.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2xybhpcjh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wtgfdjeu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wcgehsnm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qyhcyily.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ticpysqv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rieqrvoe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ocwpnxbd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wgibkwmp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pxwdarou.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2joxvvtfi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ddpderqe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2przhvwtg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2qsmtwjkq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2stomuedd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2uzniktae.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2lqvogtyq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2yhsrwquf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mdswaltq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2naiubpzj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rwpevaxw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cmipgbqo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ksaqysxt.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ywywlyah.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2vanswqvm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ylolhvdt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2guqccvfw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jwgbqzss.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2hdwqlhna.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wqsbrtnx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iycrnohd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2aztmcjwr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2xodbgjih.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ktpuswjo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rqerkipg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ymxdsxvt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2yfirubnl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2joooqwss.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2iphsjgbr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bwpxcayi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mexyyoyt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2epfkhpjv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qmvwpdfq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2glsjitnr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxqdfeyb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2szoqzwzr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2kdlamwkz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ukfnazav.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2byoxtert.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wmwvskwx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2pigyrwxf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2uzpqezbh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fopuhrmk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cdtztcnx.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zelvxnmc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2tzqfqxsk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mpiequbf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2xvbozyzw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2riaxipoz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2nphzkdvw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hdlkagzt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xpwecqfj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iculaowm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pcfyxbyb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2yujjjcdp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2afuaoueb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xgqdcdjd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2brptrrsn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qcqpjrsa.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2emwsvvrp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2umeplatx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jxatxyce.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2tgsznlta.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rxlcbbns.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zpcqfidt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2immrnulz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vnnydzsh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2aiixlijx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fknxpsif.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2shvrtfjt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2lpdbvwqy.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ukzrltkr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dnlmpdfi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eipcrotk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2mzauuakw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ejbgiwjt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2gljogbeu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vlcpyxho.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2excrjnvt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2mvmscnhh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vxzyagge.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2kuykwhdj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2cjetmlqq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qsrvgxus.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2fohgjbbe.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2gmxjwzca.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qufvvogn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2skgkoven.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ofvnaomg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2scyduwcr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2zqtwwsrx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2rfqdpdfx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jqsavsij.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ngtzeqsv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ijjxyvyo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pxhfboul.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xxjnwddc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sovcsdhr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2urbpknyq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zpphnzzt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bsttoeij.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2apvcqdxc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2avyqogeg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2dbqfbceo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2npjujpkm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ajrvwchh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2josaehpy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2cjvfuobd.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2nyhxnzor.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yqvklahp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2pwhmwczl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2cnidudfu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2duugkive.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xqcilqrv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2mjnvutbt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2efjyilte.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fauxflgj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2zvexxfta.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yjqpkabp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mavgmcva.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2bffzxdca.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2rrwoovjj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ipzzyrji.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vfuhujcg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ioauobvg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2suanfkrq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2vxygoqqp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ioilbbfz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bsoojeer.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jwznzzsq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2dxykshfk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ezodxzsp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2quembjiy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2afrikkqh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qvqmprzu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yfydnggs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2vhgnrbab.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2mwfyqjib.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nwryyxzj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vaodbvoq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2thapbzos.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tbbsyunu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2weeldlii.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2buyldejv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2oaiazmhc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2pombjkmi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hhkcyxvj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hvrgheis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2briwoghz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2kuyjkrui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcqbqbfo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ghoqvwmk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2kadozmqv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2twixlvjg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ftjwlmvp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jbueqteu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2njtvmpxw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2axeeitxg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nztrvhmo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hyrkcrli.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ndmvxxfr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pcnqarss.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xwwovtrq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iwhmexsp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ufgqekxu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2aiiihsne.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2nmycdqir.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2howvpvsc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vseaihki.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2exhnfqif.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2jsnsgtqx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ryemenhx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ueponybc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lwqnjfuv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qfyucagj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ldzgtmsv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xjwwsvol.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2beibutxc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2fzpfjtea.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gkpvzaco.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2nwykzczw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2rxwfliga.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aklgvsni.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2izxxzjbp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2sunwlwyn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jxmwddgg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kcyubgrh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2iyumgzny.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2veamythz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ompyqtmi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2taksqevl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2pkextqpm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yerbrjdv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2bkiytwuc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2sxmyomel.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jtahiabx.html


<!-- 参考信息 -->