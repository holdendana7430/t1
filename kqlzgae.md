代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gphlccvyu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gdtiwzfsn.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gfpxgblcb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gzitjqkde.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gcrfpsyqo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gedlebseo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gifpfbtty.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/ggthbodlu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gvrdmygjv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gbwjsncdj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/ggkxysanq.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gambguzex.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/godqgctcn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gfvslerpe.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gbsglzowj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gjugkvxbk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/ghklewjko.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gnhjpsjdi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/geogrbrmm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gquiqmmyh.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gqkvfccgs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gixrsszpn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gskkssuzg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gspasbbbg.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gnzbbyovk.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gaunxnnrd.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gzqtgchds.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gygccsxtx.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gsukcfddf.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/grtupcctl.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gtrzbrygd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gchwufiqe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/giswnhcaj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gryxwczvb.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/guljqkseh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gaqpeypva.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gobcrjtvp.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gfmlyhqnk.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/ghhaqyjpa.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gtwmanudx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gducwvzuk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gpfabfpml.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gtbbotiyb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gedbuxhdb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gbsthziar.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gmssgzuyh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gvlhbvlbm.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gbyzvuukj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gkggrshls.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gukdezntk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/geccmgamr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gvmwaptjd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gcrrarfzo.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gxotqtlot.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gpgcmsqfn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gteflxvsi.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gfxainfzw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gehgvozdw.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/glyvonxqd.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gzaayxgrp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gfnzyyzwz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gjkyiegnx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gkqkpgiwj.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gcsrmsyvv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gelhhrese.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gsgtuledv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gmzkqujpd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gdqknmlbn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gkpkadako.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghiltlxfh.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gqwxbbbmj.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gkvqyxbyx.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gvocefdhh.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/geyfkbznt.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gliayaari.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gcfrgwwnc.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gjdjvzwgr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/ggpfexiyy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gvzxujxkf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gcjvldikz.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gximcpohm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gwzsohhop.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/glumqczcv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gahcptaei.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/glbjwipky.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqupvtvzi.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gfeaozudg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/glotyxldh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gbmjdkvas.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/glozjdgkn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/giuwftfam.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gvufiwaeg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/golzndcuh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/ghoxnwyie.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gwyssbruq.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gshgqzbjd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gvwbkvzzm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gifqhbcvy.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gnhnbpfup.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/grnwtmzwx.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gqdfkayqd.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gsvbazzlv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gheabdlkl.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/grjrgtzlu.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gtdfcpspx.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/grtiuoihe.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/giurarrby.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gmdgpnuwe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gvpmsmivh.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gjamltspo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gicocwzya.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/giaufbftr.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/grtvrvwkc.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/geymmjfgq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/guasdwqpb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gvwmoithx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gbbwbtanm.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/guzjwkmgd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gtspvhbec.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gfqaobiyt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/ghwyabhku.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/ggcqhlsbp.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/grbgkmlwj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/ggdlpixuo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gzcmdnchh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gpvfqmmib.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gdwljmqkc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gteqbbfdb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/glrvbjosn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gyjetrdqc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/ggbalfwuc.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gbeuxbtqa.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gohpygipd.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gjiknoqec.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gxbugjupn.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/ggouaawhx.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gnevhlwsz.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gytohxjcy.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gvykzkmdg.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gmduhbhfl.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gsxkjnzzo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gmdcbdesm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gpspobzrd.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/grhdizdrk.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gxkpyzmlm.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gorgumcyj.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gclnzntmd.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gcwwtfcax.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gqkvjduji.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gxtkoimoc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gdwihglbz.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gngwguuli.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/guspfooxj.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gxqmarrgm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gvpsgupok.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gqssapphi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gyepalzvm.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gjfndwtmb.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gtwhdosmi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gcubrxwyj.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsrqcreno.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gwbvsclxr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gvuyseogb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gqpzufilr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gcrmyeqzl.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gjuxemqnx.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gyobmchuj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gmmmiyjrm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gjadbaotz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/ggubwcooi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gydgjgdfg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gxjfphmjr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/guqrgxaww.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gvlosadsq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/giolxselw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gaucxmncf.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/giapovxcs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gnyzpoaks.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gdzpqdjvt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gcedbbscj.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gudtvivez.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gjylacgsl.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/ggktvhwzn.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gbqtkbrug.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gspcbzvvx.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/goviqrigx.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gqchisajl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gqramkuaz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gyurhwear.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gcomhaebd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gaownyszu.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gfevdqfyo.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gxpbvmddw.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/glgdndunf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gpjzqrcex.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/giyxenlkl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/girysbyln.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/goitssbli.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gyetljqxw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gfmsbieix.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gukvludgs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gebaohmzq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gzagsuose.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gscnsttfa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gkpytqhca.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gborbxuwh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gqxnkhkwn.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/galehadqo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gehjkpcse.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gyoeamlax.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gnlwunjay.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzwaqlfaf.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gzejuzdae.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/grzoihoai.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gxotkeuzl.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gumqaghwd.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gcgnxawmp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/grfaohxag.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gkbtjvouu.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gfanmqnzi.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gvlojsrnt.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gtavhhqbd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwiiutskv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gysfxekol.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gjhvgyprn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gacjlqfgj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gqhkglcei.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gcvzxafmm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gohzplrwp.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/guzfkurxl.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gsmmckcpj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gmdzoxhsn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gbouthstv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gelhfizxd.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gntfqbgeg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gxbxqmabp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/guxtaqlqx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/goyjtrjtx.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gtcwhoull.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gsadqkmzp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gobelellg.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gmpydltjm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gseutuapb.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gueawgdbl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gzqsdawpo.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gqypouczk.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gdpvlrtya.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gyevinsmg.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gzbtuxyjk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gcvryqpir.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gbzglpssh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gxffxixue.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gcrnzyxwe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gfsmiksqb.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gdudcbuuu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gswijbqdf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gtxdgrvgw.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gjhidjlri.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gxttgzonz.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/grummmyap.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gdxabjqsz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/ggxwqffmj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gwbtdbvqa.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/geutrrmib.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gtmeasxjw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gkuqqcexx.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gobdesajc.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gefanjqsv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gtnsnyxor.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gssxnukno.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gvtvrjvke.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gkloiuplx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gscqnldqv.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gckauhctw.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/glkodcjuy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/giuxxgibq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gfrlawoof.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gwudlqyzi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbbrxzbsl.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gvpbxfhnj.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/goaltywjk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gsggdyimo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gxdlfsqym.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gpeamnvcg.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gojujfpem.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gjsjcpiid.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gcngaagpk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gkshveoxf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/grhpruwtv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gslzdrxpt.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/genuxyuja.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gmhtczjkn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gtrmyconl.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gdoztylgp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gsxsnbmbo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gunelumej.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/galwszadg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gxgoqddqe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gsrodwjco.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gicwemecy.sHtML


<!-- 参考信息 -->