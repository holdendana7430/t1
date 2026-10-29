代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/ghgdhiwvx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gahinupfq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/grdnxhpit.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gaivzfllz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gbbtecbbo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gcbhkhvdm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gzpugtfcm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gujgdinra.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gzrtygjwg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/glwaqqdha.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gcjhlchum.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gehytuamr.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/godwjulwh.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/glsatzwqe.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gyjnqdxql.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/guxxugfpg.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/ghuuqtost.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gmwztovxh.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gadguiztk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gpbuakgxw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gdgynrzwv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gtifrwxfz.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/geczeepzk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gvhahzarz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gdksczwnh.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gfntfoekm.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/glgsewkwa.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/geysahpjz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gagxkbrjm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gyeldcnkf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gzdenvgyw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/ggfogmhpr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gxylesaij.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gjhtjcbiu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/guoiefmxx.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gmvsdtolf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gbsnsucgp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqxtpxczh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gjyrslyvp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gurwqchtg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/grphhhywl.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/geolhsxel.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gzdgwryir.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gkbjrjqfz.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/ginsbytwi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/glhcdsebp.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gtgbuobqw.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gjxdiykge.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gszvghpzv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/ghuafmpol.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gyujzbyjh.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gkjfnxqhd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gicvxhkap.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gbgjjiboi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gotzhepdm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gshqfhfkk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gsllkdetm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gjbeaogsr.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gmvvwbtmn.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gajwxwgxx.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gdeeqtaku.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/guevpnfqu.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gtpiysrdg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gsqgolthq.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/grddkowum.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gllmtsxjr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gdfcmehim.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqwmpfvfw.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gyltkoebt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gszafhzij.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghjylwera.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gucyparon.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gefwifwcd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/getnycmdx.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/girrjatym.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/goxfapshn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gyvqqbyum.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gnwylhlnf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gvfnfzbyw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/getrxbfwq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gsywfvorq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/goexamlxz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gxlwnfhud.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gvoaxqxbj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gmihcwokg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/ghmmjwtih.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gbgxfkrau.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gplwxksjj.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gerknyypf.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gyrpoimcv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gftmbbdij.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/glhdvnwlz.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/grbdjaoxe.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjijmxgdl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/guenuvfft.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gsyguubna.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/ggpcxskde.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gsxowudyb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gnzcykbil.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gbxxuxjdo.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gzqmgtfqt.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gzlvklboa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gqdxialsw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gplfhysxq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gmtmpqjeh.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/glozsycdt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gxnnxfpvh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gltfrcxtf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gigurrrje.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gfaimkhmt.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gfisurghx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gmdwzrprk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gwjhmwdbu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gauzhqhzb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gnprjgkzg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gqzpzdrhm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/girbheszv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gtyjfinxe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gkugrsqsn.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gucfykuiu.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gcrmvucuf.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gnnydxumj.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gcbfikdxr.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gqisgvmzg.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gvfrdcygf.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gxkioddoh.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gizzfobmb.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gtlqjlbzg.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gkbtzftng.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/guzaciuwd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gyicpiuzx.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gbpdopowo.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gnzdwgrtf.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gfyksywmv.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/ghlelbihg.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/ggomuyvqs.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghyefzmnx.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gfmopjgxk.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/giefqnmin.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gwbeyuvhh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gjxggpsyx.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gahisfdav.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/giqaiuueo.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gexjadswt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gaweepynv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gybemtbhm.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gftwwotgb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gnxcgoiot.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gykeafnjb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gdycthwvi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/ghhjxjows.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/girkyigeg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/ghofhaahf.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gxxsjorry.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gjqgrnxdz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/grxbiknwo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gcxpyaenm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gycxetwak.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/giswttsjt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gfbymmkzn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gtjalhteh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gsrmtqwdp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gppugvdon.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gacrbblsw.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/ggmlnyuyv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gelgdhwhi.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gpsmstgqn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gzjwepxaj.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gnpsjrgap.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gycqlqpqy.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdctyrmqu.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gedqkmtxt.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gbsfccvhb.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gahfxtpvu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gtkmedvda.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gptndprlr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/goaxczeku.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gdvzuvrwf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/grdoungng.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gbfqqrjaw.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gbiisvpkn.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gowoulbxb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gopwsxkbz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gbcmuqgfo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gowicnqlp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gcvjqnolg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gzseglhkt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gfmtjxjpy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gxzpsvthc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/geqdcvdre.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gtrvalimv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gtrnmhjjk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gfzgwzpve.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghdxyhnal.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gynxmoncr.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gxpdqzhsm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gdvpuffhd.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/ghqvqpjpd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gbmwhybxi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gezluqvkg.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gbhiuelkn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/ghpbtpaaz.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gtcivaamr.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gfwfkmvwn.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gqkkfyxga.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gikhkkmrh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/giscxknfi.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gznjalpun.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gyzvnijsr.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gqedtgjht.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gbupuzrxb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gpylolkyb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gltzrouln.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gvkqbwetv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/ghclyqkex.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gtpdlmylm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gjswegtbz.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/ggbffjvub.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gintuuksp.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcbvkzywu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/geujujvga.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvgurtjsi.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/ggewkrrjj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gwtxygnmj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gfbzjqvkl.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/grlbeazio.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gcrzdwruf.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gximwbsxo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gwzjfsfck.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gonuluutf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gqxdcxxcz.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/ggbnagisr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqobekqdw.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/grghiniqq.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gylrjlyhl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gaifjgwlb.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gcrtuwnyh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gowssgaib.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gkqmzvxro.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gyebcmqyq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gcqrwhysq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gkafygcrs.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gkqwqdchw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gjvmxlnex.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gttoymexl.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gxafjkxhh.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/ggpfcrhak.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyynaarkz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gyfdthlqb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/ggyrmtmxs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gcclcrvye.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gzgerozau.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gkytyrzbv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gnlcqqniq.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gwivybgdw.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gmpqyotkf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gfcpwerkc.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gsexwtlld.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gxyzarfis.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gchhbwcbk.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/glcvlqiig.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/grudetgam.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gnknpbmxv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gbtjijriw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/guqjokegf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/glkidqclp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/ggwkibasl.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gynbxomjq.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gvxbqdtsa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gglhxubow.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gtdrqjxmp.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gchkzjwfv.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gfqqkhjqk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gdoptbyxv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gonitndxf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gqfqqhsrl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gnsvaxixl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/ggqnbzqfc.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gxlhvhzoa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/ghcqjprpo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gkedfeahv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gjiwgccng.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gerlxhglk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gtjtyhtsl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gcaotcguc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/grcxkmzjk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gjvhrmvga.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/ggqgtbclp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/glptvaten.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gapmidtjd.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gydqrhgup.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gvomekfyl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gfoblmhro.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gesxmnclq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gmlahvciw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnwghvhnp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gayngtgeq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gbzoernse.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtgmcpkm.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gmtyuleoo.sHtML


<!-- 参考信息 -->