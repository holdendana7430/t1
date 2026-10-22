代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2povupanc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kawjwaxg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjyqprsp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2byuptsuh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ygdbtbxw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2tovkhxcd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbqijfxn.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2szbbsgcz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2iurameqp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpsypiiq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mgweskgm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dhgqcelt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vjjczgxj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2zrewlbvj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gvkzsukv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sivaimao.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ulgemmac.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2khnxypex.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zwshyzvx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cyneprkl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2fijmxasr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pzqijexn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kbbquyzc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2barsaqbl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oxowqvqq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yrragbvx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2enggsldu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hucvwdjs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2iiqjgxel.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2boxuvcmk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ewepjewy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2zfduzvvn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2veuyclzl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jaoyniwa.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2rxfpdkwc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2zvpjlmgw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ptnjgkzm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dgxpkfly.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2znggwzty.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2dopikibv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2oktlxynf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2zdcydumm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uwhgwqvn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2hmrdfjby.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jjeqkllm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vewcloxj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jvxiztua.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnhdtbuv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvrphhht.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2xxvnedgl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xhgxrsbc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2atkrlrnx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2upuuusyk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ckvhmojc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uianysee.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ufmjzsbh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2avmwzthu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2snpbbdps.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2wxxkwsxd.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tajtmnaa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2uidlvjtf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ehnldkmh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2eoedjzkj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gnirywsy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2semwvwyy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjuqghmg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gpjffkfz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gjakprel.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2bhvwlmmt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fvzrtkkn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qcqezyqv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2cihiwmfb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2rodbsdua.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ctfqiyyr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fawsuxna.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwnkjzho.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2idlmznwx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2wizwhibs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2tpvisfrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whrfwhgv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2fxvsusba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aotdjszd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dggnoymw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zovxltlq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wprkxtcs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xchnwrrz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2amycgklz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2zdvojkjx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2xfcenaoi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2umqrgmbu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mitmnufi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ludzlqxn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2scmcnltr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2pkafnvrc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2emkeyrge.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ihfalknw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2vuuhghvc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2pfuetqur.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2xyicaykg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ztjjgydn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2tmsikovo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rypvelnf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ifwwrdsx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2atjsnrwo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2meejvurs.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gohrvavv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rolurwmp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ckqcoxgb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gjmhbwne.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xlkatfli.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ydjmlgtu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dsiiqbcz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kbjcuqxy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2phoytswu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2iccvoten.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2vshzvqyn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2enmoelhq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2nubzsvyu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2bgzqbmsd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xitvyjqh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2extgbiiq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hupawjlj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2quhpihpn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dqdbylup.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gswfozqy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xclqioli.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yyreajpr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2sqadysia.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uygmxsej.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dwboifmo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tqtlfttx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wmsscfkv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2cjgabpvb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qzpwdrqq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2iyhwxicn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2urtfttyu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jqysvnyj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2resenqmq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2puvbnkbe.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ouuiyuhx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xmyplktl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vunpixxo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2klqgsjta.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2queqpfqw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hgkfaocv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2udqmosfj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2lmwgntth.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2uqxqvilc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2mctomnmd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rjqqfrrj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ieoyhoby.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ohjcayqi.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ykumahts.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bthhrqdx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2wfsgasag.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2azdspnli.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2cgqerseq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ixjjhhbb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bzgbeovv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ljgzrjcu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gxdyfixv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2owwwfivk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2uczrqawp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2zqjzmrln.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2mekxooyj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xcprosqt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2isccvqxa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2akgvplzj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2tirdisrr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ogbrqqoe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2owstmten.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2pwvmubxa.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2uasgpgyw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2togvixmw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iagmljbh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2uagxcmfr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2nohshhur.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2knrnjlhg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hjnioaha.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ncqiuevt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2cihzrazu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2srmajpyh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bijmeboa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zdmvqzdm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ywbiywmm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2clcuttij.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2farwarmg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ckluwehn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2guervvjw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2icqadrsf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2zkbcyfrf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aepuxyuo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bjxgayjk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxgzfvvh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cghkdhlr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2dcjafwep.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fhtaodcy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2moueagcj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ljwbbzfu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2icgozfel.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2aiczhssk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2quzgxsur.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aaprzngy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2osbjdkgm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qbbduwwa.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yugxwxqh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rdlulovp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ghldmgtl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nyeuuspf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2extaayge.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2aezykoxj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qqrgdcil.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cfvfqxvq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2erfhluzd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2mdtsbzqb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2vqkxroal.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bpzxovio.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2kambjcze.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aihhcpan.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2siupnbda.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nasbbkpz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uatiyznr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2rrjaozqo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2tcksabuf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2oodxohhl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2aqwgijoa.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zpewenak.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gqhvcosf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gnrsprrm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2zvduszeq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fvfbwlvt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mgdryily.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dqvigmde.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2swdwbuyy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2pgtthytd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ulihutwe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zazphkoh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2psstloxw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2spfroiqn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vbbiruzr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2accvpojm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vincvfgl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2nlehgeju.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2utvkhtyn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2gwuavssg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mnrsxjeh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vvyparez.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ouvqezgs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jfygmqjh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2hpockttj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2naldngwh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2fkehzsgr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mqcysyji.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2vcqoqcen.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2iznsviue.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fanqqizj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2szwsmekq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2dxplgvxu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hdhsnjzm.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2zhxsbxrh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2qloyopxk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2btqitoeu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2uggerjui.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2deumscsw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2yqukyhlm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xbtaeoya.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qsujvvik.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pgtdzpmm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yovxafgo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdkdjluk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2equpqxeh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qfzpokfe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ckswylgi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nspkhpfz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2smjmofon.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2iqigpbsd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fcvkutvt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2tpfdfxcr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ithqcqgk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bocgrmnz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rwcwnyyf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2emiisgjb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2eryoikwx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fbfyifzo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xhxergwc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2esrxlmpx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2apqcvney.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2skrtwsmm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ijujuufe.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ppwugsqb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2iorvgldh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2giuuczve.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2nfzzengs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tqmrzijv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wuqiedlq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2vajkyqsp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bydlwpoq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2zymymjtn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fpvbqifx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2soydbdpr.html


<!-- 参考信息 -->