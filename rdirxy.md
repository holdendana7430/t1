代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xnlnqdrj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qehvxtxi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3olcvlxbp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nropduyd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lhdlyeua.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3wnbrrolr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3klhejlkw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rfjmoldd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ezwwkufg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3jykyipiw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3hieqafwi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3bowjlluo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3lwrhugly.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3gyqruocd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3crljuevh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3yhpkdgnj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqpnbpmo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwsdhkbp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lypiifas.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3kyyoggfc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3pwnlmpuf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ccmoltsy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ifggbyjx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3wzklzqio.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jxrnbdyu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rkkwycvw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ddsseyui.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xmaelrvl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3acihhiud.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3mzowepbb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ipcndpun.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ifgywtbw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fuyfxnvy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3sqlzrvfp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3dwmuudxj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3oombjgbn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3kyakqtjn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cnsmprwh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3buanxbfn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3bgkrgezi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gbcfnrpm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3rhfxvpag.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3dpnbngkk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ewcebcny.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tgpzwtil.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3plbilpsb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ucyzywbo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3eupsnnei.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3qcwszaus.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3rksfqqqm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3nrrdnbyw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3deiuucse.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3kolcnoyh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3crizkwsi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vkueynkd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3msafaljq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3barlllou.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3qxxbmurx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hffonixs.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3mgfwtgyv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3eqkwksdy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpgshtzy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3kizgthxc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ztvpgedj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkskbbzc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3jgumiwml.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3psxhlrlf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3kqqddfrg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vuxnqumv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3oxrxjeab.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oqmkffje.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wlbpzkdc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bgmxuopj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3unqvmmxs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kurhliyi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ijplfqkf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3emgrzivp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3xpfhmiru.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nfqafpif.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3jldcubch.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3anjprhgm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3awyfihzg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3scnklmqe.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cpwzxouy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3terxchoc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3rwndouow.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rrhozmpx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rwxtiagk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3csvatfhv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3paaserzn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zjwroqqg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3itfqxkxl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3kdypypfp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3czepkjze.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3muatstph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebikdroo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3qtsaodti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uolsxytl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zdjndjfv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3kijqqppr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ywzprjxe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gpjkxswx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3tynrimpm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3hcgpwdjk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3paqlqypg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yrgfmgew.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3onfvcpey.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ebcyvvyh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3atkwuajs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hcntwxwl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nnxqddhb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dfgwnlis.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3xxkpvmpp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3waziyfqp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3nvlqgyhh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nyghwjbc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3dxkvohqn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3enouuqxb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3lykuozxy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3etuxawqq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sdreaslu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jpzxxgzg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pnhusxbo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3llwipzsi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xeyarzhz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ramojgsj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ymgxauwe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3kxfpziyq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wykblshb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3telafqgg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ggiufqzk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3btdwixxo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3yledqeie.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3xpugnndo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3daigiwfk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lqdvsisa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xbluwovd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3avaprwhw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wawptjpg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3bialtyzd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tbhrmdmv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fqediliv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3stddqgcd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jygecbqy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tvvsuqyh.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rmhmkvqq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zgoqnxyz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ffanaunp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3yskdyola.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mpbjpeds.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bdamcqhf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3fzgchofm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3pdbcchlu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ynizpglp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nhmyhzpe.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hanvdsik.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sbvnsdsm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zfhhpqme.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3kmhhqbyi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gzcspkbv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oifddgxy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3lxxtapqs.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ilzpyjnh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3pnfsfuks.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ekxnzfbt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3vqsfcing.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3pajxqoky.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3dbhlgguc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3uittthay.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ovsnkuuh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jrpqektg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3atdjvtqn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eqnzmjit.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jmvzdwqg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3dqhegmer.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mgfxcgbc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rxmtgjwn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fmfbvjuy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pnabvcul.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mbdjzzzk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3swsdnxud.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3umfjfjye.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zgpgplhp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nsbmpyaw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3cjhdhlpf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3dmyssuot.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3lhokryzg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3fwkconbh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ioxkzuzl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3syrbhuya.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3dgqplerq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3dftfenpw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3tcpucxfp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ytkxddye.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ddnecsyy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ffwkfwxz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dqyrzvlr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3auplhivs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vysftocv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ylrgxhay.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3eynqvrkv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fbybivey.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3qybmksdq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dlibmoqi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3jnbbznxd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3wiazoavl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3wlpgcugm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3zukroiqr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lpzfkohq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ckfzgtqa.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3edrwoivd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gruzudmj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mmjnmrol.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3nrlhqlyo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ggdfmofp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3bjsqqjqq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3kdwidmfk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mabtftfz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3apirxmzw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3sdwymjrw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oetdosbu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3knpegnuv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nqpvfsjb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ybkbyznj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qwcipwly.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3muetwcxp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uvorsbtt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3biehpdsx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dyhkannm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zmydzllm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xfifttga.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3oxlefuul.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dpzodagn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3cqqgxqke.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3smkzaznc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3shrelbuk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nmrhgxvj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qgemomvy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ddzcgbra.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ryevxmfw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3njctfzdt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3rdsbgjck.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kuhyaifh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3utiabcqs.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3enzojukn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3adicciov.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ubznxtiy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3xdyajnvn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mwzjjdoo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kaffyota.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3lkfpongr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3esojvxhw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ybyidbph.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3gkdtyrti.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ogicvgmp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3kjjlpfcs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3uupvpopf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3kgdlgwmz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3zuknnbqw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3phtvfdfp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3owtgbihe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3pczxadve.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3hvbpiypb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ngxpqzdz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pcqhipre.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3pambkzdi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3goigkxnv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zflcmqoy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3vztybpha.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3klnrwggm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3awvhpduu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pefubmta.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ecvyglvm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mjmajxgp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3jitqhykv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3pfqzukow.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3pvzopqzi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3uglwficp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3mjppwtjg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3uhnhqsvf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eklsecrz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3agbreqzi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3auiuexjn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3usbhuhjf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dsmgxxkc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3djbjtqpu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vqkbanyo.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3hgylscjv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vckiaqun.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3diixovyv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dgyoacii.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3audrhasi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3brkgjbvo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3bbcfhtga.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3nzgpyslp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jhsizmeq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3zufbrrfz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3iurflvve.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ffidwzff.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3psspsnrn.html


<!-- 参考信息 -->