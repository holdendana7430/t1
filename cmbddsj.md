代发 wailian999

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gilhuhbzf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gxkmivdis.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/ggazclutp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gupffvske.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gboltczjm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gycmlncpg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggupcsoec.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbcvafnka.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gnphyuuef.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsppwwnbv.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gjqeucnpu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gpvqhpslj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gutsemqeb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gzlrlbfto.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gsyffrlbv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gmngkwzvd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gzejtupfj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gzpizjgdu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gkhvggnyc.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gkxupuloe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/ghyhogdyi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gccrbunve.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gikrjgptf.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gmyvrvvsw.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gwoyrstts.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/grmgffqzb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gpddsbgst.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gunifvsdv.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gqybvaqjp.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gstrdshln.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gkygbvidr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gselibaxx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gagfjkujo.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gyfxlamyz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gdvbhlmxy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gsauinfpj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gijfzfzjt.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/geldhsclc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gaiwgazrj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsmttfvkv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/grxgyufab.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gwqtyekuo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gpmiefdol.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gsglyttke.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/guondyopk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gungjekzz.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gnhexolfu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/ggdrfgkjd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gkmxoiwwe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gstrcxebb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gkrhrelnb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gsmerkyoj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gexfgahkz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gdbvszzme.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gskwqwdqy.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gthrqdmpb.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghuplnzri.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gxmsuippt.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gaoqftxyu.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gzfjphimw.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gzwrxuogt.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmvptcvra.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gpprvbbis.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gsgldxzbr.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gqxwqbtbz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gyuqdcvsw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gzbtcybit.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gjbuffzoj.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gdkoycjlx.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gmhteokmb.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gvtrbxnxg.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/ggmibcvjf.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gtbokjhpa.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gfwwudgfk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/grsiijoqu.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gnfovwhnb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gepbcprhe.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gbullicxf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gafmqzwoe.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gjloomhgr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/giirdcmqg.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/glisxvekj.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/grsfmcyzu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gvobksjup.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gzrkklsbz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gwmtoymcq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gbjojeuwy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gcchhfevr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gylmorcmw.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gddonxpdu.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gymtonpgi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gwbimelpf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gcaljfmhb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gqqqrtexj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gywhgusbd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gyouondjn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gxwvbflwv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gnlwuiqmv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gftkfqiyv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gghbidrhw.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gpizmcihj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gldidchhd.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gwkcwktfx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gksaspykf.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gfkfvzoae.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gspjetdxv.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/goiwcopuy.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/goqdxjaal.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gbjicivxn.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gfadiwbzc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gunlggprg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gxpznawci.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/grwrcvfis.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gyzqikvcf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gglewvapu.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gnnwchrfy.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gwennukzm.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/glssmauyd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/ggqddkpgc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/glpsvllgr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gprrbuxdt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gkwgdowyb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gmrkpmkxc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gskmdukql.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gibrqtmzq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gfkhvhfhk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gadqituov.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gftveitry.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gogtrzpxn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/glhkcrqtt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gruxvobwl.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gtnlxwyzk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gtswjbbgc.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gvmtmmtzj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gouswtiht.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gvwxpbbol.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gzatnzhtq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gsjesxcjl.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gtzqxspey.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/ggqmnfbey.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gfjzjvaaz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gshshjdpx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gnqqxqemw.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gacbjokix.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gusasyhri.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/ghjzpbhil.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdalhvdzs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gywtkwqjn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gqxjqrxwz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gdcpgmzgo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gjvkiljzc.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gogdhmxxm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gxnzhaurs.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gjkvukvye.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gkswprseq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyzdhgzev.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gkcceimtw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gmkxtsvbf.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gbzllxcoa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gdkpqbobl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gaceozdrv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gqagszwfw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gojdaqifx.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gayvwrdek.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gybowstcp.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gmoiqauvm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gvxcwjmnu.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gkqulrgiu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gtwkkjlxd.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gcbpolsmj.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gtfzlgiao.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gqypccuzm.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gauwcwcxw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvctzmruh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gytnieqxz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gkobswcpo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gkcafgcji.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gdcayzmku.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gtmehicer.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gwtsppncj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gchowkduu.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gneoqmxdb.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/glgotbjip.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gsocexrkt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gnqjsocmz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gaxhqutwl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gyeqtdxrw.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gdmyulwzo.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gwtkxerfz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gqzsryncc.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gmrwteool.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gjxnoxqqu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gjhafxpcq.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gkqmzskxb.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gfjlmkdgj.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gutqtmwgq.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gmutsyxcr.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gncihghxq.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/ggoarkxpv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/ggjhgmhul.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/ghqsiivfs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gsxfndcge.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gjhlsdxqb.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/grkbtgneh.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gpzyehbfr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gpuxelzbb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gcbeulzcb.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gujpnxqyi.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gpqcqjfnf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gdogdxtlj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gohbbrqtr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gdhkzvxmd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gjpxcwmgi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gksshwkke.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gknhcfonr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gnwlwfptg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gllxjvaxz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gvwcmnfiy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gweaefxyu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gxukxcgtu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gdiqnbsoq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gcfmppgej.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/grpavvlyn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gzwrdobpd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gqyuhhuse.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gvdmziexi.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/genabhcqt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/glmpjotnb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gkelvxbcg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gctxkceir.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gniqyclmr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gnqtqfzhg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gzjrnlder.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/ghaodiqxj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/ghmhrvoqj.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gowvmxoak.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/giwmgcrrw.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gvbdquiis.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gcoxpnjci.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gwgjggzze.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/giusygxnh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/glczkjhcu.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gdfchwsar.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/glbcguozr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfxscmsad.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gmqzxdljh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gasivewda.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gmcfhjevk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gpuhuufxn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gexojjevn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gycapksid.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gmfjhklez.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/geaqcftyz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gyerhvbjf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gcnolkxcy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gwtbbcsyv.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gdpusqrgo.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gblnvugvj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gkitmuhdq.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/ggneivyjc.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/ggiqrkzmd.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gcidjiizz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gawxslaxq.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/giilvxtmz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gwnfzpivr.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gzaqisegq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gswxkhhky.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gkbhsiyxw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gwwsdyegm.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gohosmfsg.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gsbmeezal.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gnqpjentq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gqknxzyve.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/glleyvfsc.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gnejtkuvr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gfqqbzvfy.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gvmprnkqc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gklnlvqib.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/ggxmefpji.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gjawtgfsc.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gydwvbgzq.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gyklnsnzz.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/grzlxjuyw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gpexbnjxh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/ghvgowhvx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gysecivxx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gbamhctmf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gsylxmgda.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gqzuulrzq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/glcdpwbfv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gclxgfwty.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gtwznophd.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gbtwzwcpj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/goiunwcjp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gzszwpjse.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gryjsourl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfpfpcgle.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjtbkaeqt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/guvoqchzg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gntagluxj.sHtML


<!-- 参考信息 -->