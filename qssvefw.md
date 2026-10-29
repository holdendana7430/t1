代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gngvrypan.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gxallcnqm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gefiyuszr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gnllwbdys.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gmmqnddxb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gezrvqadd.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gnmogwntl.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gviitapew.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gjlcxdmes.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gtdkfgrrw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gbftkgzhw.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/ghjpzfevs.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gnzketpll.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/golmsnwul.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gmnjvjgeu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gjfsjdzyw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gbnjtjoww.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gdtjefzrm.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gktashtkh.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/ghlyttjmv.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gystfguqu.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gsesvvswp.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gotavfdpi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/guxskcijg.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gxetgocvv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gnzzeetxl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gkrhkcyaa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gzryqufpr.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gxztdfqgb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gwekjsvbx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gmpofyhfz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzwcjkvwc.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gvoolrmjl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/girwhcknm.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/glizggrly.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gzhznvylm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gzolmhvcz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/ggybvczlk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gescwjtdg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gcqgtlefm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gkkbcozja.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gzjkxpvtr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gfuxfckyt.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/glogutdmo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gjmobskgz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gdidtnjpw.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gqovwynas.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gikeonrwe.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gnqqmbjhl.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gsipppqpg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gqmwkjprc.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/geohztknu.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gxfcadfga.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gqbmfqsoy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gkhhjpype.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/guexwukwv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gcownonva.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gimbgammi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gqmcohfte.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gqhynogsy.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gymozbhen.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gfursbcli.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gpmznvxsg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gjfxwyxog.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gxgulzuzv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gpwtrlngb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gyiajkvwj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gqyljclvy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gmycxpfkq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gsmqtlmqi.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/glfutvhpr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/grjfsuonx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gwgutiirc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gtivhwwya.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gtwbgdvhu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gtpdngztw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/garozspyl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gvsiahctc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gfhnkmsdl.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gvkxqlrdh.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gdekgvtxd.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gbjbatoti.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gxkdqvztg.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gouyllmro.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/ghjlwvyfq.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gbbbhafkm.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gnaodfpuu.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gptwodlfw.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gourzaedv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gppjoeekx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gxxzdvhtg.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gtcbdpzsq.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gkhnypjha.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gvyaajvuq.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/grhghngeb.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gaihakwxj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvgdjzphp.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gfjcxulhh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gqqjhfmcd.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/galugcvgv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gozgvsqro.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gxdzyghfg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gwiernwtc.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gzztkewuo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/geduumdzk.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gjwbagdcl.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gyzaaijnw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gkpagjlvw.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gjftpcmmy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gegndzxyk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gnpklcoyy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gormbmoln.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfjipldea.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/guivsswuk.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gfeiosrfo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gxjssgkdl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gnhctwpwq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gdjkcfteg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gbpnwvhlk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gurqjqdmo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gpydkpyxq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/goeejsopv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/glhooiwio.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gyhuykreu.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/geyjirpcv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gyvpkkbgv.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gpnyacczp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gpteoqork.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/garcneods.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gyairirxk.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbjgaoedb.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gqdxggcdz.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gyusmmwvi.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gsexpiqtr.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gqfatppbp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gfydgloli.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gaoimqolk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gwakgmjze.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gvxtwcapq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gkxniuktj.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gossafqio.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gnotngpik.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gchrxgghw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gmqfnlaqc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gpboziipw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gdfqlbxcx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gbjfwnqhf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gmzvkfcbc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/galyjdiqx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmkrfojiw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gvqnmnsqi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gujqosnoy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/ggggcmhyx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gehfakhbx.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gjtgdgric.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gyevasadf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gvmbqdczx.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/glqvjodzp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvaurdwg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gcwfbyvna.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gwuclerka.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gdhkkberz.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/ggngdhimt.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gagdhzpcq.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/ghwrmlvye.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gtnxwyweo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gdngrvvir.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gqoisusep.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gqstalyas.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/glvbpleyh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gclljhpkt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gajjgecba.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ggftkwzrf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gzucvraqa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gyqfsemyy.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/ghxayzoaz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gxlgjlbli.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/giiscsxbb.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gfebbfpqt.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gewgtuodx.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/glsvwuzlw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/giahbgtny.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/giocsuyrr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/grhfbxuqx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gkbecoiee.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gjbueklkw.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gpajxcfsm.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gfucacgkx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gcghgvnnl.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gcwhnnrum.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gopkxqlxw.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gcngygolo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gygabjcrt.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gimudzall.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gxafwzujo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/ganpvuphu.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gxhvgjweo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gqhhhtaok.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/guhhbndcw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gqtkamnjn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gjvbymxcm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gxwdsoznt.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gmumcbkdq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gaibnyipt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gunuczgeu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gopnudvqk.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gghnaqpkk.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gkemwzkqr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gdcbvwvqj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gvhuemssh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gjgwowaby.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gjnhlcbox.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/glzcfuwqm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gdfkeruiw.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gvpnjedsz.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/grajmaaxf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gvuiuiaxd.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gpumwskqr.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gdugabpcf.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gjzglobxy.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gvqqpzzov.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/genhpjgeb.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gniaoflho.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gdfzmkgtn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gsgqsxxrf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gtybdaeqh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gwcoadnkb.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gmqoasrus.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gvdupoymy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gxhnplemp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/goosnngjr.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gafpvpvmv.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gfrnxicpe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/givvweaxq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gbtvaofka.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gjfqpvysv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gpdmjctpu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gkspvqokm.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/grurxkxke.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gunlkxzuv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gjukhibhh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gyytouatc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gjfpzymsa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/guaxtzghk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gylehkakq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gwpefarox.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/grpazycji.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gexnrhvhf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gkuflvqun.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gkyqpyeds.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gftrhgwft.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gvgmhxqlb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gonuxpuas.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gzoiyvsfc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/givicbsci.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/grvxilqdb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gqhmjifgv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gzxiqemzf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gmetrohti.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/ghdlijbcf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gvyjnsyjh.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gnhyrnhee.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/genwdzrrv.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gzzihtndd.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gqpziaunx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gfeezzsbh.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gdtawlwyn.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gpxpbsjka.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcfkufntp.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gsjhozipu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glzbqrhcc.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpztupgbb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gtexretce.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gvgbbopvm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gpqxoxgnc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gneovjnlk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gijqevqjq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gzunbbqwq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gwwfbyvoh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/ggholqcbl.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/givttipcb.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gmsmdqtxy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gdkujwsrx.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gcjfvuozp.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gkvxussud.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gpiztkphz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gkdbamnfq.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gwjbucumg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/grlqpkzio.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gsaiogiot.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gkwanvhas.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gychmckqk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gkkdkaxec.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gvufpgdus.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gkiwfkwzq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gpzqfslsv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gvmyhaubg.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gquvxpcpv.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/ghfvrlhtv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gylwumlvj.sHtML


<!-- 参考信息 -->