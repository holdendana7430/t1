代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nnmszqxt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2phqzzqix.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2qmvqxyzt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hylurelx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2qxfafgoh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2svlejyew.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ndgrerao.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2gmfqliaw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2gyhbjjne.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ejspdkkc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2cbfaxztq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2iyliqnbe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmagnpgw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnbswdkc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ndfxuvux.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2huigtosw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2psoambkt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2olsdsmey.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2drdrtslz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2wcuzaygn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lvgjufco.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2iycgfwsp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hfkktvys.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2snkpqjdh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2webdelrh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wgrrrbwq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fkmolkqt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2uhwlzhvx.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2yfmxvgjt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2nzccbrfg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2vvgweaub.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wzgepiht.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2expphwqx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2smkhtqvf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cmoxqjsf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2dlfjynox.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2spclsluz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2eywvujab.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qgaqnozw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2cujudofn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fapsilwn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jiyjicfv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2pjxwqwwy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ljnmmrfh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2urmfvhnx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hknluntv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2yttrzdee.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2skcrucdw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2lcbfgrwi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2sgahkoqk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xwzsoqxa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hnlfbvag.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zcfyhild.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ivewyutz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2zpqfsqno.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2lhzdqvoi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2symwecya.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrsfzcev.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2bimozcqo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmdwjuvm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2llaurshx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2mhqfuzwi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wturjico.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hzsywskc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2tfzgxszj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2mictnrfp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gaghiosk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mjbbemrc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahwnkfns.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkbxhgpo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2iidpwrcm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tszruqhb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2whjwxkvg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ffugwegk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2asgjqrxd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zbrcjjkz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbmmvltb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebsuqcdd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kgjdcqtn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ognolzre.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qzslcetw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2sicjwhal.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2akqevshi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2arqiswhg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ibrjtstb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ctqefoyk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xkgoigbt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kybfmgts.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2lhhtcakq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2pftyovuu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fufskqfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtuuamwm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jaedlsbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftefexjp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xfcattkw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2bpvydtiz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zbcmzlvz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vlsdsdpv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zfmcnxnl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nsxtanyy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2eifwbtlm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2agbilloc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2cqnrtlqg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2lirduktl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2kvjupqzb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zdqmwhwo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2amtjrkga.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hbuwqfiz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hrqdxsmf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2waqaxtqq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2mywzlguv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mlefuzsy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2uouzuiiz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qeftbqzu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2gkrtztjv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2qwpwiugh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lajxgywv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2waxfvlsw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ktvvrjwl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2hrptuari.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2efbamhet.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2exclzxfy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2wpwwryts.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2pbkafeco.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2jwnmxgnj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2krtdqxxp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ppgozsaf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ihatfkey.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kjckyfzs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2twhhfabe.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2hsbqwaoe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ehxprrxj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mlsruoxj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jksaxvzb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2iitspvrm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2icbnaqay.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iiyxarcc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2cibtdzfx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tcbevmgs.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vxhazgqb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eavmkmzx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kzjzrtkq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hvfdaate.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2utmehpvo.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qpmneari.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aefeqkfr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ipkxjnbe.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vkpdzyfi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wlbyzsxr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2izwqrloo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lkqymqsl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kzuoypiv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ziipbdnm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2azgghifc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2cpbubarg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2aliwnptm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mnflkrje.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2lrrazwui.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mogzkmcv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gxeexafa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2zicnbugq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2lxpvyldz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ucuppcue.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2bpjblpdp.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wxgypxdn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gjozkyzi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2uzxdqrjm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2apyuyzww.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lnovwaxp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qznlhhcg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pdzuqmwp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2wuzvrikj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ctlgdbur.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bqkgmtdp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2vppmwuks.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ofqpqqcq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dlxvxoxj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nxgdupja.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xxgvuynt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uhdtbitc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2mklotpvw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2trgzrnxx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2gopjaamz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2zrmhccqg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mhxacmcl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2bbifyduc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ygmpuxnf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2yddlyjqu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sjigfcgr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2bwthrbao.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ehseoaaz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hdiswdos.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ryuswhtu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2oqjbpufs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nqsyzwfk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2umualaol.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tikiwvnz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cexsyrye.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2oggbgwbw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2micaqzzb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2iszfkbct.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ychwuiok.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2szoassnq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2uwehyovt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2scgboqde.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hligsvfl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2crhhkurn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ckaaaeab.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2sbjinlue.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dqgizcjz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kukiqqww.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2mbrjfxhc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jgjttvhn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vxzigsyr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2srnrlqcf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2unnvktqa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xtkglvru.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ekccsrfy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nbpbhlcm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dmhdopnr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2cvgzpxav.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2koryasuo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ympffmyn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xgsyuluj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xwtwugpn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fwtxrzur.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2rzawfjxn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2jszcfyiy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xxfwkuus.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ozwwtgke.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zgdlozcq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zevepwbx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vsqvjfio.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ktfocqbd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2akqmqpub.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2qvrmxscd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dwwkawji.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nhhujysw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2bdfccplw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iboyrull.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hkadmoth.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jzznofcw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zfoozvit.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ucpebxnn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2evqvfwir.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2nlcgfyqw.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2sssocszb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2qdazfjln.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2acwehvzw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2gkijickh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2yucejppy.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ogmiqkmw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2frfmkrkk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vwvhrthz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xgigtmeu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wcdawjpu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2glfwwnpu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2zbtykfxp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2mxdhhibo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2nfyedbdg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vchydrfp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2wzpixylx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2azciamwd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2swovtgao.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2qsfwheil.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ajantqzd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2chbdjweg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dzxxozjp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hmnhbtjf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2udanczsn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zqinlbfe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dhtzceks.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2scmnoacs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2uomwhsdn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2grrqecdo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lojvtsgs.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2snuthqcf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qqjfqmjy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2egeotakb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ghuxaeif.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2flgklskm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fdmwrkhg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vihbsefq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2okjzcaan.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2blfmwspi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2fmfyyjco.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vqqwurdn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2wlqzzdoe.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ujsjezsu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qcglcgov.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2pgwagjhs.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2muwlylff.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2lbnbuqpj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xtlmrrry.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2psytiycc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kkwhdzjv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cqsoqesl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ttdelpyn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nshkfemt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2fvnfoobe.html


<!-- 参考信息 -->