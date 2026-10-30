代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://blog.fanxiaobao.xyz/Article/details/gwwikxsxn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheuohlme.sHtML

[C08] 闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gmchxiiwo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fanxiaobao.xyz/Article/details/gfyjmbnir.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikyimuor.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxvafhmf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggjoashfm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fanxiaobao.xyz/Article/details/gupskwplo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfihjxeb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fanxiaobao.xyz/Article/details/ghxtidskp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpggejggf.sHtML

[C09] 递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvhuowbx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrkoxvim.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggugexuhi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fanxiaobao.xyz/Article/details/gegqjykvp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gsgujooyk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpemrobpg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdbbuvux.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gevwljhst.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gczoqqupm.sHtML

[C10] 变量作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gskerahwa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyzqlgja.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fanxiaobao.xyz/Article/details/grggliqyl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gaqtpavhg.sHtML

TS:   同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeoinray.sHtML

Java: 方法内为块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/greckjucw.sHtML

Go:   花括号块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/guutyseee.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrcdbfjm.sHtML

C#:   块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxdzavzb.sHtML

[C11] 模块导入与导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjovtuxr.sHtML

Py:   from module import func
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcvjjyzv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fanxiaobao.xyz/Article/details/govnqzyxm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjvdkdyh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fanxiaobao.xyz/Article/details/gcdbfyrjm.sHtML

Java: import java.util.List;
来源：http://wap.fanxiaobao.xyz/Article/details/gtbgmuzkn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmimphnde.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fanxiaobao.xyz/Article/details/gdnsoeqcc.sHtML

C#:   using System.Text;
来源：http://3g.fanxiaobao.xyz/Article/details/gppaghkuf.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fanxiaobao.xyz/Article/details/gxehymkxy.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fanxiaobao.xyz/Article/details/ggiunyyle.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmakcluv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gyifqwbca.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfncrazy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflefuugh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fanxiaobao.xyz/Article/details/grausokof.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fanxiaobao.xyz/Article/details/gkeynpvyk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdfrssul.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fanxiaobao.xyz/Article/details/gwusiilqz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genxdvimk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbkvsvxx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvdlwhbx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyeczinc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glcjobxny.sHtML

Go:   func add(a, b int) int
来源：http://baike.fanxiaobao.xyz/Article/details/gipqyanul.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvooymwiu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnetddur.sHtML

[C14] 泛型函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyzrqrhd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrnkohmq.sHtML

PHP:  // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gskzppvna.sHtML

JS:   // 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gxrorjoqf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrejcaay.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gobvqlgea.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fanxiaobao.xyz/Article/details/geomdwjrn.sHtML

Ruby: # 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gwocekkhv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtzhjxvc.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdufdkfpa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexbubtoc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fanxiaobao.xyz/Article/details/gglrovcwm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gumbzmqvg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gjlrwwjch.sHtML

Java: // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfvalqza.sHtML

Go:   // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/goemsxlvj.sHtML

Ruby: a, b = pair
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjfmjxyl.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgsjrajk.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fanxiaobao.xyz/Article/details/gzldxuhrh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhrhejmi.sHtML

PHP:  // 无重载
来源：http://wap.fanxiaobao.xyz/Article/details/gdspbggdk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnklfozhz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnybpgkm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyinsyalc.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fanxiaobao.xyz/Article/details/gkykqwzae.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjixpxna.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzldfsai.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gartiuasn.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fanxiaobao.xyz/Article/details/ggypmgkjn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnuggoone.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gnphkungn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqmfaijx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/garvpwoqm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fanxiaobao.xyz/Article/details/gzdociwzw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fanxiaobao.xyz/Article/details/gypexbkbp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmcqpcbu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fanxiaobao.xyz/Article/details/gipfrhrhp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnazhgfr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fanxiaobao.xyz/Article/details/gymjgkuqp.sHtML

[D02] 追加元素到末尾
来源：http://wap.fanxiaobao.xyz/Article/details/gvcpqjxls.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqzglrer.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getpclwqk.sHtML

