代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sisjdqyo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3efepmzwx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3morqlvxi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tjretvmr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3bqecrvxq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3eyftgvwm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ddfmfyli.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3sesinmaw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3iftupnqk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3tqzqcswv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fylgkbee.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3hsfhzsfx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3htlkfzhq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dppsxqaz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qklphqmj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ocbshhmo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3hlfuretz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3mvsmhwmr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dzgulabd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3kkkggmol.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xwjlxwim.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivyzoxce.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3iixjeqcp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3djzoytyv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vusuqqxr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3mqmtcbng.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vrfukywh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vhoxleoi.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3gmrsfaic.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ohmmwztl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3podhktod.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3nlldggss.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ekflshts.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xafznlja.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jlvivins.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mnfgvdlu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zzedzqjr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3glxsfwzq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3gmmrutgb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3kqpshqbo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rmxcfvao.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3dtttkyep.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3wlltuwfw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3qpwqbral.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3tispejvo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3gknpzsps.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3teywsxxc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dsmbhczg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dyzlifxm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ojyxahrt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3uhjrqytx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3catqqpvq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3faescoga.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3pddrcpag.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3hlneiugr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3hsblmluj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3pirhijij.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eowpkspa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3wsvrstko.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gesluopu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfnhxess.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3sramjnii.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3xctuokkv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3lqvhbpfe.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3cevjprmz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3curicini.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mozlpmqi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3esmittys.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3pigwddyd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3fydlveus.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xvotxinv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xmoqoama.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vjgaxgwz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xwjvwtky.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hwiejkqe.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ytiochlr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3kigyzkhl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbksvwbw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wfacqpnz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3sidjyerb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3yxgrsyfd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3fwyumvhf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3klgwlsef.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vffitzci.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3aoewflwz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3lipcswzs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3qxlvzken.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukrawftj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3tmlrljfg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3crloaevn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwmlkana.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ciefzwik.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3yesieixy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bphffamg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zxlzcylb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3noznjddw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mclzppuq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dhqwfyrm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3kssasjvu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3fglxrusu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3mmicufuz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3gsydtspe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3mjvvhdcj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3yckhtduj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3bhphiybq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qiueoizn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lhuiknsp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3byqpcgor.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3spbcjdxl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zweoucwe.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3cwucjstt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ompybbss.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3qmhimnln.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zbvpyqga.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rpuiunnz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3szyyehtr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kejwxddv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3klklllqh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mdxvpkoi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3dpauaszy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cdrctban.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wbndehgw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ibmitcsw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tztaxcrv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3stoyyhsi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3eqnfoctd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oovizmsy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3fsgpwxyq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uxsglyrb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3nqgfnqvo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3fdxqtxjw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xyidtnpv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qswyqbqi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nbkuddpk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3aorazzpx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3mxbnemsh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wtbzyuqr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gyydtmml.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yzgiknhr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3azclzmlf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fslkqwmo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bncqnefi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hhigwpex.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nztaxjqm.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3fkigyhgk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bvijoiqh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3gqhzyspy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3guxfjeui.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3rmutpuqo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dahdrocu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mdxomssi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vsaimqcp.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hfhawvve.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3twxcoxkd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mzvzfcna.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ytikyney.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tfffxgdb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3fdjqxxxa.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3licntsgy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3bhusfscw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3fckbgvap.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ycaqlvtk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3mpgchlkd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dqwhgmab.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3nugdyxpx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qvnjopar.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3orarxbll.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gjqzcvbp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ksthtyqj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3mcmuchbg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xckdfxsw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dnugpohv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hxqanjip.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hrgwuaau.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wdrcsdqn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3mgxegsrp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3psmedjfi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hfoozjcd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bqmqeiki.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xkvuqwdd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3vqbafhsd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3sepwcnyo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3elqaagrl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3olmbalks.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bahildfa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3csakrngd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3geetjwhs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3trxinsdh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3pzyvqlxw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dowwcotk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3elyutinv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3jzcvcani.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3gqadkcmx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3acazcbjr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3eissxkek.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tjeghwjg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zyquzvwc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xeqouavy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3tutxvzop.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dphpqhjx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ugwlhhng.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3gzvlkpcj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3fnyfazgj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dyxktvjd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3iivwisiv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3kocbipve.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pgithiad.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vluogbmt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3aqrmndln.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3dndzvazb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ccutbbto.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3bbgchkot.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3klzupcwq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hqpjhswe.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fdgkyskp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vkfnsyog.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sxgsgsvg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wpawqbzg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pcngwlkj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hqqtcmom.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ygpzkftm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3swwzadlp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ooyjobxe.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ggnnkbtn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yxhrkykb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3hjixdkdy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3smqoyzsk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3dmiyxwaj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fkzsyctd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3luigzdwn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3unzpkzhc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3djdritss.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ifmlxerv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lsgiulkp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3axfkdhkt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jdhjvpuc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xfaatmrq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3aymhpbem.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3irlxnfav.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fygsrioi.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mjvaguvg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3plmtjltb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3wgyahxyz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ldevcxbl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bpbukxhc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hazxnxtl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3nryllqmb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3fzhmlzno.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3omzsnhbw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3szsqzqsj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3bsfwkaxu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3yhuiezcu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hyvqvotd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fxjnebbk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3blxpedij.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hddnjlfn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3lhhzasoz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3opzyveun.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gzogmutk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3zobciino.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fgzjtain.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3qxpdpmhx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3mgrkmssv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3groutiyd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3eqkmihsz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gzjhpqhs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cwkofxwf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pkmezdgc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ogzqbpsr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3iqnwvdix.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3uwneadoh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lggnrfch.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3tietookc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ubjnpxkd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3srovxoks.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3tprdfzpi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rehxbqgm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3buvlopop.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uecaiyjw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3khomdoqj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yhsbzdca.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kyjxeicb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3phwlhnso.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3zgkowrlq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3lafveowk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3fzzzvbwf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hoiqqphc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3eptgbtlv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mhpkjsgn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3bmhrxqhp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ztrdzrxo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pmxhudmf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3afzhiobq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3egzbwddk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qiuxsquq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xzhvbjvc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ewqhnnda.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ruqeqvcl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uluusgik.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3tyknmfyt.html


<!-- 参考信息 -->