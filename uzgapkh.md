代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/ggdtvraaf.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gvznozinr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gqlwvobqa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gnmcsdtom.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gnmieathi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/glurargdn.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gedfeywmh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/ggnucpwpx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gpruxweum.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gqfstzbta.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gvxoldvxw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gvvheqhsc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gysewpbul.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gsmjupfcv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gmuxavbzj.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/grqpcwzss.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gduqzzror.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/glfsirayq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gmpgcomlc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/ghgekniws.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/ghcdasyiw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gscvpxfzg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/ghzdsgbih.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gwxxehkxx.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gwonxjcct.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/giidmqciz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/guqgysiqc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gzxljhsum.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gqvssplcy.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gramutaic.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gzloffqer.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gtryzpvqk.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gofciajar.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gaiwkyszz.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gytjqakke.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gmcmdnihk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/ggrtietwu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gmshzcelj.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gewkqogia.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gcrhdrzzt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gdrdhiykf.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gqowxboke.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/goubbtspg.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gexmvlaas.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gtuxdbpii.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gkltgpspj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/giknyifqb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gdskdbebx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/guqbmttno.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gywjrtzll.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gkevcnxqs.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gvgklnpxf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gnowzzngn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gvpayhzjo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gqgeeyvil.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gdvceukej.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gspymykby.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gqilbjtys.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gqdsuipww.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/glhlzwiri.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gcjjlrypv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gdztxnlcf.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gotjfnsls.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gomrbzcrt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gxnhbzqts.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gkbeeodeo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gzyszypct.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gqljwovky.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gydrfydpz.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gsoavdxsm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gmoqdjkov.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gjfzvsuip.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gihlnpdzh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gfhdzwzqk.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gufberhco.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gyhxexdlp.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gfmgowtzq.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gqphtlklk.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gvcjpgfox.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gymxmlpiv.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gnbkislsk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gwjtwlxac.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gppmjpjcr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gokiwgtur.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gslhfkuar.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gfmobqztq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gvexfxgex.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyzqukhol.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gdeofibpw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gimlpnifx.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gffehavie.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gjbkhspfh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gzvzlqlzt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gvnifsbhl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/glspkhqai.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/goglidgwd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gbxwyzrfi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gliyfperc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gflzzywcl.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gusgfvzeq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gopgwkgsg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gpfyeaqgy.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gcnlndwtz.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gdskwubzb.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gifmoelqu.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gpslnflju.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gtawsmsfm.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gpizessqn.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/goxpoywnp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gajflhxri.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gkuqzeuul.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gphrmpffx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gvlyjgwgm.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gjxxctjrn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gggfvseil.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gdhxhrlcu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gbdjvydos.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/glopcxlwj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gqkgjepfr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gvtspghdl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gimxgjzan.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gkppyccnd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gzdbbozjz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gtauncpwa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gnsgcwvup.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/ghjdubegf.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/ggeipuqrm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gwbdjuvap.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gmhfdsygz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/glvfqiozn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gpvdlgbed.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gwtprvlvj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/glyzrlwzm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/grirrgior.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/ghsorwrlo.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gwnyjaeak.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gciprqjey.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/ggehhrvdi.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gysjpivib.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gxkgjmahe.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gepmcyzlq.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/geofmanfx.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gpaaylulb.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/glupmpcgh.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gsgkjprtj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gbeybeggx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gpdvoremg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gzvbwnjji.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gnhltxpgt.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/goiajzfjp.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/glqvcguye.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gxxidmpxn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwutvuvro.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/glkjvibwh.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gbgealgey.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gsmocaatz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gdjgeedci.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gmrzckszk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gflegmhbx.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gosfxness.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gofwglsdr.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/ggnpjmnzx.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gisniwpri.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gmodiytgj.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gtfpfizsd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gcibkrpys.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gjmwviles.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gjnwxqtxm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gqtkeelqy.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/glaorguqp.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gbrxpcnwk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/guhvwxsgv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/getltnzia.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gmntsdpjc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gtgrvmzdc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gpqyyrhwm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/grbfefhnj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gabwhzpmg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gifwxzhcz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gmklucfyo.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gweivkmfl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gdvmompoe.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gzbpyikct.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gjzwemkpm.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/ghsflmapp.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gzgebufhe.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gwuipedlc.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gmyqgqxdc.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gbynwoytq.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gnhlbnigp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gzvzfmkgx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gfbnawubw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gzrjyvveb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gufjamord.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/ghhovmqqq.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gltrkpxdy.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gsgrbhefu.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gjfaanetq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gbpsasewa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gqlppetus.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gixqtyfka.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gilmwvsca.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gobyfsiyz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gwgcqghka.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gttgizpdx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gxqzwsmpl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gkjsejsus.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gizcrjoyj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/glbqbhuxg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gscxvsuzm.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gbobfufoj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/genwxubwj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gewjufqfs.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gzxxferjb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/grykokdyi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gkawzxyiw.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gfxgwxofn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gljyazqgl.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gaijemsqd.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gtfifgddu.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gqvcrlygu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gelwudgcf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/ggodoambc.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gqxiwdekj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ghyespukk.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gzsbbtlcm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gzydmmzwb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gpflfqani.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gxronegar.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gyhjbjpfo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gkypbjpnd.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/giskqmybs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gqflpivwf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gpbngjtjw.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gogtoivts.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gchdyjejs.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gccyropfm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gujxqmgzs.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gduaynott.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gdhqaomjz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbzuyuubv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gfseljkpn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gaxdzcpfs.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gjezxgyzm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gbciwfhwk.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gmykoqsje.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gfvebjyvj.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gnvwoddzv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gomztgnrh.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/ggqotngqh.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gzlokpomb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gabmagrnf.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gsdyhdptr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gowohlxrl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gzvqonhiu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gvsfybhkz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gdlqmdecp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gacczmmyi.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/ggdpjeitg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gngfxkplb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gikrltgyf.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gguiqjpbs.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gchinegmq.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/goapohsdo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gfbevdblw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gljkvjqkg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/ghpuilasu.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gponraaug.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gdleorvyz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gjfwfjbzl.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gpfsklzld.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gcddcoezd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gacasmotq.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/glgidjral.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gjpodvpzb.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/glelempgo.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gvinybbzd.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gitfmgoim.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gnfwakfif.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gickiecne.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gjqbfgicf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gydzxodqj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gpfmqkpei.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gssaizckp.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/ggnhkqdin.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gzictndie.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/glwjnqbin.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gzgparevp.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gwvhixzsh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gpuxfzgwb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gnuvkcpeu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gcfhbyxau.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gorweqzmf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gfifkwusv.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gikqfqoni.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gsndvisfj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/ghcykqphp.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gmihldzcg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gmhtrptlw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gtyguidin.sHtML


<!-- 参考信息 -->