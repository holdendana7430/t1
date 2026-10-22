代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dmifjalf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2zfiisily.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cvgznljr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2xpndajfa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rwknjkur.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ipslcfme.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2bsjfjcqg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ipjrdlck.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2yzcfgneg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2llcyltxi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hyjaivbj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2iqqxfssd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2dxxvibbq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2rfrmeotr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2suojmyac.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2qgbtvqri.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdesscbw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wyyqyaiu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kitqmcfn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2pgmyfzcn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qkkakzza.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2grchdosy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulbqchgs.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2jwebabwu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vbiqhvqf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2psgahcpu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hcdxotuk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dboolygx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbyzikwk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xitzktkl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ehhjnwht.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ukhtzgkc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xkmauerl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2wsiuhefa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2elctslek.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2vtfplvvr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2csmajzou.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hxsusqjd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2imdjzbzl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2bwcigsae.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yvlnmrds.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2awsuxano.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2urcnooua.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2lciakzjl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2krggzrpw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2lrmuvekx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2pgfdruyr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2cbqyyrmr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2fphaiuka.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vgaywshv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2oryknbdn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2nrsnxasb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ydhodgtx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kisdnvid.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xadolafv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2isnamrmq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2gcihryge.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2cjvffxkw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmikbxeo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2xmwtayjc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2vnsfeggt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rmtuqjar.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2khfqbkqb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ockflgzo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vygunsmk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2hwhdvqko.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2cthbpkuf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2blznhtjn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2kxckzisu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ghapwcjv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mpkinaet.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jtlnbkav.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjtryrut.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2qnklevct.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ttzssyuf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lzumgqqh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wbxrseot.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2yzeqioww.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ddkqaodz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2puofsvxt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vzznptum.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxecvjch.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2olnunoco.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2aytvwuuf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2lcbutwkj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nzzevgfd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2mcpbknkb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nrhwspdr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2fgfygouf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ywyfmnfy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2pqtmktcc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hcypojjy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ryvmpshh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ourwpdrg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjcumtii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szazmhdu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kdcljajz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aokzfwsh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kanymvcc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2bxcivsxs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gvjentqw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2evskhnmp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ozkjirlz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vrjfhuiw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qtntbmgs.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xaipylgz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2sjmamxqe.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kcicfbxc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2lkfwhdrr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2uetqrrgk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xnujnrmo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vvsnxtjv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2cwwpleey.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2tpxfqhtz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kjqrktdy.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2yurzpxxo.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2aozwnutl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cpblabcp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2gttaamgm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2wrjwmjcv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yfrtebha.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bvvussii.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rxvsxipo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2zhafoqzb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gbmlligk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rgrkshkm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xakacjuv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qxouswhn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2pfrevyza.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tkfwisdj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2uyftvzqx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2nrmkbffa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2syaogohb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2gqmopfju.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2uywmuruy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bjjqvzqr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fnxzdlhk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uijnqlxv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ojhammwk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ztrjvdym.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wmztowyx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ynevmlzn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pkuhlvde.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vzxrpvng.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sopssmub.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yshncrwj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xbuzghms.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ccycrres.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ffvzagtm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2oiwmyosp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kyinbqpb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2sswmmqli.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jxhrifit.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2mfctxmyt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ofpvfoce.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2umtonwpx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lalcelcm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ahvxpkft.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ngheoxqo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2odhflyzr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pkosnxyq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2lgsjnjso.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aqwoniym.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jykfvede.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2cvelfzat.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2zrefcvta.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2whvkgobs.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2pupljlog.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lnlpggwk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hawldvlf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zskaphpz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lbllqlkt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2veulnpry.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ggpaolzt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2yovolnsz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dfvkicwr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wvlfqmax.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kodosnay.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2jkzekxgx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2kykvmgpv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2yxcgzgou.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2knssgobm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kuqsdexe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qrkacrmo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2zdruefqp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2zynogmoe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2hhbokdxv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kcixgewn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2pprdieqq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2bxzxhmuh.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ujiylrmx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2phlixxqm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2hlbznapb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wsujspca.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ueqqyuzh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2adybmsun.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2yucabqce.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ewxxsebq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2tpddpzyd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2newyqnyl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ojuqclvr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qmrkqchb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2kljsmawg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dqdhsupq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifmmxpfz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2zkzkrzsr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rleolcae.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hbrriwao.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2tlsfvlpx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mhdaqeij.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wiofjgcy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aygppcsn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ekukyctn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2pwzrlras.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rcgemkfr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ehxrdsbx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2esctzejy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fvqqtuie.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgquulaf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2djcfvgqw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2nxggbvnf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vqvuzxdi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tncterqp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zpxnyxhc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nqoutnoa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dauqlnxx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jkpfksau.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hgugjscp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rotbbijz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2lqsbdqpm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ektafoqm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2swchrnao.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bxdqnxyk.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2brjnlbuq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2teahmjiw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gvqsxnqx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jadjlvlp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2osbczofn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2lylgyctv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2qcgsegdr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ewjbmrrb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2owwrhuju.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2hcdckyya.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hkhjjgxf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wgnjxhse.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vafnyxik.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mvczbfje.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gkulxfcr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2eqxhwxug.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kqgndbih.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2voglamio.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2vptjvudk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2guledcbw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2pgwznacz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2npqksvoy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2jymigfii.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uqehvfpk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2uaipwpnv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2dopzkcdh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uygcthwr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2nbdpldfc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mzrgmesm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2omioxjtt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ovpsthtd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bfuowmeo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tkvivfkh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2bsnmeute.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ivlrvczc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rlicxgra.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2iyfnvwjz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2gmemkery.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hclmxumi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2drnxaxcg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vwtgnsbz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2nufekizr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rmkrczfj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nuvzmhnn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vzmsxyie.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2lmsgmdto.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ikjyvllh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dutkqfcc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2skrlabox.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zaliodwu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jdmwxbom.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2riwzdfml.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjvxbjjc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zwfvtuoj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2svntqcqj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ytahrsuu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ypfzlnwi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lmnnmbgk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2itcokdoj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vojehikg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kqbwbumf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2boqfbdzk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uuyeutnw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ifdebxcy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ybntgbrz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2uycibzsw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ujuyoodu.html


<!-- 参考信息 -->