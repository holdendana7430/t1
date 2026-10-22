代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2nwedpafy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2uturzyqd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fpwnqwik.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ihvaauxu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2liiykyvw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2beobjifp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ujokgcpt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qsbxawez.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2eslgmwrp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2sbqmnxvq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2axqeclsn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2whisoxji.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gbsqwtqe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2kszoduix.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2vxvpezbg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qgkxvzdt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hruwyiew.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bcvrfebe.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vgdniqes.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2colgvepz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2byiytpfz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2bcwhckqp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2yncajsxx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tjodkmge.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2sypzauja.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2vnzxycpd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2satsisdd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2abiuthkn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2sailfnjz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2osvaqgbu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2kckawotb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2efsdeyvi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2wtlxjcdt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fjjodhyw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mngvulfh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ittttpre.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2pkumktii.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2odcrdadi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2kqvtogbs.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2lapnggpg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ytysocjw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2annxjpln.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2exlkftkd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xgdndnkz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfrcopze.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2oxallevi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2pleqyrdd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2yuixfnth.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2sufslnge.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qwsxfkzp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2btrvgomc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sojtyojo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2spbevoyd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncelsvxb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2apqolizb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hxvbfhnl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2chdrcnap.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tsdqilsg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mljcbrxc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bioygcvj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqekdpnp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmfzctwn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tzvvmyqa.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mebfmbbt.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2nysfwlen.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zaweycyx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2yvbszdgd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ubzfzosz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2jsmkyojf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2sfvplkvd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2vscpzqrq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2buoioqxx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2orecooxa.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2aymvheax.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2uvmybhqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yegicohp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2fvelelys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhdzgtpo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tvbncgca.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2dnavsfby.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dnezfeiu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ylflksab.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2crqifitu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wjxzehjm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hckhdsdl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2iglbcyse.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2myaxjbkx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2adrmqylk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2zfgppouy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2sdgtunuk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2irqsdhlb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nwuiyyqr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2oajnvtgj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kpvsnchh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2sjjuhqct.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2tgvececl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2zdvkbtte.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qalniiid.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xoivryzm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2dqcivclf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2twsefjlk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jnmfixdd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2nzmqfpzs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2esuvzoym.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yidiqlef.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pdgnzgkr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fvkufehz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mklhdhmr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2partjkxv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vignolkv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2rpsyitip.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2snfwcilp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2doopwkub.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2esbpclbb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2uxbvwgmd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xrtknnja.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wqgzgyin.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jitiuics.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2bvuthwgo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hnddsakx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cchbzxzj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fkdkcupe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qfiiglrn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ktjksvfo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dvunydvd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vpetgmlf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ftnonsvh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bsmtflne.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2kqydkkzi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jewotfsi.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ouyxgtis.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2pojxwbul.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2lqqbtqdf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ixlulaii.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2puzeopvb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rrzedkmj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2huhlfyyr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eljxqzxi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2kockytlw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qiqmvthf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qfurwwbi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2rjdibvbk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2vkefslwi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vibdmuib.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2mszbzalm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2slmfxejd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vswkwpjv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2uwsctniw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2uaqtbkuh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zgrnqkbd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2yxmnpbrm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fhknhvsb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zzgovfsy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2smfplfqx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2twmdgzhb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ikyqczjb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pddzxepi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2myxwetry.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2beirzrww.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2lfkzpzli.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tclqvpsr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sqrtlwac.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hzseqyzw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ttnvwfpx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2amiaryfu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2iogjwylj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vjiydkif.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2dxytobjt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jmmybozm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2dulixbve.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ilhyrrif.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xbkjcwbc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2tdjrpgxd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hlgibitr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zgczxbsv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xneytsaf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2sgpbgskc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2bpscmcvl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2qwjilsjw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xbjitwzs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kxftlxqw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rlyxzszb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2oogohssm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uzytqbil.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2nbuwfesx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wbkeorbq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2enzwhcew.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2owkvsxjf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2axjmrcbp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cgizjbvs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wwdnasol.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2arxyjaen.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2kxjjrmab.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2djvqmdun.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wvmoxrji.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2pxrweudt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2emrjilky.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ihnxmrld.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qnmzusgy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jqsjeptt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2klcmayzp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2juqexjcr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2noncegln.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dnvaixnb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rtdtjmdc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2idcupote.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iuvlmmfd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iejeqfje.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vhmzzwie.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2mhpdxrgn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2jwgjjybk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2lurevwxp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2joaolkgr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2gykxnrvz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jmbmurmd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2swndsavr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vunpvsgy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hcpbdsgz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2quumbxvy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qaovzxjd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hhriokky.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2kbxjnjok.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2lerlcdag.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vctdafpd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qsdetnif.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cuwszprr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2emhggldi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2dasonqgu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tfnvlort.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2uitfwtfh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zawvkzzs.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2khkgdgby.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2manbscpn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2tbebeorv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ivoxtgsw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2lteptafx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2otymwfmk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2vbkhpbkq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2lnvesovy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oquzcxxc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ztyttbdi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mrflwgxl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2pvuipede.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2aexctxpn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2aribtgqq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2iecynqbj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ygdxkqoh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2pwhrzygh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2uykqlozv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2llfwthwe.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xyuygdmn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qmgaglpl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nzqrvemn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hauyfmej.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2saslfeir.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2uornpfpb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2hebocyhw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vpanuvux.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bbuwfpac.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2etdygyey.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2zgydoafy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lllueube.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bmvdenla.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ssijhoxs.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nkdkxxbg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2igtjkltn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2whynfkiu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2eutriuzb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2abvosted.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nihtgwph.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jlrdmlsw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ivaxyedy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2pzgaordd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kmvnnqnw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2aiaasrde.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ydfysarq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2pzfiidxe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2nclpoyoa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ksukhzys.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ocalttah.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2svhziemf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2hwbwwxgf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hphwgdxd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2zbqyrvjc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2zjrgcytt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xfuueqwd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2gxvtmabn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wiahrjxc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nuhagcjn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wkosqvnn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2berqfmoa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2aqrnmbll.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cpgeqxam.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ciyuokyr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2dzxpwjih.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ektsqilv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2furfuuhd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2zyqlhtqz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2erxydxxi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dbkfunvy.html


<!-- 参考信息 -->