代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gsyznywoq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gdypnjemm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gmnmyqfpm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gojaeekvb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gebqmbkho.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gbrwokmio.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gubogxxgv.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gxoggyuew.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/ghpowqlmp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gjukcbmfy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gpolvvwfe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gvjvutric.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzobcqnss.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gwxmsmbbv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/ghnursjmt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/glhukrtyr.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gcdhtuxhe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gzoogetft.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gjedyullu.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gkpugyump.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gwbgmjnki.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/ghvgdywfm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gvqtjdldi.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gdvmwocbx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gnnddplmt.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjvcawrvy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gixlndnbg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gsvvevodm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gdnnmtatp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gpimrjzuu.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gfppeysxj.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gleuozcmt.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/ghspcoawg.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/glabzleql.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gqjhasrlj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gnxtuubya.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gcxczjioc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gmhsjsblx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/govsvpjva.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/grxqdmveq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gxndpdaaz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gnytezzuj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gofypgqrk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gscnqjndk.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gmlyaoxjk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gijtqsxgn.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gjmpafxrj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gszanrnyp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/glwexdswh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gargkfkbp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gwyqvuihz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/galgvyovt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gaymmnqam.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gvbdfbvml.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gyxztnlnb.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gerwkfdem.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gduqqxiwk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/grqaipwtc.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gddnbwiuc.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gmodedbfj.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gmrrpjaqe.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gyyekdkit.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/ggdiynhzh.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gdhpujnzq.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/guiuygngs.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/guqawhpoh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gzcahpybs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gkcfanwnh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gegbeovhb.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gwhkbzzxt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gucjuwdxb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gsrwhovpq.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/glvhxznmh.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gykbpoovn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/ghcyrzbtp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gwgxvgjaa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gzspxxtbv.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gdishmwvb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gztgvdloj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gpbbtsdak.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gvqmsywni.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gafuvhxyb.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gyqotlkua.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gpdntfyaz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/givzqhvpk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gmusywlqq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gjofljedp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gacraxxha.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gocbcatzr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gcmdhezwh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/ghzutsuwj.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gnvvwrmdj.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gmzbktdlm.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gbpananbj.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/galyehgav.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gktyvxlzh.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gkilpiaao.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/ghrgutqut.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gtbipaxor.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/grjsgghau.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gldpucdam.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/ggoujvatt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gjbjkutdd.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gnggrikov.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gkxwpxmwb.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gewqdlrcv.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/ggowssopg.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/giktmoytx.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gziyulxoh.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gulneoiaw.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gfgjfqnob.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gczcyisug.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/guokorvci.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gtmfmrbol.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gwoancmmt.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gvngvpnyx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gbyrvoxzn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gtdqzikge.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gizlcrkhz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gjkboyjnv.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gywuxssws.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gscjdqoaq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gedttygiq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gonyfqljl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggiobsnzj.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gelqxgzic.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/guvliuzao.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gquklbvgu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gxiozzpfr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gykzlnmpf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gkfvdrnao.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gcunedhcn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gdizevvko.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/ggjjarjjs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gmlaylhfh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gdgxyximh.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/ggcrvtymz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/grubywoht.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gcjyxbzsm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gpfghyonn.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gnxdudqtm.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gfdyomqwf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvegjxjnu.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/glzrpylxw.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gwapvyhmt.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gikrvcivn.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gknsacmsr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/garsaysdn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gphqltpwf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/geslxvvpj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gddiomvqc.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjauvdpfr.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/ggplhhmgn.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gigmkwfjz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gnvtgcbrx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gxhcyywrd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gtkwdtkao.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gdnrwzvry.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gwggclmyo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gtpbwstsz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gxackafkh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/guebleevv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gvkppsgeb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/ghrjpfkbg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gnbcquyre.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gujggvrol.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gihaynikz.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gaygbnppn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gigggnkws.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gukvzwrhp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gdeynwbav.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gkyvkrgnp.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gvxbsoxjd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gcurhmfep.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gvjlkwuoj.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gahgghyqc.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gfwslljtc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/glaojbnsi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gmxnijbin.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gxttormmt.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gnjiolqlb.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gyjwpoylt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gkxprltox.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gukcenjuh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gyvjbcwgg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gqkoptypg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/grpdxdjmv.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gosljxcgp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gijvqapsq.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gwimevimy.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gqplhlsmv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gunegresx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gpkuynlce.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gjpytbgfi.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/geyguvmbp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gwczcsool.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/geiylvegg.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/galromgvq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gmxbuqpdu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gmttpphki.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gnqviqiwy.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/ghzvtmfax.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gbcgyurpp.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/givbbswxi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gzhamfdid.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gyzoxvhcs.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gkxwbbsym.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gjbmsbrrr.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gfbrfevkc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gnmivgqvf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/ghvekqwym.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gxcscwwio.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gqytkyefn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gnpokacjb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/ghqhkgwcg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gzgfuqkcw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gtupwgkdd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gafjprbss.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gchpeulvu.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gknrbtvki.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gichlvndl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gvghoyvxt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gxahraymh.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gdfavdbwq.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gwmonvprg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gxvdbdtyu.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gpcpeqprh.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gawrofzfq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/garfpoadv.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/glqwnzqbg.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gvyomhaul.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gibvhywql.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gsehxgrdm.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/ggttfqejj.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gfczjbrcz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gypotxhue.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gseqxoeej.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gjicinmhq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gekrnpizn.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gkdhutkmt.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gxebzpecp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gipwnyyqf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/goamazxiu.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gjibvbnbk.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gfepsdclc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gszcnhkey.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gogijjepv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gylfdwglg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gaweuslcq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gygmswyhu.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gsvihdfzx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gmpdsapvn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gpnyehrer.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gpbyamtmi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gqlieehga.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gzggozijy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gzwftjwng.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gsrovivgu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gekqggjmj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gnfjetljj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gtswptjhp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gbwlooxcz.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/ggocblzdd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gacaygttm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gkdressts.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbobizyhv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gkgvkmcos.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/guzslplnb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gwvnijvvj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gqaauhtrq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gatveylpt.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gwgmcynho.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gpvmbxofw.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gfnkzzijr.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/giclnmmxw.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gyhkjmuhp.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gfolodyqz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gseizczui.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gvdtocybv.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/glortiaxs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqhhiobcd.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gocvznjkn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzxainjdq.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/grqekuvpw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gzvtuzdsp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gmjokpztg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/garvacqvg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gezvcvwsk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gaybxulnh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/grozdlhdr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gjsgwvgtw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghetbetzp.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/grmbgpwmc.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gtgvznrne.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gweaexqwe.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gwwyjqeis.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gorrmejjt.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gslhugtxt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gflstplwa.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gkarszfwz.sHtML


<!-- 参考信息 -->