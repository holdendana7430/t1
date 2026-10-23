代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3obwwxvug.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3rthwjvxy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3dqxzmgcy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3qqjvuxnb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3xxvvcram.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3nlafxoge.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3uxkhawqj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjryukfs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtshzfjf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ouaurllf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tshhdobj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ulrzskka.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3rdavouio.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3kfkhqtvj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bcmibwtk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3mjrlnfqr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jdhgymbj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3eyxsxsrj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zbgjyiiz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dqlsjcjp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ohkyrdbd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wxzytywn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lpmwflpn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ouafofsl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tdomguur.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yrplrqng.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ykkqfauk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xknmdcde.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3sydegjtc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hduqrxvd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3yqrqjgcc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xgvuqeui.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ebqdohvt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qlayzmjf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3wliyziav.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lixsqtsp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3adzlfrfo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3blrnzkbx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3npeivzoy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xcymekwo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tndynjkw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3dwtwkvzt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3xfcdnwti.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qbacrmyz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3tcpolafz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3dkgipgvk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3xcklqnod.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3kwpmfyom.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ywacilrr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3sylkuzjg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ovmdzsqt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3zjjpyqky.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3jafdvvxq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dpamngow.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3axoeizxo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3spremhnt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3nhqumfin.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ionjspgy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3psnfxymv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ywtvzani.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3efplopem.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3usfzktah.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yknmyplb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3txyuigai.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3enaurlen.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3slswjrkx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pnygkpdp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wpbfcycj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3usftwegz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wcwgbbuc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3yosblqbt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3hqxdxphs.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zkatplmj.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3aworfney.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ncgdduoh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3cxbccjry.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zryixkru.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3zcxozimb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3crjryxop.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3kogretbq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xqnxgukr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3guukbmci.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3onmbkvgy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3xyyfhcpf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3skfzltxj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3vogqnqpy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3gkonquku.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3bofbgnit.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3dxeqgbud.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qrnmzuvs.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ylryevob.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3rjlybrki.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3nzfltgga.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ipynpsbj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3bfurkfcn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3hklnjffi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3kjwyfalq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xpoznxyk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ipcgitfv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zymebgzu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqmotaep.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3zgtuftnm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3gqyihdgs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3gnmdzgsi.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3slivqiic.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3gjxfxzgk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vhlqweux.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lfuhbynh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3gdczaljq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3agvhcctc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qyziwvht.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mrnwthkx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bxkcsfup.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xwvoqhle.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3dbmlytym.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ddbmmzul.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikfvuvdl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3thuuzstn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pgyfadxm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qmkpwwix.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3knmrjggp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3wmsuglui.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ujjaqqzs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3flcwunzc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ekpdxdun.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3kzcmfjoq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3bnhmrckf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqfyehiw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ahfukgxh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3sdpkjgqu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3zwvkwmev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kutfeofx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3dgjenrmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdzhyuur.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tuymwuar.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3hyjyqrsu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vshqdjtq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zzogvlho.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3haqlftgt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3szrnxvmi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3pgrjdtal.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qwxzxyxz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qndobxuj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3utbttzus.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3uvcvhmgu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jaiebbph.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cynusjni.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pffesuyi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vyrddqli.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3eqrrogej.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3npvadzqt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3nmqdzndc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ionrltea.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hiotekuu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3duukwgqu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3yevjyeee.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nmyamvuo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oetvhzix.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vceksozj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3cmdahmlt.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fuzzwafg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xbsyvffm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zfenrcmv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3uszmpucz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ujcztvmo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ozrwjzhl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3bstchisu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3njprxvuc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxxvbhoe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gnwdqryv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ymccvdvi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zkjiorbt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nzkszylv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hjhblmfb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3uuxgkqla.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3iouliyfl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xsdrtzbs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mhmiqvsz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rdrjdqlg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dnnhdbte.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3coyzkome.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xxumkkyl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3obrdrsax.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hoeyytsx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kxvhrflg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yodehgvm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ysjpikzn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ruptanbq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3tpcfnhqp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3anvipkqj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wahbzspw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dblmbzdr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nbrcaetz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3exoquwtj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3wbtqvfxr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nkyudsnu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fimkiboe.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3bgfkujwo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3pyodibrd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qehnydmt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ggaobjpz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ieoookix.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3bcgbimtx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fmpmfdbt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3fubhmoih.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3susqxfym.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3linzcpsm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zwcyhcfu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3dhvnfccy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3uezrzwtg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3zvaczlnu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3hvmlpnwa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3moqbfoiw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3diqowybi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3omxnceta.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3nkxhplns.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ojxpzemc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3knlnupyf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kljekyag.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bwxvtrwx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3hdqlxlmu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3krwbavtg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ftvxdhss.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3kxlyiwcj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3sacyjhhx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ieoeevmd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3uqgnujwl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jyuxsycj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3sycdkzik.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ycrmimkf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3itmwjgcq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kkerqadl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xcfkbjxr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3lzlcqgmx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3sgvkyktq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3joiackkj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3efyphlce.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ekfloigi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3zlbbsqlv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dfsjoprv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pzkyytuz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3cayjabfl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rtfmvuig.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wjqpiogr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kvvsmbqt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bjkdawdi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3krprniip.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cclasmjm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ywdlcput.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hbvqxuwk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jpkuoxsn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3isiswnkt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xlzciyzg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lcrkcmqn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zcppqlah.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uvzdsaxh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3lsbunznv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zhrwytei.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ywqimaay.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yjjqeazd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ajkghwrj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yheycgtk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3zisiscve.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bzfyzfhy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3sqjvxvel.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vyzlrkro.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3naobqtvu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jishnyss.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vbedbovz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3xzzbnzaa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3evazdtqz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vwbagxix.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ivyydmgg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jqpdlhrw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3zalgluyx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3nrsxcbyj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3monxeyzp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qxnwivlv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3stiqgonb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nprwipex.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mxvxtlgg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zspogkpz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rylfdgzc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3oyrykypb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kxkiclqt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3yjslghka.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3nituuvug.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nwhohdlk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3yblhgdrq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lyyizpnk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wdwankxw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zzjmvyov.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hwisffml.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3lgzuybuw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3jhldecmp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ysqbdgfr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3skagrqdx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rrvttozj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dicakgkb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3cqvzhuhf.html


<!-- 参考信息 -->