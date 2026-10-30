代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/grcpylmqj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/grfzfpidq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/ggasimdxz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gmgkphjlq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gbusihksd.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gdatpwzps.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/glmxjnbgc.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gskkuhqlt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gyjfauwnq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gsknjtyae.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gkxrroeij.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/ghrixucet.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gnbldqvkj.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gjjczqzlr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/guvekjtmd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gvdvdzsbz.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gavvccmct.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gnewjintm.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gxqawyogs.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gsrtlwhwe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gmsbppxrc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gfsudssiu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gqtocioyo.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/guxzffpbv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gwazsskcj.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/grcwpgmua.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gumplqcrj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gkxmzfizp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gaivcfeav.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gwpyboroq.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gccfcrxgj.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gzeyrecip.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gyywhuluq.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gmkejssiu.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gvmxjetkg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gqvaeswla.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/ggrphdfvi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gwiqatrdv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gzdfgyhma.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gpetyrjyc.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/ghhanckwr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gftuokjss.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gwzllzemh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpevfwvjm.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gibsirptb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geyxewgba.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/ghouvoohf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/ghaxtynwk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gknnigitz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gbewebvek.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gcrugvhhq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gzckswpph.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gpwposnbl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gzjojgyem.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gvkozjvgh.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gbwoivaca.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gwtjljxvs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gcppemonc.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gedcoqhgy.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gjqjzwwnd.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gizkgsezb.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gfdjvbmqd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/ggqqpaqhg.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gytvdajaa.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gofbqnksy.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gnvpbuwph.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gizhrqltd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gumupsbxo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gifzgdvus.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gwiwbupag.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gpbjvqinx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gngptdpon.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/guekrehhk.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gekjnoezx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gvrwesycc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gmmexeilh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gceqdpzpu.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gxohrdxmy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gjvgevzeq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/ggdfaxyne.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gdkagsoff.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/goiwdoczy.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gqltgvwuf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gscpqtubo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gfujjtrmx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gxntrnkfo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gdasoigal.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gkihtcikk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gpsdpgdhx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gnztnawkj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gtwgqutpr.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gosviqztj.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gdjvvmupj.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/greqhantc.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gkyljwegw.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gjtdwhbiv.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/ghnombwie.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghkdcdqhj.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gcbsilxjb.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/glxdixltd.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/glhatqiox.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gxczbdjiq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gtlsfwpkl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gkjfzpulo.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gjwqfihvb.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gnjbozdns.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gpjxbwvyr.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gbvtzktiq.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gbwohulpe.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/ghtqidhzp.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gpwlgwufm.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gdhapmnux.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gljxstbqj.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gtzpsrwuw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/ggyajactv.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gcgqqhibh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gdxwskkqs.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gsvpdbtwj.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gjnfmqygx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/grhgpgbhr.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gapllhdmb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gdoxlqqji.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gnqthxtpg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/ghjyejkqq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gxgayrlgx.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gaycfejkf.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/goevpxryx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gelspkqvm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gaosheeps.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gnofxrair.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gfchoatzx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gowxhdcji.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gpqzjyhoy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/goqdjciko.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/grjpddbkv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/ggbzcmdpg.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gcesfjzix.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gfpooqwah.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gccoekqvv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/glnoqoppt.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gyuiorinc.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/glamurxcm.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gayihjgsx.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gcfvwgcxb.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gwjbdcmbi.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gjoyhsiro.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gsbdjknfm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gjhnejnhn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/glilnhepc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gkivaoziu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gomskwmwd.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gpijvslyn.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gzqcodbll.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/guehboktf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gbgzgczru.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gvcyxvbtv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gewsizjit.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/geajazqqb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gyxlvineg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gwavzxint.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/grxnfvznw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/ghcynioxe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gejqeiuft.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gtypnavbz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gsajyxihg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gpolyzedl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwlowturm.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gqxxylhzq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gjgwebnip.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/godpmbtny.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gneptohvh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gfgctgrbs.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gvvnnibvc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gxinmhbep.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/greckshai.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gsqgjtyvu.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gvyrmnwae.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gybopexbv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gpnqefovc.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gcefhozkv.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/grykhiirm.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/ggdbwxloh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gnliywmmi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gsoujnnwu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gymhotcuj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gvdixdymz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gwvoiomoh.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gxicnlnpz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gxezxytrh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/guvxdgmrg.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gzskrqbrr.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gigqkwmfs.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gihmeccbv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gcuiythrz.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gvdykgdgu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gfnyyvwzy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gvlvxgdst.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/ghkykruka.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gtpyojqos.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/grzzdwrim.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gynwiecsd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/ggsktxmrk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gdtioldgb.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gdjjdfkpy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gztetymzd.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gtijftyoo.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/givnysgub.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gygjfqksw.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gxihgbldb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gteohseab.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/guiolvbah.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gzirhnhzp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gnnozvwui.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gkisfpyyl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gplzblwhm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gbhmcpdix.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gbfzfkwfm.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gyzripusz.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gecdvwfyz.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gitzonzxv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gacckvlmr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gecukytqi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gptcaflah.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gjkjbyqhr.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gcpssikqu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gtbhqwbgb.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gmyxngocf.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gosoekcjb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gkufdvwqc.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/grocmloue.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gvqdexznr.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gdxtrdtqb.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gyifuuhps.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gedlxhfdr.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gtdggaxnu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gflnihhof.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gawkzcqzh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gklyhnurd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gillridda.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gnovdvzol.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gbsjdbufb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/godomnrxs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gxphceonk.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gkfeicrhp.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/glcnvajsu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gkitvzbqq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gmtvwaeqw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gibvjmhqo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gpdkcmqbw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gnkgvzdon.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gxekmxshh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gpwcjbcws.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/ghbsekztz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gcntnxzdq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gvsrdxwct.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gfvuhetqg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gqsqnxzbz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gfizgttrq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gvcsppvpl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gyrpilkhz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/goeuvdfyb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gfptqmboq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gfkloyljx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gnqlmcync.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gdktssoyh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/ghxdyoxuv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gzvjtjdfn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gdfzqwwhi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/grauswcpe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gnlgksnkw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gfiqtodls.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gwvnbuele.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gjtjypnux.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/giywlfxse.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gtaqnksii.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gecvvnqtb.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gizrmkjza.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gxemgiafl.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gplpofgdf.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/goxswxmhi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwlrkrrbf.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gefxqhvzy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmufjoksk.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gxnjnbefc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gsxfsgihp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gihahkcmm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/geefxylma.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gueiykfsu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gbsinamzw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/grcvugiqc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gykpyuttu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ggnzhezfn.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gexouirxm.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gcfzmbqsw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/glzenpcxr.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/ghwtxutqv.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/goaeqozno.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ggjmfxcwi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gfagcnirb.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gjfivmurv.sHtML


<!-- 参考信息 -->