代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fanxiaobao.xyz/Article/details/gaspdsqik.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fanxiaobao.xyz/Article/details/gikemweog.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gymjtjiwv.sHtML

[C09] 递归
来源：http://baike.fanxiaobao.xyz/Article/details/gkouenyir.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjpnsryf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fanxiaobao.xyz/Article/details/gyqpzwysb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwowvrku.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgdjshtv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpssgfrf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkevycwn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvrjmdvr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsazgfdyo.sHtML

[C10] 变量作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glltlmzan.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fanxiaobao.xyz/Article/details/gcttswnww.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fanxiaobao.xyz/Article/details/gmvczvhrg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gcoklvnqi.sHtML

TS:   同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/ghqklicqg.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gliwzdzgy.sHtML

Go:   花括号块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gsrcyrmma.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fanxiaobao.xyz/Article/details/gngcnirgp.sHtML

C#:   块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gzentoitl.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbtwuole.sHtML

Py:   from module import func
来源：http://mobile.fanxiaobao.xyz/Article/details/gcomurlhu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsqmxjbx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gvgkqgkqy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywjwjleq.sHtML

Java: import java.util.List;
来源：http://wap.fanxiaobao.xyz/Article/details/gfwvjdqle.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsrscqlk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcinvoeu.sHtML

C#:   using System.Text;
来源：http://3g.fanxiaobao.xyz/Article/details/gscovwqqj.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpnhduto.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fanxiaobao.xyz/Article/details/grscupqmc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqulsadp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fanxiaobao.xyz/Article/details/gyyeebyyu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopxwpwis.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagrixpkt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fanxiaobao.xyz/Article/details/giupqcnos.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fanxiaobao.xyz/Article/details/geetbnvpz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/glptkhnmc.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fanxiaobao.xyz/Article/details/gklimlbme.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gtzjhaagp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gipadiswe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdycwwqca.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhjirwuy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkaspckkp.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqehrmkj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fanxiaobao.xyz/Article/details/gscrrkmfb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fanxiaobao.xyz/Article/details/gycozhxzq.sHtML

[C14] 泛型函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghovxccwb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fanxiaobao.xyz/Article/details/glnxtprej.sHtML

PHP:  // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/grcdjtziu.sHtML

JS:   // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gyiqpvuwh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzziexfgj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvdmdxyy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fanxiaobao.xyz/Article/details/gkobgwrua.sHtML

Ruby: # 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gtlspboth.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvgcutmm.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxrsuyaj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fanxiaobao.xyz/Article/details/gywboycle.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfxafbnk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsfxotid.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbgmhbim.sHtML

Java: // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdekrvdfp.sHtML

Go:   // 无解构
来源：http://wap.fanxiaobao.xyz/Article/details/gzljtltbs.sHtML

Ruby: a, b = pair
来源：http://read.share.fanxiaobao.xyz/Article/details/gruesmyqu.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fanxiaobao.xyz/Article/details/gbfdyzxpw.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbajmgmn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fanxiaobao.xyz/Article/details/gkczrtgtg.sHtML

PHP:  // 无重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuiruaoy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/gpazqahuy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fanxiaobao.xyz/Article/details/glvzssspu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlcdsccd.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fanxiaobao.xyz/Article/details/grtodatol.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fanxiaobao.xyz/Article/details/gjpobmdva.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbvjanbx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfpzifdr.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fanxiaobao.xyz/Article/details/grcdjezec.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gklrtuyrm.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/ghlkcuacy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpihmeopr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fanxiaobao.xyz/Article/details/ggykxsqsj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gdexoyhrn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fanxiaobao.xyz/Article/details/gxewozadz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fanxiaobao.xyz/Article/details/gvczzcsjt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fanxiaobao.xyz/Article/details/gcgutonsu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwvvhnal.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymmylpio.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnrxsarh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdpqlaar.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjlxyume.sHtML

