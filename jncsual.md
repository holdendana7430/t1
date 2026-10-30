代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fanxiaobao.xyz/Article/details/gilbynqrn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaedgcvem.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfnxorhob.sHtML

[C09] 递归
来源：http://wap.fanxiaobao.xyz/Article/details/gzlbbcoxt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjuebkbf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtonmcsbo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlklejxd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fanxiaobao.xyz/Article/details/gbizbuksn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/gxnpjvipx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fanxiaobao.xyz/Article/details/gbxezishp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxudjpymv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gfyagjkcn.sHtML

[C10] 变量作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guynagnbn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fanxiaobao.xyz/Article/details/gncaptdal.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fanxiaobao.xyz/Article/details/gqetedkbd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gfhdbwxgb.sHtML

TS:   同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gjwaqjqag.sHtML

Java: 方法内为块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gkqathzjo.sHtML

Go:   花括号块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gpmsnenln.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fanxiaobao.xyz/Article/details/goarcbuth.sHtML

C#:   块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gebulgfij.sHtML

[C11] 模块导入与导出
来源：http://wap.fanxiaobao.xyz/Article/details/grxajjdqs.sHtML

Py:   from module import func
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiegovbd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fanxiaobao.xyz/Article/details/gybyeinqs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gbgmxoypj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fanxiaobao.xyz/Article/details/gqthyguxy.sHtML

Java: import java.util.List;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtridmmu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbdfyicv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbcjhcej.sHtML

C#:   using System.Text;
来源：http://blog.fanxiaobao.xyz/Article/details/gjxizwkha.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqcpsuhq.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrwscqlh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gityqnsgn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpcdbgds.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fanxiaobao.xyz/Article/details/gkeknmwsl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyqfndcd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fanxiaobao.xyz/Article/details/grihecqzy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fanxiaobao.xyz/Article/details/gikfkersr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbjnyxbwh.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fanxiaobao.xyz/Article/details/grxkmfivt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/ggglquevb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtirrkkk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphvsyocx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxhtrwox.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfkvdeswn.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwmtofko.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlgwmjhf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fanxiaobao.xyz/Article/details/goxruyyjc.sHtML

[C14] 泛型函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqffgdkc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fanxiaobao.xyz/Article/details/gawdcdsah.sHtML

PHP:  // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gzniwlsjy.sHtML

JS:   // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gbrukuqob.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzxaiqlmj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudihucbl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdesckwy.sHtML

Ruby: # 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpqyvflw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fanxiaobao.xyz/Article/details/gjozjzkdp.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkazimwgu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fanxiaobao.xyz/Article/details/gqtehcxuo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsulhlrm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gcefrqorm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/godgzrayp.sHtML

Java: // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/geyjyrnmn.sHtML

Go:   // 无解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gscuthapk.sHtML

Ruby: a, b = pair
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjdjcwin.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fanxiaobao.xyz/Article/details/gdexmgagr.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhdngkog.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fanxiaobao.xyz/Article/details/gtroqyoxc.sHtML

PHP:  // 无重载
来源：http://3g.fanxiaobao.xyz/Article/details/gbaointjq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gobxwyrsh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjknpcpl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gmgsytjhl.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fanxiaobao.xyz/Article/details/grgzeiemu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmplvysz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnkeddek.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplqlxrrm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiuuzvbu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvigpopa.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fanxiaobao.xyz/Article/details/ggjzjaqth.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhoeagnn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/grbkjlxdp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiqgdgjq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrmrlyuj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fanxiaobao.xyz/Article/details/goatrbnyx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkvaawtx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvuxvmff.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fanxiaobao.xyz/Article/details/guaeeixpu.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzvliwkm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fanxiaobao.xyz/Article/details/ggclqkkhj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacbflpde.sHtML

