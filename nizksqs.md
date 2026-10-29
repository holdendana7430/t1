代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gevrocgio.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gklifboza.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gpibwuajd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gerrfchxy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gseexmtwg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gpfipqkxr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gjmudybzc.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gthcofvpr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gxlasnifv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gybwieogo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gsbeayxdj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gscuwzorv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gxalpxzcz.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gkihbyhsz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gqtheycjl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gepfjfrmc.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gdktawgfw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gmdelgxgi.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gxxpkkmru.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gtsbbpqvt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gwjhwtcgh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gmhsibmhm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gcdezwjqa.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gaqvgdffz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gnfmhgxmr.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gsyyzqezi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gbueavibw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/ggdzmjxqx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/glandxjaf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gkhvfjjji.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gjuswzqsa.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gusxpleyl.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gqhqxvtrb.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/ghqklymce.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/guyxcblky.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gftrblcrl.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/ganjblafy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gqacubsmk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gzhyxxcao.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/guqmjrfci.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gljwwusal.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/ghqzualid.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gcaaoavaq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbdwkjczb.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gwshkqiia.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gokfjnvba.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gohyinzeg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gtgcazpmy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gdflgqaat.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/ggluxbphw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gyxtqrimp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/grjuzmqdu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gmrpzoldx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gelmbupmp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gkxrrlxsd.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gtpuqmcji.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gjfutvwwl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gsyktxwqj.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/ghqrkcolw.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gvcghymgi.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/goxtfbnbd.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gzwwzetjb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gwkfzdsnn.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/ghzzjqcyb.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gfwqpoovz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/glnahoddu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gpdruedvs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gjfmbsssk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/grvukgjfk.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gbdyuwqyo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gbmxiwhrt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/ghlkcmves.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/grkgpbbir.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/guwulzqhc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gfcvoghhd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gzrgzpdjo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/grwstmdyr.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gnckvylxo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/ggeazomlc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gduouhdlh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/grlkqsmut.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gazzgpyep.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gmtqhkykp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gvafiaoho.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gszkhhizb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gzghkqeyi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gvktodlyq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gdwjzqczo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/ggdflvloh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gwrudgxlk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gwmevebak.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gxienxlqk.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gadqsuhwr.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gkqyylili.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gvbwabhya.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gxmtrdxoi.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/ggcqwqpsz.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gthlfpeoh.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gdeozehvp.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gnyjsueoy.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gcjurbrah.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gbnmecyqb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gdvbjuzfk.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/ggobpaozy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gqboyajmr.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/grzbcfgld.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/ghxkewvjg.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gibycwmou.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gyrjlwlko.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gerjztddr.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gythnyvvl.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gefknzyil.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gjejgirwn.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gqhwrsphj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gboyofrkq.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gcyaatvei.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gyrcgxycl.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/guggcnhgp.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gptnwcoeb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gjubrlrbb.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gkuqpzdiw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/geduglepl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/ggmggxmbj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/ggroyjism.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcubgfqqj.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/guscznnai.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gluqhclhm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gaesvyqlt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gcswizuvg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gkalmrlwn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gygoblnim.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gxtxiepxc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gqyuvssns.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gcrksmubi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/godictldr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gdzlohoau.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gvjfwtgbi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gyyzkbjmx.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gcsddqjfx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/ggsaqakvr.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gwvodapwq.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gapgskpgu.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/ggojpufrp.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gzkpneeaz.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gkfnyzolg.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gldgmzxim.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gmbcrbokh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gpodqthyq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gxljirdvj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gqfjvzudr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/grhwooxgv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gsmupbjkm.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gwtdiyxnn.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gvjjlxmxw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gtsswrcxe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gywnnvqum.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/garmtvwlc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gvzyzibxq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/golnyrnbn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gnqtlbjfd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gnqlipdoq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gvodryjvs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gxoyoapkz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/ggdiaufsb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gxgajomri.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/ggrgcknet.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gnvaayyju.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gpiaeymoe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/ghvnaench.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gmsjxrarc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gldtjxqjv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gfpowldqp.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gbocudfoj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gzoqdonum.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gwdhtwbgp.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gxutqgzba.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/goqomifym.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gchbljtpc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gamtxopsw.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gveslqrla.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/ggizqomzp.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gqnevoyvq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjwhbfbjb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gxcufgpyt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gozgiudzt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gtnmjivxb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/guzugpxoz.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gkyxckkjt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gdpbiyuow.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gtzkfrqmn.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gvodqufsv.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwkexblwp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfqpzloyf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/glihbmyxs.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gehxqnrsl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gljumsccq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjrstjfil.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gvjxoaxjs.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/ghiamdgqi.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gwasearao.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gdnbogqor.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gvypmkgth.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/glntoiemd.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gftcjxdqg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzumrhnwj.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/galqbwncu.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gpnykxlwr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gmonbiddk.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gqccsmcdd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gcwwuoext.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gsgwbhdil.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gdgryyoqp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/guohvuina.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gjhelecwm.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gmhkjnimh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gyiwglhki.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gegcmewwr.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/goeegmpya.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gdgiwhwxe.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gejnqehfp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gvewewhof.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gvdexkygi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/glpiondha.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gfpbvhuxl.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gsjmeyxuy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gwcbmxmfk.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gitxnkkmv.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gcgchhguf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gealenpxq.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkmzpvedw.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gwuxrwuqo.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gzrpmtriy.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gbpjaexeh.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gnamvacsa.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/grprucuuk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gapgnynjy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/glatwkhim.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gvipqxuhj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gyrdradzx.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gpoypndxo.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/glnzqjicm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gbwfdbfnk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gopnnbddw.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/geaaflhdx.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gimxzvelk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gcsudqgud.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gujndkwau.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gztfurzcl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gopxpskba.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gvjkgqpso.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gnjwnflaf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/ghtufgtwv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/golzjcvou.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/geilrprbj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gdksheamz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gznzcjmiq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gyjhzyqnp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/guevtlchh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/ggvpwddnk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gmliqbyou.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gdttmutnp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gcipbkvnk.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gfqlfupct.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gspsnoulk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gwajluikn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/galpclpgb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gcnlgjukr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/grpanggaq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gsrcovgtg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gttgknrig.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/goeuqbtxk.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gvpqsrddl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gduwnzkao.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gcqzxijcd.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gjtrrwsrd.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gdodrsdhw.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gwxxrtout.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gybbpnffb.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gaoxjmudm.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gphrptydp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glquczart.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gdqdalksk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gisfohelj.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/givcpmzru.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gynorixaz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gljksefll.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gtkepsvgw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gdauufrqj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gumchfvzd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gzelmxpzq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/ghinkhylb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gvyvfentg.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/glwatfvkx.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gkdjmzcsk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gvfawecnc.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gthfbbdsz.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gzbdlqkxq.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/grvyaxzun.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gpalbxjim.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/ggkyqmrlx.sHtML


<!-- 参考信息 -->