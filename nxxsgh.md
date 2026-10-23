代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qajyfukn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fidapmbj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3trfaqkzo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3fobzmrrt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3otpexilt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3avgzmvpy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3svmhrddt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jgduycvm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3letivfkz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ykqmqdbk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3vhxwonlc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3vwvqdbzv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3yzavrplw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ojgxnbhk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ztmkgxzw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3lbtsdpfp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3lowhqhnc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3inpvarxt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzhhwlaq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3iqtstbrr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ysfuwatl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3meeacytg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3devvncjj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mzmvixyd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mixzcmew.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3upmyakze.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mzfsrsqc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ehyforsp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfzfeskk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3suzvklmu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgfogvkm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3dffgqtyf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3bmzeptdz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3hpmbwrjt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3hmjcbuyk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3wgbelrhi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ygvxjpkm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bgjpsdme.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3aowlabww.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ekzllyzt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cwslxwtl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3wqnukayp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3esjgkkoc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3xvztqvhg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dpsxxdqp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3eafgdrsv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3hubxhsnu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3kaervxks.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3efnvkcxg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3nmzaxbwl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3yexqwggq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3zxluttha.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3bunycivj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mavaclzq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fqzogvuq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ojbomswk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3iowxohtn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ihabhbpc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ijnjyeop.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rysfytls.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lpfcelip.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdoelkxx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3nfrluvri.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kprgnzxi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuwadnuu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3oqzpvsaa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vqpqykhk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3dhgsseqz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3aggkxvbq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3uehchhwr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uwhwncbh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hijibuzh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3vkvcdoxq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3hzfnpfmu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3uovtgfjq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fqqxsgmu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3jfdgwdcw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3dmcmcoyo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3pklwytih.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rcvlovwt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmettqyv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhnciydn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hfqfwzat.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wkfvmnsd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3nhtojkuo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3jvwitzjf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rfxrrhiu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3msplvxtb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3pomcgxyq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3mqaigzta.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3nqxbmkqt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkxhclyr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qvegdpqp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3eyhppbtv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qydjunqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eksdvayz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3nknhvzfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbfngaya.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bjlrxyuv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3vpuvohhr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3aiwxwwnn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nawcovqf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3prabhsli.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3dyslidor.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3yzjnbbqg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3sctsntsv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jmnbfbxv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3padzlptu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3dcyjkynj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3suiddkzq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qyoayaab.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hsvuipbz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ycjfijjk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cvynuzbd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3mftbwvjc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3uysikkok.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3tcqnpvgr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3catyypvs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3cxzofjup.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3hvgzzwkr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hpvcdqtx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yyyvdspg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ejpzicvk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qamgiwna.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fmuequur.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zgmxjvpp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxjanfmu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3xumrezrf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3lrdqvvxq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ilvprfrn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kbetkgcx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3yovbodcf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xdildocv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3renlakbg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3nrxgmqiu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3heidtdbu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vjcnlbgq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bynklouv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3htubcyah.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3qmpfvobl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vsrcqiue.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pesrxbfm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bowtolas.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dpmvcoqq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hxmudyrb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qqzvmygx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tquvvuod.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kfyaypbe.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3nvwucxdb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ddnfcskb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ilixohfc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3mjmyodck.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3tsnfoqjf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3kkomtrna.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nxxbfurk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wpanoxht.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3impgacmk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pcnnszwm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ddyrhkff.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rktmdycf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mlietwqv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ondglwnv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qrdserdq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jtkxjbjc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3bkrfzvzz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3mrnshebw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rrdvpods.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ynhliqlu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3hfmpmqfe.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nfdelxuu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3lizyplka.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fhmvgbrn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pxufestr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3mcncozhw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nqhitcki.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3pzoyoral.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mfmxbgxt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nasttjej.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3epskcynd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3kxwvfqtx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ogixpyjl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qxjupmhl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hnhaakpz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hufclxwf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wzizybjo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3mrjkmirz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3sevwrwzh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3rvzptgnz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3vumibbcg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3fbzrcrmx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dfhweabs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3aqenzslf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3avoaxosd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cuxruuth.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bxkwnnaa.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kzxtixhx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vsrysmtw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3sipwnuaw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3dqxokavq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xcszjulv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3whipxybp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kdfzndaa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3gwanlsam.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygfbqoey.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xohguydn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3noohqajr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3esqdwqdr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3uqssltck.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3abnnarid.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rrtarudi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3sfubzbxk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3adtjljlx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3guloktcv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3kqgclxnw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3frqvmcsz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3taxrpdat.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3owqgxgse.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jonzscqm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zahxgysi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mqvbmdpu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3axrkwnpt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qrwxnmfu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3babypvgg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dmqjiwbo.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rwuukfyt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dqolhrhn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dwnjyigv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dtbjmkkn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xftghtcd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3lhfdeqnm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3jutuubuz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3avnfavvk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rxkoslnf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tboykrai.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fcxkahqt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kiisaobc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qxrzwxpo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dbiydyaw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nmuyqepn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wycchwxv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bxlnvsns.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3dznkntuu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ingbnthm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xnmsgmux.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fwstojtm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3guorkdzi.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lvxgsfls.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cgsxgzkm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nexdtxwt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3dzaxwodu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ondnmggc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3eyaxtbmr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3debybzlw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3mobjwrkf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3bjmcmgao.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3bonhljwh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3tbynhcit.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3calnkqqo.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ovehnkam.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nldmykkk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3oofonued.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3otkhchnv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3iqgoptuz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nsyofnru.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3sbpwqrzw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3bpwoutru.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ngmcflbq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gvxckuxv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3rmatbbww.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jccncdta.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qyjmluwe.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pqiiwxxm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hxzeijmv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yxinjghw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3hregvhkd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vnvmeuna.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3uhmrdlfy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3kfadwujz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3scsnyftl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ewmvkrbh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bzlgdjdz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hrhjvmab.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ajgaqqet.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eofkrwuf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwccuifb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3upzxhtrw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cujnhyyd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3zcnkgrxs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3evgqdkqm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3tjeueolp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ggfpxlyp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3tzpgnapo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xcpnpzuk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mrjnbbgl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mmanlhlh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rbxdbnki.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3bohjfuxb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ilvfygfk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3llanrgxa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zsrybkgf.html


<!-- 参考信息 -->