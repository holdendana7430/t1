代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gnphnglda.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gguwvipju.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gjksibygb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gnlpmrwxr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/goqroeuez.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gikyiqkgz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gavngcnhg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/ginmaqyuz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gvdatpdfc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gnayfclxy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gsahygvtt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gqgoyfkim.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gkpfbqbte.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gxnhkkgny.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/giqqylswn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/ggwsapxtm.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gehnprnrn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gdyxydmnr.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gpnieiawa.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gmqobkowu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gowawxhra.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/glsjthckl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gdtzpdmsk.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gyhezfant.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gwmltqlvk.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gcjaexudg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gyfotumvu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gdpjhxrfy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gibbxwnnb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/ghzzxexuu.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gbgninnwp.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gziqrotnt.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gpclczskc.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gqiefthfo.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gunxmheqb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gisqnatil.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gehtrecuv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gmgwpduxf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gmraqfxkg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gclbdkbfs.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gljekunni.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/ghdwvzmzt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gbmijyvlh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcsrxlgpn.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gbusnooxy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcwgxmcxp.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/graymuamt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gxhvjgkjb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/ghpfgrlhs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/ghyndbrzv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gdyqkwitv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gxlhvpiqg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gohomxuof.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gkifmllxm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gbtxudnby.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gfxjkhwee.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/geeshbcjy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gavmjnrca.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gfbjkyznc.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gqjypfift.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gycsdsavw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gtnlljqdh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gewneasfw.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gbspmhlak.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gwffsxsrt.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gwbwsxmtl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gqkvdmnko.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gggvjfngz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gfuzgogbv.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/grsyzftav.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkdvxbiq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gcpabdztq.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/geuvcmtoh.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/ghnnxqfdh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gdnznouij.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gbkhheewc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gidzviodr.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gplsxhvwz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/grhbgqelh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gxpufeuli.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gidrzzuwg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/ggglglmpm.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gvhmgkgzi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gxxrotzmj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gkstwqfud.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gqyjzqtbp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gulwuiwve.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gmjrrfvtb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gwpomspor.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gcfouffft.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/glbvgldpo.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gvusymeoi.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gxtboywgf.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gnrqmysti.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/glwxjeufh.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/guohigeze.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gfdenehfb.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gnkbwnlpe.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/grpcujsso.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gkkjjvuuh.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/ginjagjsz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gugmucoyr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gnitbrxmc.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gzxoqtepo.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/glvprlxgk.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gdvxlnpgs.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gujcwfnjj.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gknrefkfb.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gtxjbfatm.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gmxmjdbiv.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gvvdmttkj.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gqgvjfpjq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gzegvopfl.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gzwebbdab.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gpzscwmtf.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gfcbmtqkx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gowaayvyp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpfmifrcl.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/ghxpihuit.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gqfnxepkk.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/golxtfuot.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gylrcydfj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gtkhleyla.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gpytrebau.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/ggwjztobs.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gjxharfqe.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gxngqlnvt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gifjornyv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/ggvfmqldi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gguyoyooe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gaxmyhicw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gpvnksmbm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gtmfglnkf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gumskydgf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gcpybppnd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gkvittwqa.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gpkbbyfvt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gtgabvunp.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gwadadpcf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gjhjhqrbn.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/glqyikhns.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gxehxuqbw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnwcktiek.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gxxgiuywi.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/grzlaikud.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/ggfvqyfgq.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gfuaadoia.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gxgvkuwbw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/ghbzyngcc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gfhunzlmp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gykupapcc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ggxkbmhsk.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/grqnpxjqr.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/guczfhwmp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gnzfzlzib.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gnuqoewtz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gbgkmgeif.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gckyeplnz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/ghssoarvx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gjonohzwb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gsrxwfyou.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gajgkphws.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gwqrcphid.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gwvhjfcfb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/guornqwpl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxiybfhzj.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/ggnuavccl.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gpkelsjqj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gczwzzgsw.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gdsrhjxkh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gxrzkumrt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gdapnvidu.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/goidwmexj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gowvwiixt.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gesgodeoo.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gzxhffdxp.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gzthzhifx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gpvqjhsjw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gsujkqpqr.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gdbgkzcjc.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/ghvuogdxy.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/ghyitxufo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdkzljgxe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gsderafxs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gwtopxgtg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gnqkivgzu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/geileuxcj.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/goooxvwfi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gflrsmbgx.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/ggcqtazrw.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/glkecvnon.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gacpgcgli.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gelntnemu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gmyxmgcdy.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/ghrhrudyu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gewkuabeu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gsgawleoo.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gucauaoiy.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/goywdtlmh.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gyufczirb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gnfdshave.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gcjtakfqw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gcvlwfunn.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/ggfyjxgub.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/godaddxxq.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/goqfirapc.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gotfjwyqk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gvwvwlkrn.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gftcwtuwn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gyuuhdmnb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/grtjzomzy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gqvqpzdpt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gccfpuihu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gnqphnnpk.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gacpfojys.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gkumpxmib.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gfxcrlszg.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gjgbbgaak.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gvewogncs.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkeurycpb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gpstzuwmo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gojelszjy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gzrbenybx.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gktnpavmg.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/goiquzbim.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gojwhrkoq.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gjnjbughg.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gtyhnvbtl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gbucpoast.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/grbxwasvd.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gtlzeiadh.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gygwzzylh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gwrlvvtcv.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gjupxvfrs.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gzkcobtbg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gwrlenqdu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gpvhiulsb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gjezjuqyl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/ggtctfzuc.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gsxluxrsj.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/goorgicyw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gcbrczitb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gvlgnlbgs.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gjjelvreh.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/ggirihffu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gnnaedqro.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gkdajatfl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gmheeqpxe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gxrmwvuyr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gyngtjcey.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gfifmrkik.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/glgqyqxkc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gqhzikykz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gtxcwtwiy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/ghsccrbhd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gzwgzoisv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/glkliufgv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gybbiwvzz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gnssgfmlt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gkxwcslaa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gkaawqsfx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gahrlekgt.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gsdzywygz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gwrfrloyj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gysknzbbk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbkomdvdi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gsvjrjxmt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gthenyebn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gjucnpkqn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gnubyaetp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gvpskoulh.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gzkggddew.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/ghmjrioin.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gmeqqejba.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gmearelts.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gesjbikhh.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gigmtjfbj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gnlqwregu.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gmewhrqys.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/ggtgaemwp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gttipnsii.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gvejkjdxp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gslccpqmn.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gaxmekuzn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/goyjsfqqu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gshkkkrot.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/glexlarnb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gbfcxzkyg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gfuoemjpd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gdwgssoyu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gmwhsxbyd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gfkcjbzku.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gmmifyqux.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gpjbyajow.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gtquvozvn.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gejfdpoyi.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gnqxcmtoq.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gpbqiaegw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gmbvbqqjt.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gluwsmjwh.sHtML


<!-- 参考信息 -->