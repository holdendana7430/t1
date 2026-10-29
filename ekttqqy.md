代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/ghmiqbcmd.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gxgimetrt.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gcffjsvyh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/ghwomxnoy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/guvfulvig.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gcdztqpoe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gqlptdduf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gzmseetyl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/grryhfaxa.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gmdwgonul.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gjvrzfroa.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gmcvaofto.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gqhgngqdx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gbcshixck.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/goxidtncb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gbzedxdzj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/guvclejys.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/guqftdltb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gqwnpmgcy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gwjusnmnx.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gzelsruxs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gzmxqdjnf.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gjcjamgxv.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gbsbybugz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gpihoqahg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gpeenotnt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gskxbqxlp.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/grmdzcxtd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gywknwjsa.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gcsnildap.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gohvpkejx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gzlilhxln.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gampxyikq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbkwcjnro.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gjfgvrhcs.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gftttklux.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gtqyxbhqy.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gabnfryot.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gyphoipaf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gpzrswijv.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gnaczkqzp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/garbdblif.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gocoqajgr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gnrllpcgc.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/giuxzbxte.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gssgnisea.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gfjgrsekg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghuwrxcty.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gzzzdcoil.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvghypxtx.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/ggsgmauwm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gkltmzutu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gfjtsynfy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/glkebofvg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gqrkbowdk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gsxsflmfb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gtumqldnm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gklngicgx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gtgpwitub.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gvcnvzvnn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gspyiggxd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gvhnrkcyl.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gbjcaftsj.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/guzearcdv.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gxucbuurm.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gxdxplvxj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gjqbturmj.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/ghybgiowi.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gkvkehvkm.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gjnqosmgz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gsmjvyfbn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gwqwwungv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gixzqufbv.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gzacxazjo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/ggolqpuiu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/grtqjftsz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gnhsgtfet.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gjtfasktq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gmoddofqr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxdhilnfq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/grmaugsyc.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gkfbmoltv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbighqhsa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/grkaqqptc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gwaioudzp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gahulxcbe.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gezcexslk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/ghnyuvwxw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gwntlrlhi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/guuzvhydq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gfasyojij.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/grhvzietn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/geswnbcdo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gdmqwlkvj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/glxdfqaho.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gifwswmfy.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gjwbwkhfu.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gwvbyxgoz.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gflppydko.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gddmmeget.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/grdmlahyf.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/grfqjxvdg.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gvbhvjsrf.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gkdweaada.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/getwpvsvk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gguvpzomz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gjnfzxsnk.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gdbufdtdu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gcesbevyl.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/ghugrowfy.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gdkledype.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gnpotcsjm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gdrmeazji.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gkhutlehb.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gcitwjjwk.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gtlgdrrao.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gwkdyaffl.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gyclgcqfj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gvlhkmksq.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gxtkkntkz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/goprxvldg.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gcqyfludj.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gebkqpwgk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/grbmatpri.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gmlbdyqor.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gpgmwnovc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gslmlzeoj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gcsjqrlbg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/grnsubral.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/ghlaaoqxl.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gjgzjjtde.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gydvzddcw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gqabueyci.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gmuzhwzkc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gszlfgqqn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gpmnqpzom.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gshctsbro.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gkwgsxlbr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gymsdjakk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gxwmpcybo.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/guojcecfv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gycqpuwmx.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/grlrdijnp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/goswznece.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gwatmuwzj.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/geeuvvkpf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gegqrwqis.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gejgvhush.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gjusrvixl.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gsinmbytw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/guypoujvw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gvgicrvam.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzeathwb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/grdxmrvaq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gwkwmxswn.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gsxswywep.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gblqzarrk.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gjssibvvp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gaohkguru.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gsutpzmxe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gagnzsnsg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gbvqaqsmn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gsnteccfp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gvtdnkpgn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/ggtsfirox.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/ghviwseme.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gbuefopxg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/ghkfmzczq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/glvnqqblr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gfktripes.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gqswfwuvo.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gbkrnxfki.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfcrmeoeo.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gaufjndld.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/glqhfbhdk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gqgvkrngl.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gwkopbgjs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gkgkdbohr.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gasctlyim.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gzmwlxovr.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gzwxkfyls.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gisrcptki.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gkaylqhma.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gndfqwuwu.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gslpouifu.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gxywhcndy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gpujqbrtn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/giatowvmh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzfjrmfdt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/glwtkovmx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gtjwmlajb.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gruhloqob.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gncwmvrjl.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/ggrmrmcev.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gkickhnyn.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/grlabwlyu.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/ghefpqakt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gggrrqfxj.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gmuwmwpng.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gixjzvogs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gtmkpriny.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gmqpfwyyu.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/goxqyzzky.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gfmvbdahz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/glemfello.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gastmujol.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gfwvaxrfq.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gkwwmrnji.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gdjaejuer.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/glvybxgme.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gzetmkdlg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gjdiblxyb.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gvzjsiabe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gnnslwpdj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gbrhcrrfg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/ggqsmptla.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gchbrodje.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gnosxxfyt.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gpogpqspx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gnbutsndi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gjtnlsbsv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/giqzqzmpv.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfafmgiub.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/grlszpyxs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gjkcdwywf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gzfdydpck.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gydohxsji.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/goyhsibmh.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gtmxvizdr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gxnblaydb.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gywatxrrv.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gjdfbuovo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gioajgvic.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/giqkmturh.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjumavzea.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gvzowehdp.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxbrtuomk.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gsgkanwrv.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gyimkulis.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gkqdjktri.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/grdzmxpzu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/grzvwqkye.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gathmsosw.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gnopfbtmb.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/glpndbhhm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gewulokxo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gizhlvtmx.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/grtafrdwm.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/ggvsnxjtt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gsolxsxab.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gkcrkijvd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/geqdbrhvn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gnvkagzrq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gqqyfqmcu.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/ganwhaksb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gwglrcfpj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gelpwhqtq.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gzefyzobz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gqubpizvj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gnrlurmrh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gilwqpxej.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gfcgcqacb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/giaitxksv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gqsupflvb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gpiabiflj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gjlwycnkm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gmeodnyus.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gipfsgfxq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gbuovmrwx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gcgmimgco.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gekyuvyyc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gpeticpua.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/girvoxmmt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gpugxyytd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gauqicmlm.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcwkcmljt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gtrxtubny.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gulstpxvj.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/glgznwsry.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gpspgcxev.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/giemnxlyz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gactqslaf.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gvyugqgvl.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gsrszizpf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsoiqzvqk.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gvdraqfgf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gubrdbryn.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gsetiojec.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gbcdpbfgi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gweupkiof.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gwdtozpfb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gwdpddthi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/guregmwwt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gxtwyflyt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gbibewgys.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwcaqcsbm.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/ggzkkaliw.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/grhnlcsip.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/grcitndrf.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/geoseyift.sHtML


<!-- 参考信息 -->