JS:   arr.push(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/geclukuhq.sHtML

TS:   arr.push(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gowzgsnzs.sHtML

Java: list.add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuvwxwst.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/ggsgvorbd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fanxiaobao.xyz/Article/details/gfdtieyho.sHtML

C#:   list.Add(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmmvsgql.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtozaxbyf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnzkwwok.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyqcrzuj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkvlpwvs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdlesrpw.sHtML

Java: list.add(0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/grmjvsfqg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fanxiaobao.xyz/Article/details/glmhecvlq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fanxiaobao.xyz/Article/details/gfuwthmdl.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gjibqteox.sHtML

[D04] 删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxhusbim.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhnzpfom.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibrrnisy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fanxiaobao.xyz/Article/details/gajwkyxqu.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gedmfecdg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxbpgzco.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fanxiaobao.xyz/Article/details/gtusgunwj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fanxiaobao.xyz/Article/details/ggmommxwf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjinveta.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaxiyhrh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gtohmimtr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gpwqplomc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gwptkucst.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyodjadr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhejlsup.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlkceyfn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/gmrezfgko.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gyohewhmt.sHtML

[D06] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdcznnpb.sHtML

Py:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gletvcukq.sHtML

PHP:  count($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzftdjgit.sHtML

JS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/gtgwyqkni.sHtML

TS:   arr.length
来源：http://m.share.fanxiaobao.xyz/Article/details/giucvvdit.sHtML

Java: list.size();
来源：http://www.share.fanxiaobao.xyz/Article/details/gcljviktr.sHtML

Go:   len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssjffkut.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcijtdqh.sHtML

C#:   list.Count;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweeetoaf.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsiwifjn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuibfgro.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gshzqyohg.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gevxnpjvf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfzdzvzp.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gatysfsxw.sHtML

Go:   arr[1:4]
来源：http://blog.fanxiaobao.xyz/Article/details/gdjnacedt.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/gxncifnve.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxcqcftx.sHtML

[D08] 合并两个数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqortbhq.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyazptnyz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpmktqwe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpqutfgg.sHtML

TS:   [...a, ...b];
来源：http://baike.fanxiaobao.xyz/Article/details/guoamidoo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/guiyyfipf.sHtML

Go:   append(a, b...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxufzrhav.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxrobvya.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoqtsnpg.sHtML

[D09] 排序（升序）
来源：http://baike.fanxiaobao.xyz/Article/details/gjpsetxpm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqklrubji.sHtML

PHP:  sort($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/ggulmekzg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fanxiaobao.xyz/Article/details/ggrcbtale.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzbpmocy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmiwvxkf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbfdboxc.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gxtpajyca.sHtML

C#:   list.Sort();
来源：http://baike.fanxiaobao.xyz/Article/details/gfmwznorw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbodusbg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/glnqsbnqt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gmmgjuopl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fanxiaobao.xyz/Article/details/gwblxvups.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gzjemffdt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fanxiaobao.xyz/Article/details/gwvfhxhaz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fanxiaobao.xyz/Article/details/gjkttakma.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcwawcyw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fanxiaobao.xyz/Article/details/gypilmxje.sHtML

[D11] 反转数组
来源：http://wap.fanxiaobao.xyz/Article/details/gweerpkdx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbskftius.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtooktzjk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvtocxsd.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddsbegjx.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyudqbgkc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnraynoa.sHtML

Ruby: arr.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gkbpkgxbx.sHtML

C#:   list.Reverse();
来源：http://baike.fanxiaobao.xyz/Article/details/grdlmikzj.sHtML

[D12] 查找元素下标
来源：http://3g.fanxiaobao.xyz/Article/details/gmehqiexn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fanxiaobao.xyz/Article/details/goejhacxr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gdisgpdam.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkjdxukl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdsvwmfh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fanxiaobao.xyz/Article/details/gwjifjpvn.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/grasqextl.sHtML

Ruby: arr.index(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gijwhrbnx.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgdynfhi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxckvajow.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gejeklvhr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gwqcbslnk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosacpjtx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmpvjwbq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/getlwradf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fanxiaobao.xyz/Article/details/gxpwuhfvd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fanxiaobao.xyz/Article/details/gkhztduhq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gwnsucdpp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fanxiaobao.xyz/Article/details/getyhgayf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/ggbmwnfpe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdkvtwbi.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gpdbytugm.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqctxrnfi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gmatjuaak.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/gvuxmnxpi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gjmkywlik.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gzmvicdiy.sHtML

[D15] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuwyedub.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gawtdtepd.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guutigvzc.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrqlwsif.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxikyotrm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbneafvuo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fanxiaobao.xyz/Article/details/gikaycjfx.sHtML

Ruby: arr.uniq
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxoxrfzi.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gljddeeyu.sHtML

[D16] 求和与平均值
来源：http://3g.fanxiaobao.xyz/Article/details/gsbvvwmky.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmoyidmv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gqoatawks.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/grrywwcts.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyqkupba.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fanxiaobao.xyz/Article/details/grondllig.sHtML

Go:   // 手写循环累加
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxxqfjfe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhgfcoen.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjorhmuvn.sHtML

[D17] 最大值与最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gfvhbpfqk.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gcvqswotx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gloncwrge.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvrrfpgr.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghggwizfr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqfxkcfn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgbdjbjd.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fanxiaobao.xyz/Article/details/gvspwazrc.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fanxiaobao.xyz/Article/details/ghavvwgat.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fanxiaobao.xyz/Article/details/gpxufgnrl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gddqqbffi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fanxiaobao.xyz/Article/details/gofwndftc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fanxiaobao.xyz/Article/details/glyuctvgm.sHtML

TS:   nested.flat();
来源：http://mobile.fanxiaobao.xyz/Article/details/gakcvuark.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/ghcsubnac.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlimmqii.sHtML

Ruby: nested.flatten
来源：http://baike.fanxiaobao.xyz/Article/details/gztovrzvu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhszxekl.sHtML

[D19] 按字段分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaskdqdq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/grzkrbbbt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fanxiaobao.xyz/Article/details/gxmjndqzc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiqpsmzf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwsopcam.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fanxiaobao.xyz/Article/details/gccfturxv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fanxiaobao.xyz/Article/details/grdpqsqup.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitvzfjvh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fanxiaobao.xyz/Article/details/gcnrcmsgp.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fanxiaobao.xyz/Article/details/gwozyhlwu.sHtML

Py:   Counter(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqclysiaz.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyuottan.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocazaejd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gngstfzfg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fanxiaobao.xyz/Article/details/gzwyrvevy.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztsjwhst.sHtML

Ruby: arr.tally
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkbywkuz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fanxiaobao.xyz/Article/details/gpevhuqjx.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fanxiaobao.xyz/Article/details/ggjxslurh.sHtML

Py:   x in arr
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpgunriv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gqlhsvgry.sHtML

JS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gspjtyszg.sHtML

TS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/grqzgbcax.sHtML

Java: list.contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gounvultu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdkuethx.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/glnjvmmyf.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhvodfzj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fanxiaobao.xyz/Article/details/gmnlxrupi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/ggilzpubn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyssqnjx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gzpwswrbr.sHtML

TS:   [...arr];
来源：http://www.share.fanxiaobao.xyz/Article/details/gplkxrhpx.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoowqhce.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gtiitlora.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fanxiaobao.xyz/Article/details/ggptbegvj.sHtML

C#:   new List<int>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gsvgntdsm.sHtML

[D23] reduce 累积计算
来源：http://wap.fanxiaobao.xyz/Article/details/ghhqrmffa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gifcosgop.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgelmemp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnsvrmbi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpumntrdc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fanxiaobao.xyz/Article/details/glwizqmjj.sHtML

Go:   // 手写循环
来源：http://baike.fanxiaobao.xyz/Article/details/gfauwkixp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fanxiaobao.xyz/Article/details/glpskdvgx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbojazupr.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fanxiaobao.xyz/Article/details/gsfqfklwu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gckxmxuic.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gwgkbhgxh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gfwzsorcs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gqwpcyvms.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fanxiaobao.xyz/Article/details/ggqlipjhs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyiqptpv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxcbizwg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fanxiaobao.xyz/Article/details/gnkmaiaim.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fanxiaobao.xyz/Article/details/gmiqmnewc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fanxiaobao.xyz/Article/details/ggxfwevap.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghslbrclr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnywvkbof.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcuqzacj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxtysbln.sHtML


<!-- 参考信息 -->