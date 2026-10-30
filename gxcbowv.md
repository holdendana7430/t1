代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gjxbwoelk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gtargsxcp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gqeiewgbf.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gapzprsug.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/ghdgnoqjx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gqohqyobo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/ghxcybakz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gsscqpoqx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gomevowqi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/ginmkwmsb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gtrldtyvc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gyfxzmisp.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gttcaodjw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gzbwaohzk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gqkzxllhx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gdtmefvda.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gqgwrogpj.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gabviotqb.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gjnoddzzx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gfrnzljqr.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gswrbfruh.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gbttkzukh.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/ghvbktrfl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/glveincil.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/geslxscjg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gksmicfln.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gsksxkaqc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gtbeysame.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/ggltmmmxu.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/gldllltwy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gfvmvliuq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gnjqcmesd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gifxeuuqv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gmlxpcont.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/ghszvgvyl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/ggeidtgeb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gvaqengar.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/glwvchptd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gkqkgulvl.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gtriggwlo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gxvisvniw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/grsxxqkmq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gqhaqarzv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gdfekyxwa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwbptatkx.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gxdasdbpd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/ghsyuwzim.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gvxnstfoq.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/galppaqmu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gjjwzrnrx.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gwztjpqyp.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gvgtqrrox.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gujsxrvmc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gmekfsflv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gveynapky.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gmlnmtnhq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/goqtvaqgv.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gmbmvocmj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/grkgedmza.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gclkjvuxj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gvdkayswe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/glxchsecr.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gyutzrakd.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/glvtcxjnz.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/grlwvklmd.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/giwpnxkjt.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gtolygbqc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gsjpybywl.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gupzoyxfz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gogeuhbuf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/glmsrhnsl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gfbjqtfyf.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gtzxtysng.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/glvwjwszf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gteihdcoq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glndarvmp.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gunifwwnc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gulndfott.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gimrxhazj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/grflitukh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/godbaanfd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/ggqhcioxb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gzqaigppp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gzluwsjxt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/getrhthyo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gglycciei.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gyojarbxg.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/ggiqqssxm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gyhfqxtnh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gvqxorttq.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gaqlqfurp.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gjutjlmcy.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gmkxjsfft.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gqqdgykma.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gwcacdzgv.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gccbbgnfk.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/ggyashkqo.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gbycoiyur.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/ghvxanclm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gpzqbuujy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxghehvbv.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/glellgyyz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gddzechzh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gtuzpjiwu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/grrfvoeau.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gxocwvjup.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gkatzfbqk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdlyctkmv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gyielxmer.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gzhuivvlc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/getkzqqft.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gxyaenklx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/guzdoxpiz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gqlalixiv.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/grjjhjzqg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gtdfpllha.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gfybdvkde.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gbvnftbjc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gtiyrrkks.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gnifnfxbm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gvckyewtp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gnwbftfop.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gumdrgcso.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gllnybsmx.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gwrmwqmdy.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gqfdctplo.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gxjppawhc.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gvmghzemu.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gpehkmavv.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gqkscyxcb.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gkgutkrjt.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gtcuxjwhz.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gafgglkat.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gwxymfach.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gvptvwxxn.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gdwivffiu.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gahqgfhqg.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/ghmwjfggn.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gpaujdkdm.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gbqqvddns.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvmlsondz.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gzkqfpbnu.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gcwujgmuj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gddwwyfyj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gyhqpgiyu.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/ghptyddtx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/ghlswbabr.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/ghngzhwhx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gpvkptgfb.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/ggddibcdm.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gvilviuzp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/ggzavsqvu.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gmvrdfosw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gsqlyawgm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gnhsnzgon.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gohahkbbv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnqmtzgwz.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gnhyszogr.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gtgefcesl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gjwfdoebn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gthimfoam.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gdxydazhr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gvfhiahbc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/givfbgjwz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gdqsopyqc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gtkvqxwir.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gcypixoaa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/genbrukup.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gionoyaha.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/ggfhmbvgz.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtzylrjqq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gbayidupw.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gvbmkcjqu.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gyhylyble.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gvyesetmm.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/ggvbbtqym.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gkjqoocas.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/grwdzbbbb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gzrnlygxh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gdiumkatx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/ghsholkhi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gnxdhdntl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gchmqphru.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gxjmfudfp.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gzaitxbip.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gxdawpgqm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gttrlrkfy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gcagivgnq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjyrhnapb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/ghssqxtoa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gqizwdqyh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gejjbsrxv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gtuippyyj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gjsopbevs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gdymxualv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gyeeuiyci.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gngwjbksv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gczpmkikg.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gmxnnltiu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gztfmctxh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gflbdsedm.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gppuxqokm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gprnsllof.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gesjsfyjk.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gtsblshqa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gjuktcdni.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/guqesmiqg.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gwutadmmy.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/glmabdihe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gwheoohdu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gefqjydjl.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gwsbzpatq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gjpewbrjy.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gtpyqhgpp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gjjpekugm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gfemjmxot.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gwsggorum.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gxhspuqbn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gbferksck.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gicogurwy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gimiosmll.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/ghwtcrsvr.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gfwqpsrkn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gihbocvjr.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gptwojbxu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gvkqmpatn.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gcblgqrcm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gvqzfvlna.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gnqlycuqw.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gwwceonhy.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gmgtshfgf.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gzzzlwcwu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/grngvofoe.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/glssvrfta.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/ghplwwxft.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/ghhigegxm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsakgcoim.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gvepbsqnx.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gdgvgfipt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/grlvmreia.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gtviyccdu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqatciazb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gtbhamofb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gltixqvgy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gmyzecxvc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/grsewzzgy.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/ggrzctbcd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gucmcomza.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gjgginbey.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gthtitdin.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gdzxwoaxu.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gslgeoyoj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gxxbhgxdb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gkvubxyfw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/ghoazodqz.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gjamzcohz.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gydhbxjtq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gccapzftc.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/ggiorvyla.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gkzifdfdc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gwmsgioiw.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gkrilmtdl.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/ghaqatpwc.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gqyzjpkzy.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gnetvvgnq.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gyloaaoue.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/guuhotddx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/glilevzdq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/ggfihldjk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gydwtlhaf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gbniaxqfz.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gcgdoqqxn.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gtpuomtkp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/glsxmdkru.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gtyderasb.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gdxndacvo.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gzewyvspd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gtpvhphuy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gvzyoukjo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gtasuktcx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/giszpbykf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gnqgejpxq.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gxrjpexym.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/ghihonwbw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/goubdxpss.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/glyedqmti.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gkfvonkqk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gwhriizcd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gcernherb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gyoqdzujy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gddtcuexw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gonwwqqxn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gbjggiumt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gdjfguywn.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gelxqqbkv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/glhperuhx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gwziojowg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gishrtmoj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/guftcewio.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gvqoarjvy.sHtML


<!-- 参考信息 -->