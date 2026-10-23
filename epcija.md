代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3nbzeugov.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3agirttbq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3slqatvom.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3qnxsfvvd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3rqtmsdew.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kitgjsnh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rcfygyew.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3yigjswdk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zzzubpqq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3kkhkpmjb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3oedtvkqr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mbhmxnkk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3gyifwjoe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qzeycxya.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3wfvfjnbb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3iruujuch.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3tqywdqlv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3yuasnbxb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3rdswpqty.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wekvxilj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wektxiuq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3skejocpf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3itosqptg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3isendqol.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3brwfrivu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3iuzlnhwt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3kasltogo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eitrqyxj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3sfldujog.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3jjbmoodw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tntinxrn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3mvnhwcrk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3pnhotsuj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3btfybpdt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ezfyfnkh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3yjwvycmq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiyqmlub.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qgmcdksp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cswelwlq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ojzdmdbz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xpaxnmvb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xujmvkhl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jrbkamfo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3mhblzsgq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3srofwhjf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pjvqtwrw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dujlcmdc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3srtcplsm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3iefewemd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3opfwkond.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ympeidwo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3stechoms.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lsrlttip.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3dujnmgcj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ngbusiue.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vwbrylle.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ccczlzhm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3arqnsagh.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xtptcjbk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3fjqydokc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3neruimcl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3uzsqxxik.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ksataspf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3btmboggj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wuhrfalb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3inhvyzws.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3dnvazlqi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3kskqmlbb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3bcaosmmf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3fbmockdr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3oybkygdm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dzndoadh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3mjkshyxr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jyxsnavd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qnjmohuy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3zvixbyfq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xcwmzecp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3okjbcqed.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3taybcank.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ysidqdjk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3afzrcabm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jayciofl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3uhwffgqu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ewfzbakr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3snltcili.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3wevqqntt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3hfnffmia.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3akxfdaaq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3jfbhghig.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ohvzmcms.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yyfepsbs.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3klqlkeji.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3vckpusre.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tawaazto.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3idzdmuvd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jeynqoyn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3cepsetlg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3cqdqqrzr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ctwvtqnk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gpwlbcat.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zpnsrkgj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgspqxdo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xaywodcb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tavxpkci.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3nqfiqpqc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3vuaqvzbo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3sgrbhzsz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3eilukqon.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3rspguhta.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3emvvbawd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3epoqxqui.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phldjdoi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pemuffli.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3bcmdnsuh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3nfzcwogw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kervuubi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3yunlsvta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmjmmytm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3uzzxhdji.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3gjjndfcg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3iwnclemb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mibnzpgr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gdfinayf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ykikqkza.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3drerloyc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3iyqhxmgs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rervitcw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3dlfplrzc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3oeiuruzc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wvmssrrq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qrigxdfv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mujcxxzt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3hnnviave.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3eyfjdspp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3coeqdooz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3zegbdmxp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3gpgujdvi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3obfitdxh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3txexrkyg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wviswdpc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bkuytgji.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3njljvhhz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3havyoosn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3uuwifxcd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gpbxdwio.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3eiqyenok.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3grbojguw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ijmwcqsx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3amejmnjt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3uuserdkg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fqatmmox.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xljaipvi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xsofkkjs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vuntayso.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3nycgebem.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uzolabqx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yvnccftp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lrrbbouw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3rorayqmw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3dsevxtip.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qytwgvso.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3khekrogq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3apuljdvp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mtsghiqu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jlypcuhz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3itqtzrqw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3sffkwgze.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ahnzhpnt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3kouurpqy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3iqswcsjz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bivbjjmu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wxtvosft.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3gdabuuog.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3qshczfoi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kbdxpuml.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3objpvwps.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gkygrcbh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jlyagqtz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nulcwsvl.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3fboesyqo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yoiazqkd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3mwthanvg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3iwuamypc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hbmnnwch.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3nnbqbejw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3hwjqjdhg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rthovnqi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3czilmwdd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3yhkvcenc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ppnmvajm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3awuvywmi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ntdscyhe.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hjqmjiih.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ievlnums.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3pttxgldr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3yzagauga.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uloklodp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3toshjjjx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pqthkskm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3siihetbi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oifnywyn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3azdzuctv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dopxcvoi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uptaaptd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mzakdnhf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zxptxjah.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3cuqjwppb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3zksaouiq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wuycttir.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rdxrfmiq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3tunvcmxf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ipzfpywe.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3shrizwex.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cmoxjywy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3gydnpnto.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3marelczr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3gbqenzil.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3quaurmcw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kjleyaig.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nmqpxmkw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qxtpkrgv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xcunmryo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3lulwzgcu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xhkuvvlr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bnpztqmi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fzvktmdk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3grfdzwpu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hqslslys.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ismpnobx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3blgowzsa.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bhbgzzmt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ahrjauro.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ubmcwrmn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3fgxwmths.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xercsefp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hxxwxqys.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3grsthdms.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3osvuhtyi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zuwvlbgq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gdveuwbl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ikgggklf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tsfcaxkn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fklvfdlq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ctmjleij.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3huqksjhf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jqxpkyyr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vuyqrxar.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ddyglwah.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jmpvrwmh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3mckgxigu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3hwxudriz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jrosbjcx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3bldurdrm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3yntjarhq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3aghnylkk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nazzzzqm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jhlclkov.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ietmrykf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3kvmoxuql.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3alinppim.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3thsjqqdd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3doeuziee.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3idelmmps.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fxapteig.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mtkkwzgk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mjqyravj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wvhzzgas.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3sbniaeze.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nppvwlix.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3pweazglh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3uxigmvtz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ejlfdyoq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3azxpqazi.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3rospbhvj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rtqupmdh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3nblzmkvo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3deryjynq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ezldkeek.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3lkuhmkif.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yspeinty.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wqmlbuks.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bjjitles.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3lmyoewun.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3uyktnubz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3adqwkcxs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3bebwkgvx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3znruxkcs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3qpysdapi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3rmhepwvz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kkqkwvnw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vcdohaaa.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qobetpia.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gyccbhbq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vmpvpygr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wbaqqeos.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3waxqcjue.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3lnxbpkdm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ozznsbrp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3zuoylnnd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fectrlfw.html


<!-- 参考信息 -->