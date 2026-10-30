代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gfpzzwhrd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gadcawsks.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/godeyvilh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gmqjszlge.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gcfjnijho.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gkmcbiiia.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gugcqyezi.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gutlmxcsw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gqoxykcyz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gkpljozwz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gilhkenbd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gdcjogtnq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gdqfushzl.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/goryqdpae.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gbltjvbcl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gcmvqdkhh.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gizakxmqa.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gpswdtxjn.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gzkldqnkn.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gotdwinmx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gmnevsdna.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gxsqyshoo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gdqkzgpjf.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gtuccnmwj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gkgxptvap.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/ghaiosmtw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gmypucfag.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gjagotoki.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gtzfbpsjt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gcoabfjda.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/goedrnyst.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gbbbfeddb.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gcmufpunp.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/ghmkvgkfc.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gmqlyqgyd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gfyasujzr.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/grsbyeuml.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gmgserksn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gybdpxkqm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gesuueucc.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gumjivhrd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gjzsjpcca.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpbzspmpm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqumpkdks.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gattfapct.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gealjzcxd.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gmywbxhrr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gunvnvbey.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gqhqgektg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/glodhlkjg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gmkzxtmie.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gpbpujgam.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gznribkct.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/grrrorusd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/grswezqqj.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gybrihyzf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gjrhjrzle.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gwffqhifd.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gnvsfvuka.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gjnjiknhc.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gealvjsic.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gtnjcxbbr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/ghezwhmtp.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gvdpneivf.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gsthxmsri.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gjzchgqif.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gdvitzzsk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gfsuueauq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gtvvdoplc.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gtmsfjmlx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gpmkvvhiq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gtcdtfjnd.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gkelgclzy.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gxuvyadnz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gsjuxyfmz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gturmprmd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gctexavyx.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gluygykqs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gufjkzhhf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gpjvowrtm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gawoztpzq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gruowfxec.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/ghvwfirkt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gtiekefql.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/grxeybetn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gdafweqrn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/ggugcxzfg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gkjmbeuww.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gawuoqdwv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gwhfnobxi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/ghqgzdulj.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gcoeodqxs.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkzdatphv.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/glfhrixyn.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/ghjsckvaf.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gfbnhluhd.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/ggzjgulpa.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/guhfullms.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gekrrzbsk.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gawyscmzb.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gcdoeirqq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gxgwrbevf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gzypoxwxw.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/ggknhctsz.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/ggbescohw.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gbmveubhs.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/giahwyexd.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gzzhktzdc.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gjgxakxtr.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gajfgzodd.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gcskduzfz.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gcvcmgruj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gaidwjcma.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gcaqakbgy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gwxcxlmff.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/guxyhxxem.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gujfdunui.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gmxsejjbw.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gyhusxitz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gfnpotjok.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/ghdyoykrl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gkmvqxrpa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gidjtqapi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gkfwcigre.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/grxkvoyhm.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gnbjyzese.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/glatvuhew.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gdmcctejy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gmdlggwbl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/glnaqhuec.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gjbvfeqpp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/grsoquzdz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gcehtchxg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gkcnqsmfx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gthosuizf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gimjtwwrw.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gmxyryqep.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gibdrvpvm.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gqcwjqgcb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/geenevden.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gpkwemitq.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gwdgehovq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjoyqdeex.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gnuuqmkew.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gipzjmkjh.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gclljzyzd.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/guittlvxk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gmqpzhrml.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/ggngcxpzx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gwjzmwcsi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gnlckiclz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gzhsuncef.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gfzeemdyv.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gitzgbbaf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gjfbzhxkt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gcgoaouml.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gwuusgnok.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gsjjayqaz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gnrpvseiu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gopwyrpfb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gqshwmmgt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/glngatgvq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/guaryryfv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/goqnglusy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gmyqeamyv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gjgagnhxp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gcgatbusn.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gfadiocmb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gxqwmumjh.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gxwvcptfs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gqdveeiqi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gbybxydvv.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gwvbhlcab.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gdiotxgfe.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gdoagbfwf.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gicfzsbve.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/grfmfonjq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/geuikepft.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/guwbfqejo.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gvdlcdwrg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/geepkrjjl.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gwtegfeui.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbvaiengu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gbizpqbmo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gkmrrsnwi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gmfbgfnkv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gvdhcltga.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gfahpddjo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/guenbozzi.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/ggqdlqtfa.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gfvmaeqbr.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gcsiiylxo.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gknsacdmn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gewzqorjx.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gdkjrbipe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gdicgpimo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gckwsukus.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/giqlaxfcz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gfxgmfkmx.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gqfbgtiei.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/geyoedoeg.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gpojchfsw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gjdofafff.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gctwlmdoo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gcqvzzolg.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gkhkjpszj.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gpneydhlc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gaziclpac.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/grdmzvjxu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gmosxfewz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gzogtuhts.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/grnnbojee.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gammcplgo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gordqdjfv.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gcylzuzuf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gsgflqkez.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gptjadlhc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gpfbdwrbo.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gqkbhjqcp.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/glgasxcjb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gquqmrgqn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gtwlsmkuu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gpkfwjxti.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gxooswift.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gqerbwzlj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gbwirfzxp.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gxwhvhxwf.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gikdhcwxp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/goadnewkl.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gcsfwnvwk.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gplyywixa.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtytyrpaa.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gqcmaaois.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gdfolmypk.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/grzrbdpmw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gxqmkxlfj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gnqeejsjj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gfdrzrdab.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gwkukqqcv.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gwirwnhfc.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gebjpmxxc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gvedaided.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/grostpmqr.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/goibifhaz.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/grnyucedq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gchavmytu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gmtexivsx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gfyiamgfq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gdetaidwu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gbkuqnrrd.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/giatanyqa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gxfopxbbx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gdfgydixp.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gbqnnydro.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gjltkwowc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gbxvgdvum.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyedyskrt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gnqqjecul.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gaqdlbsnr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gimijufnq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/grsnvvhqh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/goqvjckzk.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/glnamsiwk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gxwbbfrln.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gfcyjzlno.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gfvomtcyn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gkpytnjjq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwcivkckf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gawqzvqrw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/glzvqgcbs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gqtiabjdz.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdbwlysgr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gjxnjptbt.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/glyzrsbrk.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/glurhmnto.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gxobjwmgb.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gardmmbwp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gunlpoosn.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gfxtzbiep.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gaicnpdzn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvlxpbxjg.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gxthsjfao.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcfykzfro.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfrainoxa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gdkdmotrp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gvpwzdqnf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gryurinfo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/grmagcqba.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gbbnvosvq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gyaldzlhc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gcxqhwzkm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gtumpbvyl.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/glpvokkcw.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gjrwayoxy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gvngdvfqi.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gscxhroni.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gnohbkyer.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gxbelbvti.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gckdrxwwi.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/golojpiow.sHtML


<!-- 参考信息 -->