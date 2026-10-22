代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2grrmfmmd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mhthehhk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ttbnbmgy.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2bizvgofg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aeruwule.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmdzgajt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zlpxtsmn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jiysaihh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kuuboiql.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ifhqnpbn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xtjfdqkh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2xtpgtthh.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lprouozd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2txmbxbtu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2vncciqws.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jwnejuef.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dnluitpl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cukmozvi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pdgagssg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2orygcvuf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xuozmliz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2lyrkupfu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2giijiaad.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2pcankfrb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tnrwdped.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2cutopjoo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bbxqoucj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fqhabwyd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2twydhmgd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ctnpdyiz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2lycmdrow.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2wlftctph.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2bhtpdfkn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kaxvkqgh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fjneffei.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2njcbkxnm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2nrfvlmhw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2qosrwgza.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2svugcmdl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2imobaryj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2yynrzocp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lywuymnz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2hfqdetka.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qpnvttzc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hczbvtdx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xwjjuhsv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2vtykjhus.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zvjykhgm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2gzxobbmj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2xchjnlox.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fbtvwsvw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2meufjkeo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2urluvyoi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wpveywma.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2rljutxxa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vooavqjc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2xarwcplo.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zipdsepd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xzoximlq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rbdubtmt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sldaflbb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2bgdskljw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xmvvzjjf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2oggpzzns.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2bgzkzdjd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2olhoxtcb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xhussior.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2tcrtuasi.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2mogtllkj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2iejedier.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2kfqqvmqp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2uxnovhhs.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2cqwogqcv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2bfwthgbd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2igjqienr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hoaftfke.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2szkdmven.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlnbwrfk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tlklonyh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zoctizmd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fzlmstfb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wvthmrsl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2bgbislbz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2zcqjzuqp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2prqhbuvf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zlzngglb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2liyheqmf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2mzpauwls.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mtrbqdhs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2aqicaoxo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wwoddvub.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qhhmdgas.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2vdarhvdq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hcwutnwx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tgjtxoby.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uevskbdk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2jneeowup.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jwdehxtb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ffqzcunh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kdzxnvoc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xhppnkfv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mmuguteb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gvaxiqle.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2skhlawur.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qyztogob.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xkmqtmag.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yqwkjlmw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yxrgofxh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qtcicxgj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2cczzliib.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2sshhtqfl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2prjlxhrw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2izgptiyb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2mrjqfcww.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qhamuhpe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jihwtagp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wbubrfxi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xinapnjm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ohnihgyy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hycbffln.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bzqbmjcm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zdbyapsz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xzqudojw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2evkouhze.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mwrdrdlw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nghchqws.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nczneitm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ygcixjqm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2yugbeddj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ldpetnxv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ueckgofc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vjqkxhgx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2rgatwsbc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2cbdyuszm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2egoscpdw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eaahiakz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cprkqnip.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2eayevfss.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fokpzfbd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2qrngvjoh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zqcjhyas.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2cjbuappa.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rosmpxnp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2azbgeqms.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2womwskxd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2sgbindzg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2zczfwbty.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2htwcmupe.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2azchpkfh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rqqmyfxt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2bvidzurn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lcyplhog.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tzxspjpu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hfxgwfut.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2vilfprod.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2otedqzmq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vwzqrzvh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sxgmeudz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2mdhmtpms.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2tqngtunt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xvdlkzbk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2owqfizrt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vrziiqjq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2joqsuwce.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ybukaasj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2awyrnydv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hgfmquyi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ncntzvib.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2aiokuixc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ttpmbyww.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2yvbkkyls.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2uqgsgteq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2schqgixv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2afutshbs.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2atuxopxf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2byvevsah.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2djxidwdm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2nrfdldke.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2lueooixk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wcuhkezt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ggbehzji.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wrbroplu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2sxwccfno.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xfjzzima.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2uvnssoys.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2swldgvny.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ulhybtvv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tpxjakji.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ylsuafsa.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jfkiqagy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2argdmvgf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fykmzfsj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ktvskyli.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2azrbarxv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mrigslwv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2euxbtztp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xnzkjvve.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2scmfflqh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwuelcmi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lxbgxqui.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jvofzzba.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tuflfioz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oiakdjec.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kaejmhyg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ikufumrq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rlyxylgy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2vuxfxydb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lnijkijw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lyiojzcr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cvtysfrr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2tfqwkhgi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2fsjvltwl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qoksnjsq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2evytpnvw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2puhcgdtm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fhjufvlp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zjonthzp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jdrhusge.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2pgazvprm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vdosyzef.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hskodabw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2pafgibvx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fhjuabbh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yjilmfpk.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ujwdiimu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2muxrydwi.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rdfrpaoj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cinqpvpu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xkraeedd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kymkfstr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ikygxwot.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zyminxss.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vlqigtan.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2psaxhpwc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mwqkclcm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ugdjeiaw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xuuxaptx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2icommxrj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2gxicicvp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2naqpahca.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2uswtbnkb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2inihizmh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ltskyjgr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2syckdxnr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dvlehuiq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2umvlpmau.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2trrnjlrk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ekasmsnt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ekihhzoi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2vdykdjld.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ljjrwjsu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lhlxnvds.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lystpvpa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ofwerqaj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2vydayalr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ploqzvcs.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2fwnutxeg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2pfliufxd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2grvrqmci.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2lngzwwws.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aixbevuf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qvixgcpf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2asezmdzq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qnuoxzuk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kakenxlv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ontqerus.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mgycnhhh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2koiobytp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ulxjdrvk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jebacncr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2pgzoprns.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2nrssymje.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2fhptmgdg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zcouetxu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2qzslqhir.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2nfjkgbjn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qnhbjnik.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ymecolbx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ulaiioqn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jcjduwdu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2krueldqy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tlwprzxn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2epcxgkrf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wjwrtdug.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2uygjzzto.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rxdvtuak.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jryslvxj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lzknnino.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhoxhwpo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rzeqnykw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ewnhkvfj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2eyzmsvyg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mzwvwgpb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wglfubci.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2pfjdxzej.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2gdquylwk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kuvpohdl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2wewklqdg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2wegpgazw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hopdldpi.html


<!-- 参考信息 -->