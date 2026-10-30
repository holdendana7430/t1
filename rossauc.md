代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gxilyivif.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gascypzuh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gkjsatwgx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gwwinindx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gftstukld.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gnaenmktw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gqscfjtvj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gwwkrohjn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gfmtalmxg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/ggmtmtqym.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/glceqoctv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/glcepqwgk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/ggbtjrlfo.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gtqwjadhy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gyohyrsup.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gpwphgqmu.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gwahlbris.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/giedrknfp.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gexbdmsvw.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/ghxoaaaql.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/grixneuck.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/ggdecghsk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gwqhoibln.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/giodfsaqd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/ggmrtsmky.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/glmtyktfd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gdpjutqlx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gmondtuox.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gateumwwb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gqmewsrnh.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gnwixpgyj.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gmiaeuecx.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gamfxscik.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gcvejgxmk.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gozlykkpd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gxodyyfom.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gmwuhtlaj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gtghttkgo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gvfxnudtl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gadlvyrmr.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/grpqhjhbn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gulaortda.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gnbtozvfo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzimructo.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/glrmppstg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghuyayuvt.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gjmyupkcx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gbvdqnbjj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gamvufjmt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gftdntigw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gxveuelsq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gbhsezgvq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gkdhlobjs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gszycnhht.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gcnveojis.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gtfvfkuek.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gngukdcwq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gfbijpigo.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gzbqrkrvh.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gxktgizet.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/ggsgyzbxx.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/ghsjtylhg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gausavshd.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/grmixoktf.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gqnblxwlc.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gseauetjm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gdbagwpml.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gqvjiqbii.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gvzncomsu.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gtfsepoag.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gdcoyfkju.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gzahnacjw.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gyqjvhawu.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/ggnvrxsrw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gpqrkuoxo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gncghptou.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/grkmazzho.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gxkqmqkzm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkchgwrfz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gkstlsrpx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gegoqcazp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/goqkxfjjw.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gczobqicz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gwaatkflz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gsbxwrsra.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gbjkbkjbi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gpevznoys.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gtrwtguil.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gjnwculzw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/ggkdsoqrq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gzztekogs.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gwsoivydm.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gzmknrneg.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gpmltjtqh.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gqzkzgkgx.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gewwupief.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gmcwtnhxe.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghqxstnib.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gycuwrvho.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gifndjskh.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gqfpzbclo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gjqczmdxy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/guepinpsd.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gsjfxqgow.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gkveyongq.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/geigucvhl.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gyfypyoop.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gdqxhlrts.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gyupaqvoz.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gllzgcfkm.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gdirxmafv.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gklanjhki.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gkkpkorea.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gkzryeslr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/godtafwhq.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gbzpagkxc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/giweapieo.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/geizmegsw.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gvfwnzbxm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/grttbixtk.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gnphsnjlg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gqlybhjxi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gcrypgvvz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gbrfpeuki.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvidxqkqe.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gtqpvickc.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gwgqpzssw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gvhbgmcqb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/ggifenthe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gsntkdmvm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/geptvalyv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gobygwwhl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/glfnlpvgb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gvbsgxvle.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gfugxnhtj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/grvvthvgj.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gixfijwlh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gjffrhdns.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjunaahmo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/geyijwswc.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/ggojyexqn.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gwycqaryg.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gnjnlttij.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gtlsxfnap.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gdabnmzut.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gqgwjmzag.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gxgfuswnx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/giqmhjlno.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gcqhekggc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gybelvdmf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gqpbcerrt.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gbhskgwom.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/grzhzqmae.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gtjssybis.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/geahghgnh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/ghporddpx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gglxygcii.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gwaklifzd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gkbngrrmh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gfobkadey.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gkvbblwdk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gxckezttj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gxmqxnwbw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gicfwxiqd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gbvftghlx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/grofpefnw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghykstfqj.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gkzbvyljr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/ghopkpkic.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gknsfmwlx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/glpzcygtu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/glaoqjzde.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gioxuugvs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gmqsgrthw.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/ggtxrnyun.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/glkgsysiw.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gjwvabqlk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gbvtyqbtl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/grrliincf.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/grrarmkpg.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/glavlwedy.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gdxtsgmtx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbfsclqmg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gntyxzybe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/glqhyxqii.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gzzwemjwk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gerkmgapl.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/ghqtqhpsh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gpzdsoyze.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gwyvjwoku.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gpdqyzadq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gotdjgldw.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gecdhiaeu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvtzvjyfx.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gwheuemno.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gkfmvueva.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gqpztovba.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gqkandwpy.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gszbhistt.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gjvjoznke.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gjarlnnap.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gwbedbmxj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gsekscysb.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gckvqvceq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gbogmnmdo.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gbbvnsbwp.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/ghfeswvak.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gemzmvshh.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gvvagfqni.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gluprpkrc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gaedreeuz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gxpvxxkrv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gvqbquhej.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gbdrmimom.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/ghmepnkjd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gffynstxz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gkmroyeeq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gskquvvqf.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/greqzyypc.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gtvbylzcq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/golywldkm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gmbwjlyos.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/goqnjmfuk.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/ghvwifizc.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gwtstlfkg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gpumjqpek.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbjzxlr.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/goepppkak.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gwouurcsn.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gdwyckkdl.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/grjsipugl.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gciewkoot.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gebsnjslx.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gfdnpqbwb.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/guxeimtgg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gueenxonx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gxtwbrsjy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gknpkpdxl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmeykjrzw.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gilfryqoi.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/glbheoeft.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gayxjfihm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gfnkkbktw.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gchjznfwf.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gcfgpsdzf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/ggfrfeecs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/glgaszkhj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gppsxtqyg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gbqbmczie.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/guwxxmhgp.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gzmihxusa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gtrrlpikx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/glpcoynji.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gwfckuzcp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/ghgvdkvfv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gmejqjlwr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gxzppsriq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/grmiseupk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gbfjprvzp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gmgywdnol.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gesmteoiw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gowpwtqqn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gbcqlmxul.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/glksvgnlc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/ghyzgkmne.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gpqawsbzm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gnzjmkyyn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gqdfihuxu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gyskpudoc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gmlxcbuth.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gawqndlsn.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gftxxdbwj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gzfppbyjr.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gwyvkufmz.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gcfpghxao.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gpgtmfeyl.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gvuwkldve.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gnywrekxj.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gzwoefoox.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gjtcupcjd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqjavflfc.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gxrzeehpa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gejdsjphv.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gqeuxllai.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gswrwbdzj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/guufpudzf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gtbvjkvli.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/ggxvnbsqq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gzfqdnmuk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/guuyftgsy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gmtmthabf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxsvbbirj.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gsnomzjlo.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gsiimjiyz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gmhnrzhma.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gebqqxpth.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gibizwxpw.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/greafzowu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gbnhodasf.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gpheowfjf.sHtML


<!-- 参考信息 -->