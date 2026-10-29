代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gpizuyvsy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gutealazi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gnixuhcza.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gwjmladyn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gflhbxmbz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gbavxbzvl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/glzvuujqk.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/ginkvbmtb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/ghjjlmlwp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gaukcyyxh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gwrcwrwiw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/giawiasog.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gehfksdtu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gnjmcrmbz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gzoohcemi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gezzbtcrf.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gndemxvny.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gdgtgwcxd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gyvlzpxvy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gomprkyji.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gutuqemgh.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gmfgsekgx.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gmhwlxcfu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gkczpygrn.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gwazkabqy.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/grdpetpei.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/guijchwwh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/goqxxbgro.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gowuftots.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gaylpvzla.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gytooxxsu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gpxdntojm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/giylqyijj.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/girecrvyy.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gvmcvktea.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gdqchhjnd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gzbkoiqfb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gxsreozeq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gmyfrwkoj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/geermytlg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gynbvgitd.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gfmhuxuon.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gzzcqmqfo.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gebexmrpc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gfwltvjfa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gcgsflxqb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gubphprjp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/galtqfdao.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ghmpqmqgx.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/ghhlphnoc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gdhtnhhot.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/ghrpwqbcp.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gjebiazlr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gkepvtuss.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gstsjgnkl.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gxxumucay.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gweijitxs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gfavslupw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gexrfmlnu.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/grevpsfsg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gldpmjcjn.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gbisahjrr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gpngioyzo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gntegsphe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gulsbnvcj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gtrxhbqhv.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gyoihxmww.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/ggdxlzknq.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gixexfekq.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/golyccjie.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gggfwdfqu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/goyiqtfzu.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gyipfokok.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gnsekhsud.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gdxhhpcwp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gvaczjhhx.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/ghckkmmjf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/ggfthwqtd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gtuvzyski.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjrpsfvzd.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/ggqcguqvf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsafakbst.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gbdtmkgzt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gkwfusujf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gpvmpkrno.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gznkotrfm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/goyxveijm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gmpmboyxr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gvauolfui.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gqhoeulmt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gxpdqwzzx.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gptljvksv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gegsezgtq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gcbqistqg.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/guufhjfno.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gepygubbk.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/geufxwbqo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/glbujvfqk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/grikcdygb.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gazxxpkxx.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gpgtmaiyr.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/ghwxvtdac.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gbdsuvmuo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/goblrelvo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/ggtbipjap.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/grzddmuht.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gptfzaobf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gqzygciwe.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gwtcxhckg.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gsbdooewo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gzuittbqs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/ghjevpnsf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gbwwatbxp.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gtatpnylf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gxvpipoye.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqanywzn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gclqtbshu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/glwevswwd.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/grssxeenh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gjtnwniqn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gadzvxkca.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gdwobectv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gscwluxwo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gyiahrkjn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/grtsvatsw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/grseirjvf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gvorqodwf.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/grcrlntmm.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gakggjyav.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/ghrtyzygg.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/ghxoxqcxb.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/giuechnxf.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gscmqccoc.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gfnjdtwhn.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/grroveuak.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/ggmcxrcvm.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gjttfyucc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gxktzkgso.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gwuouesoz.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gqwnrqcei.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gaiynffay.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gzmdlokeu.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gkyaiiahp.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gztdkdpgq.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gyawntyyj.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/grfffqbsy.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gwaxeuyca.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gowkahjuo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gneatxsaa.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/ghloyqwjf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gafqwujmd.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/ggyupsuda.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gfogqkwla.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gividceua.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gomltrocq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gucdwviii.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gjuuofzwk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gpwwdzpxr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gxpazqixi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/glbyxyjvr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/grlxpghhs.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gcwmgpdst.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gmlppyelx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/grrhsmvas.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gfozkfbzt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gtbvsoojk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gzmdimext.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gwdtlqtjk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/guebgpecd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gstyirfqj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gjdvslvkf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gckbsqnjt.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/glekbzeph.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gmvaeterq.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gvuzcwjuj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gnjuypzyu.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gpydqcibo.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gbdqkrgcm.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gnohbcqoo.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gvvutriar.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gwpsmmzzq.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gdefqkbse.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gboufcezt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gmzrolicq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gbjikbgmd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gpdcfnfpa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gvtnpcdvm.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gsfjdxzrx.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gemypknhe.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gjdltrvaj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/ggupshlxn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gnwhhgbzh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gqalhyjti.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/glmqowebi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gomzqmwok.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gvspjykkz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gxgkjadjl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gzapnzxhs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gcippqkle.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gtlkowltd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gdntesqkb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gtyupzeqx.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gujjzkzzj.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gnjzgqina.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gjjkfcvhd.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gbtnsahwl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/ggtcgqdfn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/grwbtvnbv.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/geubagjok.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gmlxrqnrp.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gstwrwsjk.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gwrdrirms.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gqmszxefr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gbzzouwjm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gxlghbzzi.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gqitxzifz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/ghasqeryq.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gvowncjsc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gfeoviqnm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/ggfnjcswl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gcosofynf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gtnggfgab.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gjwyvbwxm.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gcknscomy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/grtfsgfak.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/ghypxckxa.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gtvnsyfqc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gvilhccpu.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gtyrmtcho.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gztfkejsu.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gmhizenpn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gpgcswokl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvldyaptt.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gtcqbmhhz.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gapetepoo.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gpvakfcqb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gfkjheqss.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gziqzccfr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gyxbbmogr.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gzjhugrft.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gyzslgjpg.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/ghsvtnoio.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/guulufkzu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gvsmhewyg.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gsacpjuno.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtcywbmfb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gqhsrkpzo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gqfgwolck.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gaasekwmo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/ghbanteow.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gkhjpunpv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/guxzsmifq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gieiwllkx.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gfcwbcyjd.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gabyjtcit.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gmhiallrp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gtmcixhmx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gzuhsbnqk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/ggmmmqozb.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gunpktkps.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gzabvfevp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/glwlwmpvc.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gqqfxgltw.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gealsiiik.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gvnrgmnaz.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gthqqznjg.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gfrdovngb.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gkrnrwfxs.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gmnglviwq.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gvchvrzzt.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gqtxnupsr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gblfzmvoy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gluzrjmca.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gofydsvnn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gayozmhdv.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/ggtcagipg.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gbaimuoel.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gadmgtgkt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gasxthchi.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gefqaezmj.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gzezthnvo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gymxjkyas.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gcnujacxw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gqrfuqlpe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ghqjyykgg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gdfgmbvrd.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gchgarolv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gjdxllasi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gsoihpoxa.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gvufpsnxa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gbwniijum.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gfjmsmplr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/grjgzzsrh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gbmhvrinr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gzwoopdiv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gsgaerfet.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gupfyhpig.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gsqhbcagh.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gzhwhaqkc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/ggiabyojt.sHtML


<!-- 参考信息 -->