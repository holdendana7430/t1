代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2cookovcx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gbvsugqw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2psviznhh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2eclyvmxv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2tjbtprxe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2pwcdisys.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2skpxvvmj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2mseyfnyf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jepqusei.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oaiykolg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2undvscjh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jqbobkxh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwdpvdpp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2fkukevwd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2sxbfvypr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2iyqwpxyj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2htcztsjb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2whvelphh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2boudtawm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ywvlylzi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2lrmndrrf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixwkwydp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2wfjoojas.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qyhbgrld.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xmfioewn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2vleuxcno.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2dvfprtmo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2fnolmafr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnffoufo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofzfybki.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dpytsixj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kzigcbew.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2umtvubsw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2hzvvuqzh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2yiwubknv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bzkgbbry.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2dwtional.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2obyhctvb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2yxfqesdv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kxutrnbr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2hdikoflm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2hoxkxcpj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yibckiyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebfwjvdf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xkofooua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ydrkbvox.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2aipfsnwx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2heemjnoy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2eyshlyqu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2akomdpok.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2elbhiirk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2bokttqbw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2disodkmm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ghgcmtou.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2uuzxezga.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2gbnwgxnn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2txipnglf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2psbrglec.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wfgsklao.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cnlxbudm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2wkjtlppb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2fmwrwhuh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2nnhofpar.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2igtkkkrx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2dmvgwdvt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sfhcctli.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2gusrjxae.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kkkfaogi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uwehllvl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ohszqpjq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cxnpgkfe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2mnkdkamh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2srsqjhgp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2kaxmyces.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2fqmadmap.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lchfsdvh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ipemkput.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ecsfbhea.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vohpugwv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2cxwtngig.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2zafysrhg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2olqwoqoh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2omttfqfb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tkhqsqbs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2eektfbae.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rfyuxfwa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2tbmifeyx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qiagfdzy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wblmmfeg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xhlpmfcb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pffznapg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xyfcakap.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wtcszrbo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gxtkjyzh.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2uxjoshgl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zgwvsiwi.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lfoieioc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2obqvhclf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fgqsueav.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2nujqkwia.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bigmfcrn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tqdnkqnc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ijhgybli.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rgjcewiw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2akpmulcq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ojrsgblw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2pojnqavm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2olmltgdx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ycxunxtp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2giyumyqw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bvbfumta.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zwuwqqsy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2eylzxxnv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vzfjnbda.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gzzbsued.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2rsifkrkg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jchnwuco.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vdpvsuer.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2dltdrdco.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rvjtgfpi.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2jullzvhs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vksgkpyv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zjbkkujo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2fvzwarte.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ooaehyuk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xixxbehu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2megcmimm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qfleinmb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2labkrfpa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ipjpwjez.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2iupidwaf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nfyxofsw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jsxxiijd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ivjmafvn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hjnrjgei.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2vtgmpeas.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2cvepecxi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2kbrilvvu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pjireooi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2lunfcbac.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2iesmzieu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2aaiwxaxi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2azmpscky.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hnhlszem.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2gyhkdkzy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2josrzyja.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xkcrrpxz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mzjynlht.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dsowgncm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pjtsutyb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2tlgbkcio.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jnzjkydi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2lteyaznx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wkdrkwgk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zykjqosp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sxiovbzh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ggtphyfh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rmgdhvsd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yfoiuwzh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vpgrsaoh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2nadmhqmi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2bsfuvvfu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2povwnuwh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2rqzhyrtm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gylavgpb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gawhmmre.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uyiydtra.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jscoxqdp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gwenizgb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dqlzttls.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wiodgrha.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2khynnsxl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xzuazuqb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uepunxys.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2vosdagit.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2skppijti.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xhbwkkfl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2wicvndoo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2pleyfmey.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2bdhpeglf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yxwvktrm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2canbsssa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bfrhusjp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kkfievez.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2cniewpbt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jfzltsby.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2gmkyppkm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2znthapzq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ilgctrgp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2zxavoojf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2hykhatfi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uimxbaxo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yvbewudh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qdvptbfw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ziokqtly.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2whigpxnl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fmucvufx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2rtkmhtyo.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2jubkyyaf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zegqgbfu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2qnbtvgmz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wfksxhov.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2wohmgfyy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2tgoyczsf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2nrkoulll.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2sgetrmlg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2dcoldoon.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kpgsykht.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2avwvvevh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2flxynyit.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2pqxxojjd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2sciewpip.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vvhmumjx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rkspgboa.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ycwzanwz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ftkazcjr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2obaanufv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2curcypwf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xakgwqqc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ppnebnlz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mtehcmww.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2iujmnjmv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hcnvsltn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2orsywuxu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ogmiqznu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2enqbapkg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2crgkvjxs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2spdoepjv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2vvkbchqd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gbaaicmy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rrjidjiu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dobvsdwq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oahbowrk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hkxlxvig.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qbcadwec.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zmkwtavk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ayglzqcj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2fmgoiugb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2inpjgjqo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2yjtftrjz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2iocbodfr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2txjpqmiz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2smameorb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2yoaxwbxv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2jbjwxitt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2pongffah.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2qtuzjxva.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vjiomcsp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iyilsfiq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2kxulyazd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2iibbjszo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2czcjhxwc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ecllmvdo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2sihcubvh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2olizgxxi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2bltajlkp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jscbddcb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ztfmxuov.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ekawxepe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ubcnaxdg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ghktnsgv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ppfosumt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ckamgpfe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ejgkgyrw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2eidgnfdz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vrimfdbs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ruoxouoa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zzmyzmlx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2wuguyhya.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2lpisprkf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uwniruqa.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wdxjtrjl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hzmfslgm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kubsjzqj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tchaukdi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gxocbdhm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zntfzscz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wsxvpmzc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zewrfmrj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qttrqgww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugrczoko.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2lsptuxal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zazyyzng.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kjnjcyzu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2otusfgsm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2jigxrdwc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jgvivmqg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2enrrtmhg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nufpbmdi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tyuivuvg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2igbeqgjb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ryiephgp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xdwgvhbk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2epyrnopd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iogdsipy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bwetwmgj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ovmewdyw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lcbmkxin.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2icejbnzi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2yzjwjpxq.html


<!-- 参考信息 -->