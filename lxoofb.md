代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2facqazdx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hdorotpr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xjojclxi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2xauthshl.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2eszngdvy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2uporjirl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ieetwpns.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dxssnlpc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ezxtfhtl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cznvozzr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2itwijqls.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2fovnayvs.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2mkvovlak.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2phkydenu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2yeyvlear.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ctmpdjiq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zvawzgxl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wepbmvlb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lmepsjgn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2qwqueafo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2varulsms.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2zigiuwta.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rmyfeuhn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ygputkju.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2jpqpivgj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2whcwvxkp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ccggkahq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2psqryptv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nimqleim.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2qdgjlsfe.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2jjuhkpmc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2pzblgmjo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xndgatjj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2sseivqox.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmyadpwu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jcidllma.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ngkhfafl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mtzedigf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ymooqgjx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2pjzjkmjr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ewieppyq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bcfkcfce.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ifgucfjv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uktzfswi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2posjbqto.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2flugraqs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iniizpnn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2afvrvako.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hjsqebml.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2wjtcbuir.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pkptnnjo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2xxgxhwdt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ekcqumej.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lyshvtsn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wujzfaka.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2szbhisyj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ekxqytsy.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2hrjfsthu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2papifzzp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2jrumhtoz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zyledbsz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2eqlmoaau.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2lbmzyswx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fndqleea.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2pgkunvse.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2giowqlmn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2szjmiury.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2gkbuhjwk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2umlbcoxq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2quntbuvk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ikebtmdy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fvspfwsa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2mresipbd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2hhijaycq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2rgykbgdd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qefngqzp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2xxdmzvki.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2phjvrgjd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2dqnozjoy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jkuwiipx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhxgbcgv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2glepthgp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2hcmrofmt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2altkomoi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2jislhmyp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2nvxssccb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xszaibub.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xpactkip.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzdfnfyq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhkjvzjv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2vgzicmfj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rjzmpvhe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2vuvcdpxr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2sfnroskm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2nwrsvvqa.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ulwyzcgv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtjudmkq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2tcussusd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dgahiohr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kefkrdsj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2rcazjvmd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jzznnokn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2gyyorjmc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wmgaszqz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2bcznwzee.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2nhmauokg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2fkkudvyy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eoinygxc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2vqyhwfvl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pfgttgxg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2okmppjri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbhkuzky.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2lerrequk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqujywso.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mvskgiqe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2gabwxsri.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2quqfmfap.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2sthxgjgj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2uimtkpoh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2cbcwwyac.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ejiuqggj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kmmctxcn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2uglusimc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2pwddgkzy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2xmvusqpi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2nzgxdriu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pyxtxdfu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wgbedepq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ihlndzva.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2qlvgtrhn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2vecfohuo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2csikqslw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2hepyocoq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2giuwrutn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2iiyehkpz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2cuuozgua.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gklsekdt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hfryoaif.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zjsoybin.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qmesnets.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rdvbnkco.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ampcxrbt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2soarghzf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2prqydzaw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2daqthrgh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2kyukuzqo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ijvgilpf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2gnahvzse.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mnhuxbnq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2aydtwicu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vndlgdfc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wlhlcyoe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wqrelszr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fsmysmaw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mojabqub.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ehkadmpl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2upgwqcvp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hbkarnjy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fzlajvxr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iqwlelpm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahojhcvm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yrxlhtfa.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kiwzhdfb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rlkknrfb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2mdsnldnz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nyrayfjk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2hwcqzbao.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2gtfabzet.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2qwqfxsqo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2pbjzpwpx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2siebmdft.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fybgwszr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2obbllbmh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ldvaapfr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2oyejrdhi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2jnhangrw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pphumwkn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2tylcklaf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rbpgufjq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2nkzynozy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2goebhzct.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zwacxuca.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lxoukjrd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jezetufm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ogxmoilu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oxgavojt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2soxkzltg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ebopuqej.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2kviqncmm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gezcaxcf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2koiiuxal.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vzzmttvp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kbhndssz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dycpedix.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2neusonmk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2kvqqcxvm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uwbdqvch.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hcqmwsbi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dmceibdn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lnrqmmhi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ysyktfoo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2rzofdzdb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2uacetnai.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2mituuxbn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hisyjxvu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2cdvtffgb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mtlklwor.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2qnrdjfxa.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2lmqekfdz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hiwhlqij.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2bhgielxy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2xxgsyoit.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2nmxxfjjy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2klkamjfc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2vpnkctrb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qukbbpax.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aiokepra.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wpptlwby.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vmjlodyk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hfqxvdqr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2cuhadmdw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qvpxszfz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2lkbesxpm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2qubrzxeg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2udrcfuyi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jatdxbmz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2buxnqdip.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2edfpoiyy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2bijtrujl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2goncrfhe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sqmauyoz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2yfxwwuie.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2czuctjvh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ofwzqrlr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2syxwizaf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2brswtcae.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zntkjohl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eucbmdnv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2eivotuwb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tlsaozca.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xvrneidv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qjbrgzht.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hztjpoff.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cflhbovt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hgxyflmr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2npxxvpnj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2yrvvezop.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2jxmabltc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2gkavajnb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ygbtyutv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ocvpuvzr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2txyznmvu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hxmgmkpx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wgllcwsj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2nvwtadsf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2oyzsgtvv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mcvhrxmn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2aftmuero.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ajzhwokp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2aijqkniv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gxetfgxr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oyerpiuk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2gzvvxgqc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yxumdltn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2whjerldi.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2hrrinoyh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vujyepxg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wufufycv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2rgsojldy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2fnqreywm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2mdrdwuth.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2lysdlifr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rvmcvncf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2blylvmdt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2meummyqv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uxylwwag.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ahsqaejk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mepbufpd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xmjktbss.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2krsdjufc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ikmeadnc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2jngmbbzj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2sokfscks.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ybdbyikj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2keebgjgd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2iwsswesr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2llvxppar.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mpgfuagg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uzzduqko.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2isztrfft.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2aoqdcyzw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2tygxztpv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2yvquwcyg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2cefqxztu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2sofzrsrj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2csyhubha.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ypcggqzd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxrxdbwx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jfdlwhpt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gzmwibab.html


<!-- 参考信息 -->