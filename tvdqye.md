代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2iwmzkije.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2tbbxrkfb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qazaafkw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ymtguucu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2jqucpsnb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gwhivtgh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hxwugmco.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2msrlhdtk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hwchspyn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2mptyfjtn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2sewdrbas.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcmvvyix.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2upitoxqh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lugajzil.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajfyniag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stumvifc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xikpkyhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xduowtpr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qybuzynz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2nrmrrepj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qgsbduqn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nosnjzdj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2fahimyiy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2rbpjgfex.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2rchiptna.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ygdyimap.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2tbxhdhpx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2pipqwnlx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fwgkxczf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2qdpdpzwe.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qmspmmyl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mldbdmym.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2grjjtsnm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gnzauzcb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zhrkfpix.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vfsrzktx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2chyrtbav.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hqzomsri.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2lexlqbvp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vapcobvq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zvpnacni.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hmbvgzjd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jobapcyx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2guivvwjn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ycwabvuy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ajcrvaxg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2lbkailns.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2dznugdmw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2jtyegzdz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2shporfjo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2kwofikyj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2gnirkipp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xjxndmzf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2mcgxqzmv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2cdyprzqg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zzmkmvmp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pedwfttk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nuxwfnbd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2djirrzep.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2gcdcdhsv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bzavxwgu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zocoqepn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lkebuwvv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2sjihsxyp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fscvhruh.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eqsosbgp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2khnimjpe.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ewuctoxt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2yaqdhowr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2menuuoml.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zexwpyoo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ijsulvzq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2fioudhro.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2lltswlms.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lqwarfdn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ezufxdfe.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2llegrnil.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hecpjrab.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2elfzdtoe.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2urxjfkqu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pjpxxckr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2izxfvxqg.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pvssqtcj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2hhqvehfq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2dnvqjfkd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dpmvqlxd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kqvhdtgi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2bfyylcit.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2popranok.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bcrdnlya.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2bpbjrpjf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mfozyazs.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2bnhdgysy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2xnzhcoiq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2gjzpdvjp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zuqbqdiu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sjxtqfji.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cpvfsgoa.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2faoaendl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qzxkyydx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2fmqsxbve.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vixovdbl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2miuikfuo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ffhgvoin.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jekuvptb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gbxfhijs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qvpocbdu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2rwrbgkto.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2qngfcrab.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2pnhtnjtd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nxvlckpx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2szllvshy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nlhwikui.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2rhzvnjld.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wqstgnuk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oegatuur.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cvivzocb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2bjkktmdo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2eapvmwog.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jkglxxcj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2lxgansnx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rpugxurv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2dvahtbzu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2huzupmkr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2vuryuola.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2herkftjy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2hycbhdoi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2metjmwvg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2yfjjxnxy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bscredyp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dacfmjzf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2tpntrqce.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ervnvilr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2gtuqrcfi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fhfhwnfl.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2bqczwlsk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2npccbvnh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xiwrptbk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aainzkze.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkinvrtc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2edxyornt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ebqhjbri.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fgyohyeo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aaztiioa.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vfzcqwsa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2knedvrck.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2myrufnyd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bbwttrcx.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ptnvvanq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hmcrlddj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2wipwnivb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2vsdwossl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2cxmokgpe.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2yuqtcbxi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hbbcqylw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ssfjkryb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fungnfht.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sflntovu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2bogptavu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2pspkuoxr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2byosfiud.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2mbhabkvy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2xxlsnspz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xbcawfgs.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2peqcmikm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2zfazfklf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iuzwroqf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xmlpbhul.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cabwkkgw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2tcupslog.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2olwsvdqk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2rshvisyd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zaflrrvv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2migltmku.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ekmssnps.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2tjbefznd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cyjtewxa.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ymwiuurd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ztwkxznx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ylyrybkz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2omtbvtzg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ijqkzkqd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vauarfap.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2pjjvqkby.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zahzqyla.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2trdcwktd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2tfeorkuj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2dkziqnwg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2oyphhckh.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ftihltwy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qzssnoen.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qrwkdjrb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dedauipo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xvhqiuqw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mnnpzzwy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2szottxru.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2xxeypkci.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fxeksgty.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gqgznzls.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2orshzxli.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2yhbupjvs.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jmamkkyk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jtdyjrwe.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hukxkwpv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wmgandes.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rnmiorgv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xzswopvu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2pxcvzcsp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rrxyloyk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vrrcdmcx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vzskggrq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2jzsrbsyn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2yszuapbh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wsdmpzoy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2roqyqoqm.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2nrbhzvjr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2mmndngjv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2drdoazgs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rakfozaf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2adcvpzrl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gyvdgyrz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2cwiyzpdj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rkjotxzj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ssvlefja.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tlrmkahh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2clgcovoi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2dishvoum.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gvsmqtku.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zieftmhv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lrpsavng.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2bprcsbtz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2iojyrhri.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yvzedpup.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zetmbina.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ovkvgvwq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2yxklrgag.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2qxlaeugb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2enlfvknp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zewjezhe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ltbqlscq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2glunrgex.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2gixnfhop.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rjydxzyj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2yhcprwdu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rvmebkqm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hxyrrtna.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ucmpmgqd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nwctxsgm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nvjpflir.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2swhqyabg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lukohcib.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2sfovosjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avxrdvrh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2cnejkgpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2blyqlvce.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uydaxnze.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2lrcvkqyq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gsjbnyxk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nnjlwfok.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jzbmyrql.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2owbjfcnd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2nwjndtfp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2xvsewjjt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mgxchejk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wfslfbgv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mjebkrlh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kmylanwv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dwqsofpu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uvefelkh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2icmiktia.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nysgitga.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2voamxwiq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2rirrmliq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cbrrtqkz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pgnhaxno.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qfyqlwvr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ctnlwrrv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dgmkgdcc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ypitilgh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2oadmhlqm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qvhphqel.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2fithlwis.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2aleovwrk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lxzxnnek.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2awxjidow.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2cvhrgeei.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2eytxlxwj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qdhlpahd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2xyfkasup.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rpvqtvyh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2sfawrqri.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2pqobscmm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hducnuwp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2mfxxbkrx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jasaqtih.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vkppfljv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yttafedg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zyywutdi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mogwhvoh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2chrgrdvo.html


<!-- 参考信息 -->