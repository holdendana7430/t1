代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ahihbhvm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kwudrkhg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3asgasulq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3onpnuwcw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ehyecoyo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3cdfmiwnk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uknkdmzm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vhaomywa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3rnysnbfr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gsgavnvt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fxzjlqef.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ktparwrf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pzpdjsvo.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3kuyhxqhn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ylvdngzp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xcnbdgai.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3choglmci.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3umeydqzw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3yfjvzbna.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jahewyjs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3byawpkfq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3tkvnxwuf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rlssmpgg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ucpljlpq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3jclcpemv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3vjdvurzt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mjiupdqe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3qqvasllg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3qamyrgft.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3hvrhmefd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lbxqblay.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3usserwjj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3siiivoqx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3japackvc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ehzrtrbj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3pobcpeap.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3pwbqrcam.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3rufvgsng.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ulaizuvx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3mmgckfrn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ntvhdphj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzgevuqh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3icwjsrxk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3auuestho.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rynorjwm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3iehgtzix.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgfbvudq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3rjwjlsfu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3irbpojlq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3nfdjqfnr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ufwuqklv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tkmncoce.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3otojszad.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ucccxawl.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lsecxyui.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3kadejesl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bibdanuv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3vhqjymeb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3xbgjqhma.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bzgaybfg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ahmvdmrq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3xcyoeoys.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3tporaicd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xljontni.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3xhziqwwe.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3tyyherpv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ukuwjfja.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ysjexkyh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3znccgexx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3oayfxife.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dtexgdyy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vkdxdrfk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3zpseusbr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3thfokcto.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3lzhomxki.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3tyrcrtag.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uszesanu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3heudcoeh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qkjyztho.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qexdehmg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kunsfdxn.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3yityjoxe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3yzfmupxo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qpcnrkia.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3camrnxgm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3vnkvtoux.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nghtivur.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dhxqcnrf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqgwcneb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3fjjkaqze.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3cuazvnpb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3giaruvgn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gowpmywg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3wcultmrw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3kxtireyh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3wsbkgstq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mmghtbde.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvnrssgm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ivkpnxzz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3aybunrib.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zjisqjuj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3rvbqlpps.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3hvxspyur.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3glbplktl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3iqkfiyvc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dcryodkf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gtomgvbh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hymfjymn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3fsanvmxg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3jmyndiyi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3szisvapg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3muqctjzh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3vtgokkoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3asofoctw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gsrgewbk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3kubcuwrs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mkunkmyz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ewnvynpq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3xrfgbhxl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3almfsqce.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3cfdkldiw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3sgzvhfkq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3znfuxghy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3rvnqutwx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ngoaznoh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3wtsmkynw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xolcokbx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ttmbkvxc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3tfnedmpu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jrotblwa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hrbnezbp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3zmrdhgts.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3kumblsta.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tlbrgwds.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wxfovbnb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3mqxkpkdj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3guxyuzwe.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3siuuktxe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3kxltxvxm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qsxpshon.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fgbzalrm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3isktxggl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tkcfuvpj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eeugsjwt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bnzkhbid.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qzivavql.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3qmfuzyfq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3cezqhorl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tpdqvyyd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3wirxoket.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3mhisnccc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ykeavjwm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vktlvnuy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qqzsfwdk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3epgeuauc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3tazpgcgp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jcbznuqi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kctunbga.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3goglsijb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jxnekgbs.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3doilvfoi.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rltetbqg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gvswwhxd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3elgvaqrf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3dlqbmxje.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3botmzsxh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3lhpgxhuy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3oodgjnbb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3kobwfxgw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3zksfmlze.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mkhhearg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vxdijhyu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tsvlskkz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kszyvrsg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ewtinivg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3sgesjxzk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pqoloewo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3lwihahyt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pjdrvgzt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3wcdmggsp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ckipxxdk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3srbzyjbo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ilnnrfia.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3mjwfkynp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3pbwiqknf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zgwncktb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3eajrmnzs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hkliqwly.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3djneftlg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jtcjjebl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3rndayxag.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3zntuafyl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3agqsuydc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rswgwtxn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3afbyoshl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3sajedtda.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3lvjineob.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aforxqdy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cryakrfa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ksorhapj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wacydxnx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ldzaixuz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ycuggkae.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3dkwwobrz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rcmhexsa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mgzyrjec.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3olzcwhkl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3kqcmvgar.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3uedsjhym.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pmzhtoel.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3swpsdxvf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mbcmtbru.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3nlwngori.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3sidamwsa.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3jmxytocr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3enzokidm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ccuvymjw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qgfcvkhc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3gqgpebyp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aoysbkly.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qzqkrjkx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jqqyplct.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3wpeafipe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3bjxebnsv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3yjrtchwr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3piiriwuc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3guaydjeu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3dzbnjcnx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zkygkeuf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3oxldphch.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lizngnxk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ieefxdnh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3zmqjmpqe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3otkdazaq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wshbrhqv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lqikfwxr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gnlwgkdb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vmwqlyqt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ozatwowc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nnzkfgqs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3bmeljtpn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rikpwquv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hhstermw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zpiqdkqp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zqehqozc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3uvjmckne.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ebplkyve.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3nenduckb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3mjhzywqs.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dzptknru.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gpwmzknj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3onxexokv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oqopqilu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3naiqxifp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bqhuluei.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3geckqtpc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3bewmkywd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3dgnkfrav.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3yhrqlkgy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bbeobzuf.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ryqkhznr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cmurjauz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3bjsreflv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ftcbdpbz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ackoupfh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3uzhcchyk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3pjdgpaer.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3uuvvoupf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3okcsmxux.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3sosndpay.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3vvavmlmi.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3duslqkos.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3drdwyxli.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dmwljxom.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3knqxtglz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3alsvzikp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xtdtgeaq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hnysondx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3rjpbyfvi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nuuhbsfi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3flujxyob.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3avzdjevd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3aogybixc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3xhomsdsg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3vkofwtph.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3caukmdwq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3kmecrgnm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cfjfirzg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pensqjcb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hwkcnxtc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jzgzazra.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wmfqxvwf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3qhaztgfz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3oztkvipv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3iypvrtoh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3kwrfmffl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zrkfynhu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dxxqhdkl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zugklpxd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rijzrdcu.html


<!-- 参考信息 -->