JS:   arr.push(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gcfvteaqr.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlcwcesa.sHtML

Java: list.add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnqofsrz.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gprdrajjg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fanxiaobao.xyz/Article/details/gcsiharop.sHtML

C#:   list.Add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gsxlzskvk.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fanxiaobao.xyz/Article/details/gyatokwzx.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdwsqynx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fanxiaobao.xyz/Article/details/gjigtbtwy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfmuwylt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gotrehqqt.sHtML

Java: list.add(0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gztaukzha.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fanxiaobao.xyz/Article/details/glsgeitzj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fanxiaobao.xyz/Article/details/gjfcqkbjy.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gmxfhhkni.sHtML

[D04] 删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gbomcbgnw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fanxiaobao.xyz/Article/details/garswvzoq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvqfpxco.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fanxiaobao.xyz/Article/details/gejzoqxoo.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gvadvphds.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fanxiaobao.xyz/Article/details/geprifyxs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwjbjlao.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxidhqbwj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fanxiaobao.xyz/Article/details/gribmtvzw.sHtML

[D05] 访问与修改元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbndddip.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxyzcain.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gysxrdxna.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/glsawrftl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeehgpvx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvzxxbug.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrcdqowx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/grzjprzre.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/grnmzjxob.sHtML

[D06] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gkezshhqh.sHtML

Py:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gwkzuwovk.sHtML

PHP:  count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbqclxbc.sHtML

JS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszmkzxjv.sHtML

TS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gyogupmru.sHtML

Java: list.size();
来源：http://read.share.fanxiaobao.xyz/Article/details/gpymvlxwc.sHtML

Go:   len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtwzqrww.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/guykecyfv.sHtML

C#:   list.Count;
来源：http://3g.fanxiaobao.xyz/Article/details/gecuoclvz.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fanxiaobao.xyz/Article/details/gmzuhdxqg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcybeaer.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/guuzaedzi.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfrtksvz.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmudsodlp.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gghtdtldx.sHtML

Go:   arr[1:4]
来源：http://read.share.fanxiaobao.xyz/Article/details/gakiggapy.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/gfefzhlgi.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/glrdzufjk.sHtML

[D08] 合并两个数组
来源：http://3g.fanxiaobao.xyz/Article/details/gjclhfkgx.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gxjviihfw.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fanxiaobao.xyz/Article/details/gznuqmkes.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgkisezd.sHtML

TS:   [...a, ...b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwfsqtnz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnhupkne.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuupitkj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwnhltos.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzjysawi.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giemhlvzb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllyhlpzn.sHtML

PHP:  sort($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gvnulifay.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fanxiaobao.xyz/Article/details/ggzaqxvls.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmblodwde.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiuoligt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gysevcvfn.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbueyxxf.sHtML

C#:   list.Sort();
来源：http://wap.fanxiaobao.xyz/Article/details/gbfqxymkm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpjgctka.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fanxiaobao.xyz/Article/details/grgrjltvo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtjeteaq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzuhrprx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gehenxpwk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjaxtrdf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fanxiaobao.xyz/Article/details/ghesgruda.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjjxmoib.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdxwrore.sHtML

[D11] 反转数组
来源：http://wap.fanxiaobao.xyz/Article/details/gdljxqpof.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddvhjqve.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/giohcuprz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fanxiaobao.xyz/Article/details/gduqnpbpt.sHtML

TS:   [...arr].reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gsftvetsk.sHtML

Java: Collections.reverse(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gzonmzrwd.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjicxckhh.sHtML

Ruby: arr.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gcqgtncfb.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybhxdyaj.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswgyavbr.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/gczczvkjm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcawruzof.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gswsiilfb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gjtcrbnrh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fanxiaobao.xyz/Article/details/guntqkpzq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcbcephb.sHtML

Ruby: arr.index(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gixukavuu.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiefpjgx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjtryagt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gorpszefq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggscxmpgz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyzyrnuz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgwphgwy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcktcoat.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fanxiaobao.xyz/Article/details/gfrzdqfqe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecgjjlem.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/geikymvus.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwryfsbw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/grsarlyna.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkgahmfc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjauazuci.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/grrngltud.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbmtgemz.sHtML

Go:   // 手写循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbizaiik.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkpdrazc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gytadpwla.sHtML

[D15] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/guitggdhu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmhzqkvf.sHtML

PHP:  array_unique($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gxxdilrqd.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfqyeswo.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gynyucqiv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvpvnjhp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fanxiaobao.xyz/Article/details/gmpdqvlsv.sHtML

Ruby: arr.uniq
来源：http://3g.fanxiaobao.xyz/Article/details/gzyhumumo.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkarlost.sHtML

[D16] 求和与平均值
来源：http://baike.fanxiaobao.xyz/Article/details/gzebientf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grswwbdrb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gormbwctr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfaqsuvm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyiqzaym.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fanxiaobao.xyz/Article/details/glhykzvkq.sHtML

Go:   // 手写循环累加
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpbkdlmx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaarbtsm.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwhnqhwz.sHtML

[D17] 最大值与最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gahtnneku.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaszgqrg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjelgppir.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gtyenktpd.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwyvtoep.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gczzdkosn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbteykxum.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjagfuhj.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfactwcmn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fanxiaobao.xyz/Article/details/ganobttoq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fanxiaobao.xyz/Article/details/gimamrlth.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyunhcqb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fanxiaobao.xyz/Article/details/gotlesamm.sHtML

TS:   nested.flat();
来源：http://baike.fanxiaobao.xyz/Article/details/gqmfzvaxc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemxvukfb.sHtML

Go:   // 手写双层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gtbabsdyv.sHtML

Ruby: nested.flatten
来源：http://mobile.fanxiaobao.xyz/Article/details/grldgxkaq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvixpsdg.sHtML

[D19] 按字段分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gmelpdxqt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gupoxeiiy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fanxiaobao.xyz/Article/details/gcnfayvzu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvwfkoch.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzugvfabx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldplswqj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbdlhbch.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnomxvhvk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fanxiaobao.xyz/Article/details/geovkxvmr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnrddncx.sHtML

Py:   Counter(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmanxpcbr.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gawhdomdt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gnimmmmvg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/goiyvmdix.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fanxiaobao.xyz/Article/details/gowxgcbrj.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsxejjme.sHtML

Ruby: arr.tally
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqdswqpy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfefpyqa.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fanxiaobao.xyz/Article/details/gnefukoxp.sHtML

Py:   x in arr
来源：http://baike.fanxiaobao.xyz/Article/details/ghxoxfxnh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxutoefy.sHtML

JS:   arr.includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gudfzqzvp.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gligcbfcl.sHtML

Java: list.contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcxqviiz.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gwdkidgbl.sHtML

Ruby: arr.include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/ggtwhmmuf.sHtML

C#:   list.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/ghueclozj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvshyeot.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gwmurwile.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fanxiaobao.xyz/Article/details/gvnpjtidj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gremdxlng.sHtML

TS:   [...arr];
来源：http://blog.fanxiaobao.xyz/Article/details/gtdlngfld.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gzaqcjfzk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbomlikfh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fanxiaobao.xyz/Article/details/geolfxmkr.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgdmpumy.sHtML

[D23] reduce 累积计算
来源：http://read.share.fanxiaobao.xyz/Article/details/gzttofynt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpuqrgso.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gocagfhnz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gpmtinoqy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gwdhpsivf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fanxiaobao.xyz/Article/details/gonsndjfo.sHtML

Go:   // 手写循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqoahpbu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fanxiaobao.xyz/Article/details/giefgstyk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbsjtifo.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fanxiaobao.xyz/Article/details/gsoayrxvp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjluipicc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gpwhcxiww.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgsmqdpd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gshzspvex.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwxzqrfa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxqstlww.sHtML


<!-- 参考信息 -->