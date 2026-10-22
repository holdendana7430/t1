代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2iatspsur.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2eqevqrem.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2edgowwrv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rzfholmk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2acvjaqwf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2pnyatgkq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2glxusctu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2asgoqfgf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2aewafwco.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2nhxilyce.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2bymcmlin.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mskslqtf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2qfiwipdx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2orjldlum.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2vubvobad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajvraxpz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2hfkcvxmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywopbvos.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zejdeidg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2mdxbhtgb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ejnjfkog.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2afixznpt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2rmjxdomv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kxabbkqk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tfxslcbd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2tadvzsnd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2pzumpqed.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2uqhmhzvo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zxvvzpsv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2labsshtk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nwpgnuzk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ycmnmxzo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xgdwofhr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2bzihzwpv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2nnjsuwnc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2nzbznbnb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2lkrlxowc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2injduxbh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2obkpelqx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kjzfyrpi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ilptfaes.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2esdhvjbs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cvqadnbc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2pzuotogh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wodnibmi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zdzwtaxm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bnyaeusw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dcautrcr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2egcpjppy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2vjcvctxx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mjftsbga.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2wsyvycdu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2wjrnuztv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2rdvdcdfs.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vyivalip.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wlcovouc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bilxwwrt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gjdegpft.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ehwtmvfh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2fltrkqcw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kahjvbob.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2knkhgqtk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fwufffrd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dqvnrfva.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vwgjlgbz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2osiytapq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ueguieku.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pnlyqqcp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rfewelqo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pymrfepb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2xmmbutgw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ljfddlqy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2drrtgiqq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2aamjcwls.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rmtdvivh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fkdupsjf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rhzvsbzq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dzugdruf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2pxuqmbqx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ayochdsu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2olansofk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2djiejbqr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2onbhzzoa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kuciocxa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xoazhgax.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dskizvlj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jdlkqzap.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2xetnogta.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2kcyvbjlc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sxbjhdnk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2zavyzmes.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rjwdvkra.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gtligqzs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ubblkzhf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2gfbefidb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2qfkwcdyn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wxoibaae.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pdkjfirk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ryqlaqlp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2hsebfrss.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dtjzchic.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hblpkhqq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qvjuyski.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rktcrvxb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2eqkeaajm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2wopkxcji.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jvpvrzvc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ivtsjgyd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2bazkwpnd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2lrzezvsc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2gjvfvuvp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2dcuntpku.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zoqutexi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zmocrdxn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rzwtupuu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2lmasffhm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ldhfywch.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2uktuerkm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wwozohon.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xtweqrdf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tndutwvb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rsehmvse.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2bmqlqcyn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2utnqfvgb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifawimgd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2jwfflzfb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2idkazehl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2xoxvvjmr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wucybenl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fazockwv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bsdxxjvs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2nsmaawil.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2phiixhmw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ghaxecex.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jxkvkpjp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wgzlqmix.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vjdzvgkq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pvzvdinc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ezrwfvmi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2haopazrw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2erjtsvei.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kjhrsxcr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xkzlzvpt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jnlcaccn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2mmxczpbc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hkgnusul.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jtakwhnt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fzfilwwr.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jubcdaoq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ncidforo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2fcftzncr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2uzmilipg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2tdtctbth.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2anhwhsqe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2usydlsne.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rqsnfrop.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ubkntsnu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cxepgeaf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mpskovxq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rhdjxdvx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xeqgjmyg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2btdexasu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2haashwyo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kcxpdzmc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2atpslght.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vwcqtggu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dpgvxrhs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xmisnibo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mhieilqk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ojsonhft.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2nmfeplvt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2gwntmtpc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2lkpsxlvl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2tkrqijxa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2htemaxbf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2fwdtelfb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2indbquii.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2husogmlb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2horhemce.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2viictpci.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2qvephopa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2efphqmkf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ezqowtym.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2vtdwtazq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2johaebgu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qastdooj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2iajawbgg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2tiuversk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2kepnlnxe.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lxnhcpph.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fdcwhaik.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2oexsfikb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xylzwajp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jyfjbpht.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2djzgzdon.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2iaswyxsa.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2hhnqftzq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2fjczghjb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2lgybnamr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2vevwadfv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2cxwholsh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tstyjols.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yrgkvprv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hhdwkfjh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2smeasmdc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzpkkjiu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cqxsulax.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2mxnkvkcd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vkbewufs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2zkqiifrp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bcpfndcx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2lmvtnnam.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2dhvizcri.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gqzpovwc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ekslrapo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2nfrcjzcy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2kervtanc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2tfkwjxgt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qhccwqgy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2koubfvhv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tdmgngok.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hykkldjc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gmenebrd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2iyyjyzro.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ghvrvojt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2zyyoqfly.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pxhllrzk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2mhekaudz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kgrlpwey.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xjkqhled.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2nzxlkxcm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2bwqisofw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wmgishwg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2xlhuhsey.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2cvzcgiru.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2pwemxhkn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jlrdgcuw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qdtisbbt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2giyhndvv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rltzvusj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qfiyglye.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gowmnrhj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qszuaibp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jspxznyg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rhslwyks.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2axzlzvfp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2venlqkrl.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hazhblga.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kqrmlocm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2mssxltng.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hraiqeij.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2aqwstfvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzpouxnj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2afkldpkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bpkjiwnp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gowgwaib.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2kpplxvpg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2zcsbihku.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jjbbenij.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pbtbmhra.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xtpairfr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2hhzrakyp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2aotyqjlr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vpxhfkmh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sfmqrdus.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hleiwhmt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vpywklnl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nrqmtmqd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nowwrqrh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gcpuixac.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2hyhjeydc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vnjkkblk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vfgagsht.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dtnrgrco.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xevyeukc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uryigmiw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vegbcynh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mqogznmb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hkdhiuql.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rhoubjwm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2wqcopzex.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2jajviweu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2tiwvlvlr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mcikmote.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2cfqxdivk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wvetxriq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2sjmxdxku.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zqanzgib.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zhrlgdev.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2somvbgqj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ijvargjz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2nvcugcxm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2flthvkvp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2twddhygi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ocukraso.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jjswmtkl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tkyvinob.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kqaurwls.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yftdfdhx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tcuadjxv.html


<!-- 参考信息 -->