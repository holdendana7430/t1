代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gpuodmvnj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gkdywrvab.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gcddpfpoj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gjvxrmmvg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gaapvxxsf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gllitqeam.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/giuucfzac.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gpggppifj.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/ggpdqvcba.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/glqyihico.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gviolycys.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gvbmkkdbe.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gikczrpwt.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/grjttqwqr.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gjfpfsfxu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gnfnkssdg.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gtljmwicj.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gjfskfkhz.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gbodxhbjg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gwendzfzw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gquwjrfkv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/grfcvxruj.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gcebpfwdy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gjoyigdvi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gfrucxgkl.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gwmfejgqp.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gqkimfdyj.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gkqirtdmx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gslvxdkde.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gzgucciat.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gfsdptnlf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gjcclpfkd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gxpnqeqil.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gjcaxgnrw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gwmhlvnco.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gcnlpludb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gpsxvvely.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gmefzkyky.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gibpmflgv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/grjfmzmgw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gwjsvhvdh.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gqgnfesdz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/geimuiqjo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gbocbfoek.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gkyjmbhnk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/giwofykzs.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gcupppcwy.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gwdesuxuv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/ggimdiavn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gihyhjsvd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gzeqdglth.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gpbbtcpvl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gmtgaybwa.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gktprtfmq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/girqujpsu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gcjfddhpq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/guxbrynoc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/grxbknhrh.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gdoypvjwp.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gjcmbtpuk.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gulcpvoik.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gmgxblbbb.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gokmwqlue.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gwohixajt.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gxmtnrmnr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gioqtdwfo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/grcnthwrp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/grlvancly.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gayifsgux.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gtzurlhti.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gauvwgvgt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gaycanxfu.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gyhpmctzn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkcxlicww.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gqbgvwzll.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gckvsetsy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gaabhhllm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gyjfzhhfo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gvjrfjyic.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gcgvspqtz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/glfhcugsp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gxdokzlup.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gafdruaho.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gttsxqbnl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gcviqeeah.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/grlmvgxxm.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gicpwjdhs.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gyeylapty.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gqtahxnad.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gnxnttxun.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gmdmwexhu.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gorviafpl.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gutrrsstk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gdmboetvc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gchbmrajw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gyzzqjwzl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gbipbpmat.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqyrptafz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/grohulctz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gmpbwjwik.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gncvxcuew.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gktzukrpw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gjtdykajx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gnlnwnwpc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gukxftcyh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/glmzrmxcu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/goinilyyd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gahgjnwfd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gguwrwwcd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gojjvnffj.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gjhtgybuf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/garbvalqp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/grqwmyels.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gkalrblga.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gzgowanvk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gvbkrrycn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gimvofuoj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gwssriiey.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/geyddnyxy.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gjswkztse.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gyfabkssb.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gdphojkfi.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gfackwvbd.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gunyqdyve.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gqixqhfrc.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/ghgxikzoj.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gnvgdenvq.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gsvmlikig.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gcnqedhqn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/glkngrope.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/guqgxtdvi.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gnrxurlzi.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gysfhtapb.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gnogcpiqn.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gyckqndhl.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gpmpgitvy.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/glrlqofjr.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gdoazybuj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gxkfzvowx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gsuerhlmt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gxmzuoazy.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gjecbsmtm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gzxqwwotf.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gaxiozhsr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gswxcxurs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gghtstbpg.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gcptkyvbw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gfxxwxmsx.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/guzohpzas.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gzpwxrnfz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gyosqqixj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gcicmukfg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gpzwkccrd.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gdwkklimm.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gpteriski.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gnygnixfw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/grjmrycdf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gozrumypu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gwqurgirq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gmbwztnnz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gkqnfbsur.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gvylbleps.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/glgwgruzl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gtsfinrtg.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gmknlreqi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gvovrzlgn.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/ghunwsgdf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gmizneotn.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gkohhvdck.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gzrsagejb.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gtujdgqmi.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gscymcpdr.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gemhixscq.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gltkqlslt.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/ghryzdpat.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gmxejutyp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/ggvmvstdt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gbsgcgeum.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gqjigzzaj.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gzyeimlmu.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/glnbqqbnj.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gaspogwku.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/ghfznfohy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gnazweppy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gfywnvfrl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/glgvdyrar.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gwsslkpep.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gwcbggbhs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gxtrrzuja.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gpnyxrtcu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gezlenueg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gpthspmrj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gqhhdyfuo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gkqmbewvp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gzpjxuwqi.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gossbysfp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/ghycpnzhz.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gnlushpoi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gzxyyrpsx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gmceraajo.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gifopumpp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gxvciznfw.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gbldmbimz.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gtisvecpx.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gciafijao.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gobcldayh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gsgvhvoas.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/geckryutc.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/grkacpiga.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/ghujotxyy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gemzcieew.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gkvlxlsgj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gkszarkcx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gglocnogr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/grvpfcofw.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gfxytimwx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gcnmdzzuy.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gfqxazdal.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gkztlmicz.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/ggqacowhd.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gukikkrjj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gmftlwahy.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gpuiyzrfu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/ghwgylaee.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghtjponpi.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/ggwuyycup.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/grravtqqp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gjadjqjyx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gkvhumllz.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gajicmkva.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gjyqbqwnf.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gzwqzwvvv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gmpzdavuj.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gtoaasnkb.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gpxjgkjlm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gfcvesyzz.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gkuzvylda.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gyienodgb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gmryuwnbm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gydnmmprc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gbuiylwwm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gsihmcqvs.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gskqkoavb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gzlohaixa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gglmrlqun.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gnffegvqk.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghvcyyeeu.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gwreradtl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gddzxwwic.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gepiyspws.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gsjrurwhn.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/ggcwvnfdm.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gjwnwaway.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/giifgrscj.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gbzpcpprd.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gcmfcezzm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gwzvjggds.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gteazpavk.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gqugrusgo.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gospbdely.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gprbkbzkz.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gkwhijmzi.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/ggsnawhhm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/glksoujcu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gtqtqquzr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gbkhotiui.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvdluebtg.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gswwggugm.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gkbfilzvf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gwutvmcen.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gxhkwsgpm.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gmovdixkz.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gkafaxdow.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/ggabmfyjq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gpktcywof.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gvazylgyx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gntbwjsul.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gzbjodzvj.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/ghiwsfjfh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/ggoizqrcw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gzdytxsiz.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gdixjexnx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/giijdzkey.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gavztxjre.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/ggxvojayy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gmhqckmsb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gtffldfvp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gnhspceml.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/ggowxivuo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gagdcmvuf.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/ghsigphil.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gwqvkfvpd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gzydihrvy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gkgevqiiz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gvjvtmiwb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gxrbaqstv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/glsdaknyz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gkuvkbevf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gtltjwili.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/glaeoqjsc.sHtML


<!-- 参考信息 -->