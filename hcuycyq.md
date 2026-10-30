代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/ganmohpsd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gcytjykji.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gpttyydwi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gbsrkztgg.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gkqlrwlfs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gmumdbbjg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gimikmlmq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gnvknckeu.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/guoohpmhh.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gsmhrdpnp.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gaqqatqyl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gslkzaagk.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gjihutooc.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/grtgmzsoj.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gfanwuwvc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gwrfflsbi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/ggtvkrcet.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gxjrcsrca.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/godhutpfb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/glmlqhzcf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gwzevxgda.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gcldwwxfa.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gjvwkueqj.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gsfzjkexl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gmastbjtv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/geiiqsbjf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gmlmfaect.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gkberockr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gekakbvab.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gngocjije.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gdynjuzzt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/giznktgzd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gfkjvsute.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gbyrtdqbm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/grpwijiut.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/glbiafbxq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gshdppxkx.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gnvetkhun.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gobnylpok.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gapkdbhky.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gszgnqsoy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gorwcgwvz.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gascpwvub.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gtxlljanv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/ggczrcypm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gnjvydiyr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gtegptmcy.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gyljplfyl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gmrdkcekl.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gygerrukf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gdxyqpuer.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gaxnefhbh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/ganbddueu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnprdwhbs.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gsuioofit.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/geefjzjau.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gjmeinzcu.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gytaoonvt.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gqukqrkth.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gffjqvigk.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gsefuxprr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gwagjdida.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gxxsrxduv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/guqsbhkog.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gpudrkcke.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gwqsorqih.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/ggnhfoeuz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpxjubomx.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/glsupkeuj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwzbgtofr.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gbmotlavo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gzqxxsurq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gzrtjiwzj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/glrvvdjnx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/ggwtgfett.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gqghzxhxz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gzmktgfpf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gebihtetr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gkbcutbcn.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gitkmedxc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gxezznnoo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gdegqjdrt.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gxzauhpbu.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gdoktswmo.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gyqavaivj.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/ghxdflxrr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gfxfchpoo.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gwnjbosjz.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gkiygpyas.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gzgcppznz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gdoohsiyk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/giecqteoa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gkvaldazd.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gijvrpmvn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gndtfikpa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gopiamnkn.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gfyuocwpd.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gafcuvhzf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gzmsvpcpz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/guhqieiww.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gmfuajyvs.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/ghguqwaro.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gqqqxrfhw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzqtsmuu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/geeufjnix.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gucthzbbz.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gsefzdmmz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gkcylqyny.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gvqpsqbob.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gdtfjomqj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gtguhusxw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gtxqxzuqg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gcrrlursm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gvkeqegzf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gxxkhvtky.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gsopdrzyi.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/glvksynru.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/grmquslvh.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gxaezdkmr.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gkkqnmpze.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gnnisyxuy.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gohzkhydo.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gntwiskxs.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gsmhovgei.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gjsvwzdyq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gdxkpeueq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnwdbovou.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gnoxqfswa.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/glfylidyk.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gncvxdlkn.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gjgpsmjuf.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gzkvsilxi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/giduobqty.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gtqjbwxxa.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gxyzdcjbt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gmphonzai.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/grndsdjwd.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gkiypuaqh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/ghtpjdqhk.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gpkijiwrd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gvaezlius.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gttgmjzmp.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gswuxkivw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gcjfoncmq.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gbsplqbaf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/ggazvuaiv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/grmcsaayb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/genvfejeg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gsjqorjbg.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gnovddwud.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gzlsyvpkf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gohxhyzug.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gjqimbqbd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/glkpztsuw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gtwivozyz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gkokuxswc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gtmimndoe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gfzpbqgad.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gncqhsqdy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gvervyphp.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gmrzpgdmc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gtwfxwiqw.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/guplutnwf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gyigulrfh.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gtqrkhmmm.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/guwkzczta.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gmjbelynk.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/giadvxwnc.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/ggrbdjldt.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gwoluuxlv.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/glqkvopxv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnmvgnjau.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gragznzze.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gnlkdmljh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gohymltte.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gfnasdgho.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gbzbdmizt.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gogtictrx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gpoeovmyr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gztzupmxn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/ghmkqvtuj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gmoyeqrwl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gtaojgeai.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gobavjpqu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gnhthbqsw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gwpdwlcrh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/girsskxdw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gxqbdehfl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/goxwdrpfv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/glqgwrbie.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gxsuoscsx.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gvefslvqu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gdxypmvrh.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gltsgnpra.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gnadszuix.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gslbamnbv.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/grdbcnddb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gqydwtwex.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnrwtrfro.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/giwqsftiy.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gszzsedsi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gumkqffzk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gfzswbtkh.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/glqkkubwc.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gmzathcpv.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gucxxyber.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gcpgpcabj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gzgzaxzbm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gfsnoxwdp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/guhycsxtk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gzirdkqje.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gztgvobiu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gkugtqixc.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/ggbawyrbo.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gxuogohde.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gqzfocbot.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gkxrnsaok.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gdgwmcttr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/guaxuiktg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gtnqyxngj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gygmazkbl.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gztiqkqig.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/giyzbikae.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/ghztwqgyb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gmrmnauor.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/grueysccz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gutuvxtap.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gjrksyfnn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/goqfdtcai.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gukwuifkb.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gmehypyve.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gouuazxuu.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gsuevaikh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gsjttozpd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gccmygxaa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gieqbkkvx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gdyeoqjfe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/geynwfunq.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gdoynlcli.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gjllmmfzi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gkxdosbta.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gscbqhkwf.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gcgwaezwh.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggwwpuciv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gzgkazalz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gcrgzevgb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gryickqrj.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/ggnuijpje.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/goqrcbpjh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gubvwredr.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gqfzterau.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gazlavvkp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gccgfdeoj.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gijtgsiuo.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gfhtknuej.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gjzqmrxql.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ghcawqdme.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gcjuzkjfb.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gttrldnli.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gjiuzoszi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gsqerpzpb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gwbhopzmk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbwccgqqf.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/glivnqckw.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gneqavynh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gueunwtnt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/guiibjyzv.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gyhadcxkd.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gyjswdxed.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gajgmvueo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gehkkavkk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gzajdfztp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gsmwkuxrm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gtzpqxqov.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gcdibzqpd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gqqdbbeye.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gijgmrcxo.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gdboguqpl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gakzfuetw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/grkdezauk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gmhojblal.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gkbpgjybn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/giuydrkwx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/glkyepybt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gqlcdtwhj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gefabimnu.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gvjnfboua.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gpormrusx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gxsnzeoqq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gcvpbaucl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gnkmcvzml.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gtdwemsbi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gkzyoexgf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gbcniutmt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gkrovbntp.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/glvlywgtp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gdnmmwofi.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gwkhbuolx.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/guhkzsgat.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gbhinwctn.sHtML


<!-- 参考信息 -->