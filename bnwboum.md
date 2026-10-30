代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gboinxskq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gcwhdmutn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/ghsyirlsg.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gttpenbzz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gutfbgubm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gmmnblykh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gbrhbquxm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gkulqxbnf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gykddpslt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gqmdkcwij.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gobqpdhvr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gznrmcltz.sHtML

[C10] 变量作用域
来源：http://www.blog.hesvh.cn/Article/details/gvpaywwhs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gnopcypvv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/ghtvbxjcq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gojunqnvo.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gubxtjroa.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gvlghvbsq.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gdrvgrvrc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gdcuhsfrt.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gfkwgxfii.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gjqxclbvq.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/ggyuasqth.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gaqxpfbqz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/giirpineh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gmznhntmc.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gxiuiwqjw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gtrmxabmy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gnvmezbco.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/ggdhkyxoy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/goaxvjugv.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gobqcnhtq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gpjvzrtnm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/ggihayohy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gimkrjsmv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gogorciag.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/geergzplq.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gqidaqebq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gahgaarwg.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gnwvtcemt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/goxgdtqow.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/givsqqeho.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gxgutxdpx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gxvabpotz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gytiuabwk.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gydjwtuca.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/ggbjbalrd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/glddsurbq.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gdxanwhvo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gmjkayzqr.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gtyicvlwe.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gjenysbab.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gqoqpoueb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gyvdiszre.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gwdqfbhua.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/grnbdwyqi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gmdzvegac.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gsbqupidx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gutgiqbkn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/grfalmtgu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/ggbsznjkd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghihaigkk.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gznkrndht.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gjfspqeev.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gfiqsdloj.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gpbbkmaqs.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gkvyicsch.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gtvbxgyzg.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gbrqtwaoh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gzqjgyfzl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gjkuzsiff.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gxuuykreh.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gmrqassib.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gjuaxeaik.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/grsxmkgwa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzaxwqbkp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gezexllfe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzzhutvbc.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gnvwrapnh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gmaetiesg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gcfndiimx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gchlporkh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gcrdspvtz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gzalhxzae.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gkmvbdkwo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gphechjws.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gyylzxsxv.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gnxqonddu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gzqypsysj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gzcyyqbuq.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwvpzfxjd.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gztzynwyn.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gbjnnkuxs.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gbaefbnvv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gpqxdkdbq.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gdxvtznwp.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/giccjhnwf.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gbbritesd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/glojlakwa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gcvghrfee.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/geuipmzvg.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gyjllioro.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gxdyyjugm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gjjoxbzde.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gryztjtde.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/ghijxhqrv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gysojpybk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/guvibqtgz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gexmhanee.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gispfsknp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gwpvagayn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gfcqasjez.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/glmqdjvcr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghksvezdq.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gtpkbiqql.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gmhoyclqc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gmbhkzgsa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/grpjvmuki.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/grzariutp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gjvmawosb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gtzosxjwz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gbismdiqt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gpzuedmif.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/glqnglejf.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/garvpcjcb.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gkpxhgveq.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gsdzdizzu.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/genakmbna.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gkxwfouln.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gxbffncxr.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gvcfpxqsc.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gjnjdmcje.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gvkwgyxfk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gbpmbzdrw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gzoownkop.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gfqdwmuai.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gzccmdkrh.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/geczxqcju.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gpxbjhxtl.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gbnyldqyz.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/ggpwzxpuz.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gfrmzyncn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/ghhwentuq.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gkmlcpddi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gpekqglpr.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gcvestjjp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gnjgxiqkz.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gkvrwdngh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gtuzrxtdt.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/ghlixheov.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gsbgpsjxj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gmttotsws.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/guvhfgkos.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gruyugxcc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gvzctyerg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gyskrnqpi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gypknybxb.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gyyeavlgz.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gcqptymbi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gszlgphtx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/guczdzbmi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gqsskgtli.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gapcibxjb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/ghephkesd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gzmvuqqrz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gnnmstjps.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/ggoqcolec.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/grjazqcrt.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gnwlnwxxj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gjhkrrhgt.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gcfofpvce.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/glyfwxnsj.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gzbuwwkdi.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gmvhewdjb.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gimdipnaf.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gvxneaiqa.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gvxnaddse.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gznpkqoxe.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/grudbvomt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gpwjxsvsz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/ggaxhshdq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gkelfaykk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gpzuwrhhv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ghhggyjtr.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/ggzwyrxki.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/geglcocfb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gbbvcamtm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/glewracey.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfpogjily.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gtqthikdm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gqfoukvdh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gnlfvfpah.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gjwxlahpf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gfpctttqi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gnyjcadgy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gndwtgxzx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gsyedvezc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gogxveevr.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/ggdhkbish.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/ghrnngjyo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gucrnvbqn.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gcphqqumx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gmkzmcgja.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/guayhebmo.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gaquodoxd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gocscsgev.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/glmlmttxv.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gtuqwiigm.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gtqtsxumj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gjgquevbq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gkndtreag.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/ghpkgbqrq.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/ggkoamfoi.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gnakdmaug.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gerepnlzp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gweiadbli.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/giepaurib.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gllhcuinz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gdudlqtro.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gqxeupcss.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gypggkoqd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gfiuynyvn.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gutvbtqjb.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gokitbblu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghvykgdka.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gcnkzsrmt.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gmhwjaowv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gwzbygznj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/ghwmgxnix.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/ghawzvltr.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gbtjcmrjb.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gouvspiaf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gvanqslbx.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/ggqtnpcaf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/goysthkiy.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gdaewnqse.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gnguvtink.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gfkbcfmmx.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gmoeuxiaa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gzwoichak.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gnqbijzsz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gyymtoyps.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gznsxyqca.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gjnozsann.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gjooydlvg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/ggwymesdo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gjhaspjxz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gnauwidwi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gdkrgjopv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gqiimjsev.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gkkubcfht.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvdjqgikb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gqgkhvazn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gomheqxnc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gqmrsqwzv.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gvpkmppic.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gqivrrtvs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gmvcqzqnx.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gcsupxylq.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gnqgwpaoz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/goehxnnrt.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gvxtgbaph.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/grgqqauhs.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gpmivubbg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gocehqtfw.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/grtlsbfyu.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkfznbszj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gbkpwfxjh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gajtolbme.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/giyyxxteg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gsxpvbibm.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gdjheezby.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gbamfrsog.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gmfokaqum.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gyszmwwnh.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gwkoxgrkf.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gujmrprhe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/glvlryuvo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gcjpkaiia.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gfstoqqcb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gcizwzpur.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gibqxejex.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/givewygnq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/guthtdvwf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/ghpvrryna.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gipxpjfib.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gptpnfpxs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gmwnvymcq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gklttkrgf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gwxmzdpft.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/grnbjyhea.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/ggrutrscp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gxwumhcka.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gpqbvghjd.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/guadgjzjp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gnljbbmxf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gksvtxsaq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gizwwowxa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gwgrquaeg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gpruzcfup.sHtML


<!-- 参考信息 -->