代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3qyctrlwu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yodexbey.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fidzqltm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3kwptcqeq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3nbrdvmiq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gokzzwyr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yhqgxsyy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ahkormku.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zpijoaak.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3hmizopcb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hqmqeopu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cpkrywcv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3hbrrqwth.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pereoepf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3pcjsnfmr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ezxudamz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3bungocno.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3iydsmdbi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3uqzoheiz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pljpjoua.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ptmakutg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3xbifstzj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ppgpktjg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3taljuvta.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3syhugapl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3hlgvwytd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3wdkemdpm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3latdpbkw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3fzjtdcob.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3fqkowtqt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sfdwrozn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3qlztlvdz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ulytgyru.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mtvtiidb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3yerkpnbn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3sudcpzbd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3truosjjr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nqisdcxf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ffxhtzak.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xfbeosft.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3fyehvlkl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3sgdtctxm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gatqfgmj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3trpyouct.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3tmkrfuki.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mzgqmiwz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3prltrjst.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3eyshothg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynxuachz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xmnnhxem.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xjfnyado.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3uredytak.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lluvaluz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3uakontyj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3nhnbufri.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3itmtmhmc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3fyljhzov.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vrqlrwwu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tqpgnvxk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ybrfsagt.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3aipmjnud.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fmpfaxbs.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3jrjskypz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3reyrsmot.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3sfgfyfrv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3rrczdhgf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3hetyzqja.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gvcqdutk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gvlvjsjq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3vxndlepw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zwickgyl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3wqmqmpdg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lfinyvoh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nowvfvsk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3okeksksm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3raznmlwi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3uwgysnzd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3sckuznir.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rqkrhypz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3uxesyzcp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rhyugvhi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3thenmstt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3yueefayv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrwhuakm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hwxerqtf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3xvoxljdb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3bomqaaze.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3yyexaycm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3mtixlwem.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3szpsllfo.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qpcohutf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qxvfxypv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wkzjptdv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3edpivlpu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3sunldfcp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qaftooad.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3onkduckp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ovifaysq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3oqytervz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3htxzkbbd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mevblxym.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssxvsygt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ejmtuxgu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3daimbsgs.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3riozdrtz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zelzghgf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3uzasqmfs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3adyemuzo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3wiqrrayd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jlyqmntc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cbkijmrt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhqsqzfj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3whjgcxiy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3clanqcka.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmqagkhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpgkhgvb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3dfcnnbdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzgfxajp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cgeznysc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3bdnlemlv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fxdbhoes.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3dxzwugod.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3thupmmkg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3rrdupnxh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3lussmisz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zjhjmmpm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3hjimcgnj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3sktuhnem.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3dhvkqwtx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3rdnmqdvf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3etwnwhnh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xxguyhxw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3huwejsmy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uujjfxye.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ealbpnoz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ikmitgwh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3rzyacpdu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pdjbkkiw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3prfrbdmp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ihvdataq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3trvkxoga.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hudxwyan.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cpaumgfv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3wgvoeewb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3brjmwycr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3quuqhkjv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dsfeuszh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3xthfjebx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3muudntnl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3zrozpolt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3oijyehit.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ygyxehik.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xquubxyl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3uplyjrlv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3qshkheon.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bujvogcy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xomjwxge.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3idrkdqsh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3wjbeykkb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3stqttopx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zlkhdlzq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3egzrwqfo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jzsikcha.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3duzjyxvk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gefykhqa.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nasasiar.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3seeefqsc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3oepmtisa.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3mtewefuw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cdtatmzn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kcxsazeh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3dtdgvcoa.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3rcymdkpa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3asqksoha.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3sjzxhcvf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3veezdcgm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wopaboba.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uebekzkh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ikkzfwyx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3skqkewfj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zdtwvson.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3skofzume.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nrnqgcnz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3dulvozuo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ysyslmbv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3bzmvlcjq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ivvssrcj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3hnrplxhc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mikfwmum.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kxzryiaf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3sbooyxuv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pbqhltnu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cxwidedu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3mfvvcawu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3rghvppdh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3nmowhoah.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3favlnqha.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3iecduqpi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3geiuxiom.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3eaqdcscs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cubonhbl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tikkpwbb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3aruvtshl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vwaouhko.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3tiwbaidz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rvbsijfp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tjymaztt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3gztfpzlu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3fdnsapxf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3qhjhbynk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ivpbnqbu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qkuwgtzw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3lbeokqpx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nkbqpfhf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3wxhrvkjy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kwysbnhr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3thnhhyff.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3uhiizahs.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3pzkhoolp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bntoqahp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yzsznttp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qfbvajje.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ydkqstdw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3igovlkff.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qtyfcvkf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3zkbpaltr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3yhumhrar.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ohellcwu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3apzeaauc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wmkqenpx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xpafxoiu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rrcypvqd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3juomiemu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3bbhxpube.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uzxpelwk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hnwljdky.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xfepqkrz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mcpftpzr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vxvsuvsn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fqyvavur.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3xlrmxhjl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xtvewybg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rslbygfk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oywzwdnn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3yngrmqvu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3coylmxte.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xgmhqfqx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bmcqdbbd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3imlbboio.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wqivhqpn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3aduehbqo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3bmfflvhn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sxeydhge.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3siedrfsl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cepvhmlf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oqzyohgz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tvbuefwm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tipjpyvo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3swprtxzt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3fhrkehny.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mpfcqasm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ildsbrvi.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hdiuodiw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3haedzxlh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3cztqxhbm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zpmfyich.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ztkwjmle.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3bcolrpdg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tebheqrn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jkqtjfgx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3lbgeicsi.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xtwizbae.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3slhcgqaf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3lbkxljra.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3gsyhjorn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zmrdyhdz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bxmlqhyb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fibeybak.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3vlxmytds.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ojirbjhr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3jmtoiwff.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3bskngjxj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3drarmaqx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3vgrrqnla.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qoyxzuut.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ywnfutik.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3tmlhuxvv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3jlqfeovz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3iosbyzpf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3admagxky.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ovjjqosh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hwdvgmlp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gmwvljnu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bwwfysnu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pndsbakp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ickhscos.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zdlzmlmk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ybnetujg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3shbdhrwl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3aendsktr.html


<!-- 参考信息 -->