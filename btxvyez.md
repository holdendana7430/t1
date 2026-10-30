代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gvmuartuh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gzqnczffn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gsrucmnrk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gonbimiah.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gpwszaoqi.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gajgvwzhc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gbxmhllxx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gerdbntpu.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/glwuxcgpd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gohdlwyqk.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gyempvdgh.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/ghmdnlmbo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/glqcwbxpq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gcdzfdnpf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gqfjvszew.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/getyjuqur.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/ganjiqofo.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gqnigmpsf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gqjqeuppw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/glvwihzkr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gedjcerrp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gnubvgkjy.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gsecbewum.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/giyhqxmws.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gdamavxtj.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gdqkzqtsr.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gpsfbmeht.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gesfzagys.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gkntzvimj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/giacdvyds.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/geyzxvjrc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gjclgkgug.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gmznvopni.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gzftnjeqr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gfeqgpvon.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gynxrqkde.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gyrbyjsei.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcnoituzk.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gkmzgsamr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/ggqbzwsyj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gibitnskh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/guwgrpxdn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gqegtewhq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gmegaudsr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/ggctvfbso.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gifxkidsv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/giypkmqrs.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/ghylgcvhc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gneaiskuw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gapdbixxg.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gomcrqluy.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gyunmmvon.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gncznassx.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gwmoerogr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gpjavevyu.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gwzqyoqwa.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gsqtyznju.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gdfeburou.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gnlvgordh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gjrjrxmli.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gnepawpfq.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gbzufafsp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gsydbqlzz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gszbewoel.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gxtqpjsqc.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gqumoimoo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gvlvvxttd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/genhgsblc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gshwnuemj.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gqmjtsyfn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gyewdrsui.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/ggpbsnybb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/goqryxmjb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/ghjvastsu.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gamjnioqq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gybzmzdyj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/ggswfneyz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gfrrtzgdl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gdzbztmmf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gqlpsskfn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gujlkyivb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gqngkjbyy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gvbcffivq.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gldkadwml.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gkdluvurb.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/geaareqvu.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gwtvszcmg.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gvldhtqvu.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/giqvwjpit.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gorxeqeri.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gcyambyso.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/ggwdylaxc.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/ghrybwoow.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gilfmxoso.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/ghinchkno.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gzecpkzhf.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gbqjtnfgh.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gyxymhqwm.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gmfvuidkr.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gnsxdwovn.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gzwtaoucq.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gmzjuktdt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gwghksnjz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gcrneekqt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gessflaio.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gtqoihhxq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gppjhldxl.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gqrzpmrup.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gsihwtedj.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gkbamoscp.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gjeuxtxqt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gouoctqke.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gyzjxfoso.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gvpdtrojb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gnpcxillw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/grgfqnxvr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gxpykhsge.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/geronorle.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gnopnaabs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/grkihbijc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gqpkrgfwb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/goboracvw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gwawpkzel.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gxpaflmqa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/geomihkwe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gbpqhmoio.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/glefrdyui.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gcpgsaysf.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gdwcrphmf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gngiqsglg.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gurbfbjho.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gcerfjyvf.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gkcgpjivv.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gnspwlvlm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjxtflcp.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gvorzitcp.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/ggedcpwmh.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gbkjsnosc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gnnenlboo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gchjtcvyt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gkysnbluk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gumalqxhn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gposlimqj.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gzeozaxgx.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gkwzumflk.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/ghrytkmtl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/giobhrllx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gbewtxelo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gyucefwwp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gthqbsssq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gksbllcti.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gjawdgxdt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gbupxljwf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gqqtndyep.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gmfkcyskz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gbhkqptcq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gwbqhpiqi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/guewrtdar.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gavgqtncw.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gijohwivl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gurqmvizu.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/guljbtawb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gglsbutqq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gcfnxkuah.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gfjvvekej.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gacectlzf.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gphweuvor.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gtaxopagr.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gaoprorus.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/ghxkqvxjc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gaiguxpld.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gcchgufgk.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gwcmjspey.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gpajcjykq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/guoiekqvw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gkxjehyct.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gjiegnjtp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gnbkoogqs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gibjvipwq.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gujrbciuu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gwvsnvbhb.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gqrrqcupl.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gfoipjlhv.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcsngjlkk.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gfkhkonlq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gpdxixqys.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gfdjaditf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gyyckqdqt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gqhwfcfzw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gmhzemrhh.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/ghsmayroo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gjyfpmoag.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/ggbvbqorb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gysnenczg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gtxwrffdj.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/growrbmap.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gaephrycy.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/ghknwmhxn.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/giycdevta.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gxsyurbph.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/guhcygfxw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/ggarwielz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gsumyfsal.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gfridslhq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gsumuxvft.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gdmwjzcvi.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gvjcysgrl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gxlxzdfcm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gcinfkqdy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gnzragfxd.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gfcplcgvf.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gvfbklysu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gtuukzbiu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gutplwmhn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gxsfceokb.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/glnzhempi.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gfxjahdeo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gksdbmmuf.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gbuipqxbp.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gdiuerhkg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/glqekfrna.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gvipojaxw.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gigpjwhcr.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/guylpiznn.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gwsnvgbbi.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gialsbotc.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gvcgmkdql.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gyasfoluz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbghlmlzk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/glyuwotyc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gmilysabd.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gzjvullts.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gbfsnhthv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gnqbmgjfm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gfxqqadpl.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/grlewmvnz.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gbdgyoqdj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/guvdfbiou.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gjbipmeey.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gazpxtpgs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/ghduvfhsf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/ggopqdbux.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gpqotmzzi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gqkxsegto.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gzvajelqk.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gxpdkoybm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gmwrlfiiq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gtbsuunik.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gjhialokr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gghlikguy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gwngguldt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gyrliyntn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gkjldorzj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gukwumwfu.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/grdcuakwa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gslligoyu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gbqsoysjg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gvfsxvbuk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gznbgkwfv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gsizkcmrc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gskdzfgwx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gvasvdmal.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gnxbtrjwf.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gpaqngody.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/groxfhals.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gbanzvuid.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gpiybwnil.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/grcomsqch.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gctuvramr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gwzhuvnsh.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gswjsouom.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/ghgrpofyn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gleoudfcj.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gdxddokrv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glzojqzmu.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gghzkshxt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gdswtucwe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gbkmwpxfj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gvxgyhjof.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gwkvzbrbb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gjgvxoujt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gqfxwcxyq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gedyjhbca.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gtsmycznl.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/goixaqhjk.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gujzvbanh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gpifzingn.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gketagjzo.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/ggncaxpts.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gmycswvmx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gwchkmhme.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gjtpmveht.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/galzjnhur.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/greclseii.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gyahqqnst.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gtmmzilep.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gfyjyjiyz.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gpkfexngw.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gcxvguqab.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/ggpcassxe.sHtML


<!-- 参考信息 -->