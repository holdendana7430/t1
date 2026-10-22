代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pdyefpuo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2plqnujmq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ougbpics.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dcmbprkj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2gxpbrcoo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2tvkicele.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dhhpsljv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2rqenokeh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ydodlgnr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2yrzvocuf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pfzldfww.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2iebsefto.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2rwdlzxmf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iipyvxgw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2picojcov.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2afuiswvs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2nibltssr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2fsqzgiaa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nudnnlzn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2asavntwm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qchswbge.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zztioqqy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mkrbplgx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ehvvabph.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2uookwmxc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2zmuizayf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ryeuhazb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sqwfuioi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ldnscfwt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2akodzauf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2zyejahhr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gljujhtz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2mdvclrlh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jfszgyjx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sralkcwb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2gvjgbbpo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2feyfwkvu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2wfwhaurd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jzvldyfo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2yehmmajq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fydpnbue.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2gorbxyrh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2gaivslks.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2szdqwdcs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2rbdfsbpl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2onpcxgxi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2evmmzpsl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wvfgzsrw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pboruqku.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bcscohwp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tlbcvvnk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2zgkdwvib.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wljksrzc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hfmgfsuj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2yuzwalcy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2yprdance.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jkkbdseu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2adzefkul.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jeamwgos.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhhyxaha.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivkzteqi.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2wpuecbic.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2jndiyawi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2boizszgp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2qfjxehbt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2zgdutcbw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hbdijrnq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2itlmpruw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2radufbha.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2khgehxkr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zeqswjcg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ihcdaeav.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wymzdcor.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2yqlqsmst.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2hbwpfnpr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kbeoxdjy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uczwbhlk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqfbbhrv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wgpjflfk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2sjzcaceq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2zqbjfptu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qwuowrqa.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vhhzugoc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ylygvcph.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2zvtddfrb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2kgccodwm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2bvsjqnry.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ednjogzs.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ywbwhzbd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2bgqkfnex.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2llmyboml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gygaprpo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kcjaucsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xksxrjsa.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2csvykpsu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tdrpbftl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fnknfqfz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ukoqrqye.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2mfikskfl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2birfhywp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tezgpwev.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ltmztfdw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tlzodbim.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2obybiltj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ezsxxlcc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fywuyzwl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2noeegozj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2sjrbnnjb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lklvayok.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2lebajjjs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2fxakainm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2pzuhvvca.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qogflrsm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xivrmeue.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2azigbzub.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2yiiddhkm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ofbmzxrq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2iusgbbsi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2chuimmic.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2kasvunhk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pbyvitbj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2fvcmjvpo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oubxumtg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qtjammlu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2nobugzsr.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lxeknzbp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2zfuaecio.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2fipjipxh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2nfelpwpu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2pykxtfdu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2setuevwm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oggwrgmm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hojrexdg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cmwuurqm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xxbjfzhj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2cprgjfoi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gwlfjwfj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iwidlyim.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ytfndkmd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dhhoyuzu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vxvhtonu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zoijtgzf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fejezuto.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2uvfytqar.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2uhgunezb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2frygdzfo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tpfntnlz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2qolwwzon.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2cejjhjdn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2pskavylv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dncggsnj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hldmstjd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2iuvpxwzt.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uwmjfkrt.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2pbxxphfp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dgcgkpgo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ujfoxcaq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2rocuchzk.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dnddnbah.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mcoatyfv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2llppsqpn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2gtprgcfb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2zcwxeytu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2fsijffrn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2meqhbizn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nkclyjzr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2svikqtrt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ptjflmha.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2nrszltpk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2zgimabqo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2iuovkwjc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2onewjzua.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ckzderyy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qfbipqnz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ggnvnkve.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2hwkgjihq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ibasiygg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ucnottyi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2znngpclg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gbprwdwc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2uabxseip.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ylkigavc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2klvjuduu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2glqnmlee.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2duxnnkbp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2uwmiqiow.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2yaqjuzdi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rkekpewy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2aqusatun.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2bpiobrfk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qabuxjfz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cugxyyon.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vtqgyfim.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2besbqgvd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yvksrxwj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ruqxrqhi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wjsqfgvz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ywdnwwqn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2atdbbahd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hkndbusm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bheaobmj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2otmciwpz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2tuwkwutw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jzmziowe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mzygqlcm.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qndhtbro.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2uzjxnqns.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2glyoqjla.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2qsslqbus.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2cnpwlowf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ifzvjjva.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ximglsss.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2yhfszhzg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yfrvikyi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yevkgctr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yrvybgcl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2szxvcccy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eyesetfb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2emezulbs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hxrqreid.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2qcjsrhul.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sirkphmh.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jdjwfttu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2thdvggql.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2obbjtebn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2lluljwlw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2wqcevwij.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kkcpolrs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2maowabzw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2hangoogd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bjmyqbdo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ytwjobpm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uddbudwk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vfxyahhq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qrsrvvse.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xoqgdlns.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2iwtjkcal.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2nhbfuyzu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dkfxzkeo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kburqiqv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ypjehpxe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ioqwifmh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eykrahhy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ltrynhbj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mdbirfwb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2mszlhebo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2befuzsni.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2anffgvri.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ygpnzkdp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wklnmrjz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2rurbupmy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2idyeavpq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2jcjvhfhe.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2frtkfsoj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2cjbbywol.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2smbgsulv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2zhydnrhy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2nhxrblfl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2atbnmadb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ufjewggr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wfzdxrqv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xykkfpki.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2pybrnlmf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2uosgwznk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2zfuymrak.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2shmppyky.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gcbxrnpq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lhzagkva.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jeivctrl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wrughiiy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2qsbaebcv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2fstqpnna.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2swvwdqda.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2kojjtvrf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rurtcyfs.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2qfzghsyi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qkswlsur.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oohcrugq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2koxuszzb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kduurwaa.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdbrcqsi.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bnqklqbj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bcecyasg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2clnpoofi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ypdnkuyq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2inrzvhdt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fkotnbss.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2vqndoapd.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2sezghgzm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kwgxvkcu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2rzedlgdn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2isvsnzkl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ajhsxzks.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tiotoymw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zidgnwpp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yslgugob.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xzgvprer.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2mryhswgl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ckppfrpx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2blhhrlvf.html


<!-- 参考信息 -->