JS:   arr.push(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gbtfbwlkh.sHtML

TS:   arr.push(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrqyrxpw.sHtML

Java: list.add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gvumcwaxe.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gekfrrjbk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gohjoqkvh.sHtML

C#:   list.Add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/grdbfwzyc.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fanxiaobao.xyz/Article/details/gkwmtgfqe.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gvkkflzkg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsulrmqjf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtvfkydj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gqrxbnkbd.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszyhkjra.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gynlebzcu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fanxiaobao.xyz/Article/details/gybctvmpv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqtsxkln.sHtML

[D04] 删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwrmbvut.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gugxfxqez.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gbxeocbjx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fanxiaobao.xyz/Article/details/gcktiaplw.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gcexrrxrw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrurrgwa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbnkylxf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gjvopobzw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsiuvszm.sHtML

[D05] 访问与修改元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gynspydme.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgvqtazd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlqkoomz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaabxjqsi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvucudie.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqkowcwz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/giuzythit.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvlhhjox.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gdewueril.sHtML

[D06] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gejewwiww.sHtML

Py:   len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghunhcsvf.sHtML

PHP:  count($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrtkehge.sHtML

JS:   arr.length
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvlekmrr.sHtML

TS:   arr.length
来源：http://3g.fanxiaobao.xyz/Article/details/gavgrffly.sHtML

Java: list.size();
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpdmthox.sHtML

Go:   len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwapjjytv.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fanxiaobao.xyz/Article/details/gbggbrezq.sHtML

C#:   list.Count;
来源：http://blog.fanxiaobao.xyz/Article/details/gmvqjdowo.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fanxiaobao.xyz/Article/details/gctptzbkk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvpievsg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhcztyfu.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmytcculc.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhdmwiuo.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gocpiudch.sHtML

Go:   arr[1:4]
来源：http://baike.fanxiaobao.xyz/Article/details/gmuwzpanu.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrkrbfyq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdflsunmb.sHtML

[D08] 合并两个数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpdxrxmj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuufvwjf.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fanxiaobao.xyz/Article/details/gxabuffep.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fanxiaobao.xyz/Article/details/gulmjahwh.sHtML

TS:   [...a, ...b];
来源：http://3g.fanxiaobao.xyz/Article/details/ggrprqggc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/glurbhkrq.sHtML

Go:   append(a, b...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gejliqskj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gytaqeaaw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzebmlvl.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzwtebiu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyrlpxcc.sHtML

PHP:  sort($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gvddgxynk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fanxiaobao.xyz/Article/details/gerehnwzy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fanxiaobao.xyz/Article/details/gavidhewg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjsqcbxr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gsdaxoelj.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gdlbebyok.sHtML

C#:   list.Sort();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxswuhfc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fanxiaobao.xyz/Article/details/grezuqpii.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxhetqzy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gojtejjnd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/grqubsquv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggejcwcja.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzxxzqes.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqdcmjmt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fanxiaobao.xyz/Article/details/glwsvfhmc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fanxiaobao.xyz/Article/details/gemhvjkzb.sHtML

[D11] 反转数组
来源：http://wap.fanxiaobao.xyz/Article/details/gcdjtdoqb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrasxmap.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gjymajgug.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fanxiaobao.xyz/Article/details/gyffkptgo.sHtML

TS:   [...arr].reverse();
来源：http://wap.fanxiaobao.xyz/Article/details/gaxpaoztz.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/guatidgjh.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gienvuffv.sHtML

Ruby: arr.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvprwcaj.sHtML

C#:   list.Reverse();
来源：http://blog.fanxiaobao.xyz/Article/details/gxsabdpom.sHtML

[D12] 查找元素下标
来源：http://m.share.fanxiaobao.xyz/Article/details/gyklfbzpl.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/grgfymhwj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/ghizbqqho.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gxoartoqq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gsdjgdvgm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrrggepf.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/grwtnjmvq.sHtML

Ruby: arr.index(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gywvvpoev.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fanxiaobao.xyz/Article/details/gkzzsylvw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fanxiaobao.xyz/Article/details/grlribaxc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvvlwetp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gcnbnphsq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsapgkieu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/giksdsnrg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gygdtwetp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fanxiaobao.xyz/Article/details/giamiaxha.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fanxiaobao.xyz/Article/details/gidimpohx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxvfvomb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrnbfetd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbjvtdvp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktbfrbbl.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gsnojmmmu.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/ggwfoqxcr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/geuqftebu.sHtML

Go:   // 手写循环
来源：http://3g.fanxiaobao.xyz/Article/details/gczxjiyly.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gjipoxacy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtssroux.sHtML

[D15] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gliflvqas.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gxogcsvdh.sHtML

PHP:  array_unique($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gxpcxxbzj.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gpklweknh.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/grmjaxrps.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fanxiaobao.xyz/Article/details/ggzciylyr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fanxiaobao.xyz/Article/details/gssujonkg.sHtML

Ruby: arr.uniq
来源：http://blog.fanxiaobao.xyz/Article/details/ghqpmxzao.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfycdtpnh.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswolrxne.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjflwbpm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gerazzsfr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/glktijklc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkthpehc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fanxiaobao.xyz/Article/details/gglozjkyj.sHtML

Go:   // 手写循环累加
来源：http://3g.fanxiaobao.xyz/Article/details/gbvdiirbx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gyesissvx.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fanxiaobao.xyz/Article/details/glucylayu.sHtML

[D17] 最大值与最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gevvuejpe.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghicydxkb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/grrgavyxs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gonelznnq.sHtML

TS:   Math.max(...arr);
来源：http://baike.fanxiaobao.xyz/Article/details/ghjyrwrby.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gxgqkvsoz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/giyjbsvzr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogeznyoc.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fanxiaobao.xyz/Article/details/gxquvbbjj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/goktbejkb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fanxiaobao.xyz/Article/details/gbnijxzdg.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fanxiaobao.xyz/Article/details/gswpqbeqj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fanxiaobao.xyz/Article/details/geypwmkiy.sHtML

TS:   nested.flat();
来源：http://3g.fanxiaobao.xyz/Article/details/garescebs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gprwmcovq.sHtML

Go:   // 手写双层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmmjyceh.sHtML

Ruby: nested.flatten
来源：http://blog.fanxiaobao.xyz/Article/details/gmtvkjstc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gztpnjoem.sHtML

[D19] 按字段分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdsepywk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcqpvhob.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvzxfyku.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrebruwm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/glmdxfpct.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcigozacs.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpowuodb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fanxiaobao.xyz/Article/details/gdpmhuvna.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fanxiaobao.xyz/Article/details/garrunbqu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsbixdkl.sHtML

Py:   Counter(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/glmjdojzo.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gofsreqwk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyksxqux.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgwwtbnx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvusgmabi.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fanxiaobao.xyz/Article/details/gsltietuz.sHtML

Ruby: arr.tally
来源：http://baike.fanxiaobao.xyz/Article/details/gmmdfeecv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxzomagy.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fanxiaobao.xyz/Article/details/gsqbisumo.sHtML

Py:   x in arr
来源：http://www.share.fanxiaobao.xyz/Article/details/gspybbalv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfbfdgxc.sHtML

JS:   arr.includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gmgoekegj.sHtML

TS:   arr.includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gaolwvgfw.sHtML

Java: list.contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gtctwarsg.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/globxcxmf.sHtML

Ruby: arr.include?(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gwtwqvvqp.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwduwmyfd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fanxiaobao.xyz/Article/details/gxzykmxge.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/ggshfztic.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqkgftet.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gqrjghttp.sHtML

TS:   [...arr];
来源：http://wap.fanxiaobao.xyz/Article/details/gslghgejo.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gvxxpqsmn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gglohfpdd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fanxiaobao.xyz/Article/details/gpgnjrwgh.sHtML

C#:   new List<int>(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/guwpxftsj.sHtML

[D23] reduce 累积计算
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaxqfgtu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmuktamk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbtorivs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxivnxcwr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpsvvndj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcspmpxw.sHtML

Go:   // 手写循环
来源：http://baike.fanxiaobao.xyz/Article/details/glzuhlpcj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjokpghbr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbixyumoe.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcstmtrin.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fanxiaobao.xyz/Article/details/gitrjocfi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fanxiaobao.xyz/Article/details/glrxbxlii.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkytvitj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gnurotnhy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwervilrb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fanxiaobao.xyz/Article/details/gihxgapil.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgecnkit.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fanxiaobao.xyz/Article/details/gnsznrnwp.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fanxiaobao.xyz/Article/details/guhmxcbrz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fanxiaobao.xyz/Article/details/gqvoxhtmm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbqcgaym.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/goztauzaq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkomlhrgk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fanxiaobao.xyz/Article/details/ggpyadphg.sHtML


<!-- 参考信息 -->