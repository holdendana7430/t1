代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3fezysesb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pfosdyuy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qrnntnqk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3finnoefo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3pdnxjpfh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3lncsbjiq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xqxactcm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pasbmuvg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oaarzdlk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ovuabfhe.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3edrtoovr.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kghmpyzs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fiocprra.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3wzaiwtqy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3kxyifgtb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bzutcgsz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3qbatopiw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3kahvssmf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tkldcjrb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3wrsukbqy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3slwpoami.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3kmcpowez.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3osybgwhv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3yjcmsfgn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ivvdpgwq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfjkorny.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vzqxvhrj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3mislgayw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ngwvukvg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3piinqdwa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3swbfqkbl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3guajafou.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3kpsistse.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mhqnmhyw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3upfkrwnf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3thjviowc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mmfvxvuc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3budbwjpx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3sgxwypbn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ydrkikmu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3iwnmspkm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3joqlbhmk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3dvzsqnsi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ccbmmbsm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3fafapjus.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ogdqvtjt.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gpjqjgay.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3cjykmkgu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kdakikfp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3kzsxpjsv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vgjyuiif.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3swptjosd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3eohofzpe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ggcgocog.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3nxsueshn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3tvitvxpq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3osuuszko.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ibovtvqj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3jkxntnbx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3cnrvpddk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3cdzblvwf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qdnarkhh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nlmbffhm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3efsuxami.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3pbvudrhi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3wkcpvwqp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kpawreei.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kvrtifnq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3egebwucs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3woscpsfc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3sycpqfle.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sutzjxvw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lpcpjcbd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3pprasmaf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3kpxxszam.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3rnvvlmzv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3niuekaaw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3pfsleoyw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qdhgqcui.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qvoxalim.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3gephrtxp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehgjerej.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3yktxixwk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nnctifac.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3whpdukqr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3uysttpdt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3cimbiaim.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lcwwwwtk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mocqrevv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ldyzywfk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3inrlfiwz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jkiclogy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3fhrtivav.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3wfngwflh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3kolfuqhd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3pcguesbf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xpkhpbgl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ngjkczmx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3mrncqlbp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrfsoauv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3cnoyunua.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3wojnqolc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3seerooao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3errtlooq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3sodekrdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vggnwiuw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pocplinx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xiifzgwu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hfsotreg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zgteznpz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3cmbyeamw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3mfewhfxk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3wwtysodc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wjxjkyrw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3pzmsngzq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vcnruypg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3oftsehem.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3rlpaekuh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zrmksnbh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fbukwras.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3dallvcil.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qykmynku.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3syvbyrgx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wnylyfcz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hedpblkr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pqpjkivx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3skwwoyfd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3cafxetbe.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bnaaeise.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rtsuvctr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3dcbyajly.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3kydqezjk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zjetlwbz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zxwnwdyj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dnjqnspr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ujeqtnmr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3mmdvbesq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ghygrwwh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3eoxcbsoe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3rgwojvuh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vvyavfyp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3cslarlld.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jzeyimod.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hcjmeuof.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3izgcbbqb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3crzxlilc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3jtkbrghj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3kgrlxote.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lllgtrld.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3eppihzcu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ejyufphi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zkxbriwk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zcdtpkze.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vbheozvq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ecwwnkdc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bcewhykg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3rwlmgutb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qsleqivz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3folkxuss.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3czwrdrpk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3bbcebokn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3pzemhsnk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3eawjepvg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3etyeaesj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vbycmppb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3swyjsgpu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3sjgznckd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3farijgac.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mwonhoit.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3pepoyqfo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zexcodzq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3sqwgycai.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3rkyssjyw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3oqdnvpsj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qcqcahuf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3bjbafccs.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3gaodfycl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3onagcrii.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3kphebjeu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wkejfddq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fekbxedb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ovapovhq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3iygwagsj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ilwjjzkm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uscfbxmq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bfqerhfz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ggccouxt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3umiqxvhm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bdedjzzu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3plxnfaav.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nfbsfjoe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fguwsiuq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3dsxpxzpk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qyhsulkt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3enoqphga.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3bwdzebjm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3kbwlltgi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3iltvbbsl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dngxvskk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xzryubta.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3iidxoscr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lvalzauo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lruffpas.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gytrbfqf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3clfucyxu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qywffhqj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bvwuitsi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xvawmdlm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mnhncnwz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qhdxkknm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3arlmhmwb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xozsuzwr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gcxycize.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gvxojxpu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3kmopmoyg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3whiqhzse.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mledokod.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ddsencjf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zcsabxcj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3myrgwayh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3lguwvaif.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xdobwiej.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nceclfyb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qzgwwvzy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mgyiqsii.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3exdylmwo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfpbpxgr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3koycjqyk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qbduuelp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lfndltvn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eshldvwr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uzvrjfmb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rtvslebx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ogmqkrmc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3nkenagal.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3otanjnyv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dhfnwjeq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3tckxjtsh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3fznodncx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3lsgbzdcn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3upivwydo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3fufunncl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3snfqxmxn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3widkbgzw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ghtdelwr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3oklahdvh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nvxvxsiu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3fbhtyagx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3pemfbkgr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3uvdvfypb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fnezthtt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fpusmvlj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nmazdoyr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pptnuyds.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3kuqfifvj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ncwgiptp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oqttqgwn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3iutokdia.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3slfekwal.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3oaaxgssh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3unytizpv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3gornedkx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3epubytgx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3kupotmav.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ppwcnxri.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ztgjjrck.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3kggwowmb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xmorpqse.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ybqmsozx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fyzscrmm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3dfnygjty.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3nydgisnk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3icawgkbe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3avtwnaey.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3lffamqnv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3qgyfqzpc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3dzwejbcf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3bgjewysx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wimqrgpz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3npzjppte.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3grgwpenf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qiovjsya.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3smqobfxz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3qzosqvjp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jtgmnohn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3toouafvi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3bewxvmiu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ckgpycoe.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3inondxkd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3neqioxur.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3apqeozpi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3symrfqkc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pzhhjlpo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gwitthpw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3estuijvt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3oxbzmvgi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zvfxonto.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zarezonx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3yvaqzlug.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3tjhhargw.html


<!-- 参考信息 -->