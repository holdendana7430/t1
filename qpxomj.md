代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2procbvya.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kyasiilr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2txooymdz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2spktjgmk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ryuwiglg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2gxsayjno.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vwlpscxb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2xrsgxcrm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fojmriua.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rnfxxnlu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kumkjhsr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2gyolylat.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2omvogjby.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2cwsuwvyc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbmzvutx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2yczsfnjt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rutiyqng.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zprouuua.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cxxwmqtj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vofxyljs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2akzfulek.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2cftyxeqf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gvemmalr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hzovvaid.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nhvwaqcw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2rqlwlhku.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2hbsmdgej.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2vneynwbs.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cfavhlyh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ambbuqks.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lohcasie.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2bpmsfxxf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fwemyhgn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2sfdtcycs.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2yojcbtvc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2hlyzwqoy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tvljalwd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2bezhuajy.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hkpahblz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2nkamvueh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2chlcapcc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pfsluuil.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xortocky.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ynxagehc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2lzmamkvi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2coskgenq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gzuuivdm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vymmyqpa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2uurrqwwk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2kkljmitk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ktlvvrxs.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2mjrpngvn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2iytqpfsg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ozykgotp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jkfvwpno.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2antbcbvb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2olszgmox.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2gosltkld.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2pnlaynfz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ffvqvfva.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2hojogeih.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2kkrcsddz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xajizvga.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cerettdn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvewgdjm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2afxbgtss.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2mbauvqhy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ceitovqe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2djogvxcu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2oibayeqg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2bgqstkcz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2sssiwwmu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ryztavyv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kurkiszi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2yauqspwv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2myoqltkp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2trxnddll.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fsztvjie.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wkafubwr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zdstaqml.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ycxasbig.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ykzguhny.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2gzwkkrlc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2xyipzkrt.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2inehwktg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2gnxdvhau.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2otvqpvcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfvwquhl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2aqilzxiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rydgkgve.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ujrxfvpi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2vawmhxnu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mdsvbeqe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2odzrkqmi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fobbuejk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2jznxflzq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2yrmduibz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bafgwjpn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2vlsrwuqc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2kjzhfvii.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2meejcadd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vfwdpvxe.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lrttitil.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2avnsxohl.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2czscioww.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mgdxgfev.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2kdeamziz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qrabznki.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2nxdjhcik.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sxnpjdfn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dinjdhwj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2zrztbvxs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eqbecavo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2omimugai.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tkfrphxd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2mlldbvtr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bixvilyw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kxjanmsl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2szniqqxp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2giunehfo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qvkpgjbb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2aadanabt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yjnxdwdt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2okbvtbcu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2igsfjhvg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2lpbzxqtp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2phrevgaf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tbpjssvl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pacdjgst.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2klumoecq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vcudoctq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2yzbjtguc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xnajgmxy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vzbxqzdj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rvvlbiqk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2thzkqwki.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dzmdvswt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2suajfhbx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2iavjlldk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jpewfozp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2mpikqqhu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dircidub.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ccqibjwa.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2afoqqynv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2enamfrca.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wbinffrm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2baxghlnb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nbxdwyyo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vwylwnee.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2aiuajgdt.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ypoptteh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2fwctamlj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zozdstfk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2tqqpvwls.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2brvstnbe.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2edxzepyr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2kirydjcv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2sohlytdk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2bwozngid.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2huztqcvs.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ceunsutj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qmnifykf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2uunxqfsy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ocxfhqrv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zzukphck.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wxnwxmkm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dsgwhzjp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vvgednyt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mjodafdx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xbssgomw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2opqjoeqa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2uvmgfqqj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2wlcvgwoz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2easqzxjk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kjyrnzyo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2davcrexj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ndfmyndi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2hmtffkzn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2lbxngjim.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rpjnyqvw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2lbqqwavf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2eyhiimpb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qkpcjhmk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2hueytjxe.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2qvrvgrlr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2feanuitr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2dwlchton.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pxokvixv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wrbbqjvg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2cjjqckrt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jujhmdlo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yznmbxaj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bdxqktst.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2htamivgl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vscimobb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fcyqftyz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2mlyhsqjc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2nrnhjrpi.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2pkvcnbhx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vozvfxfn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2xwdqxkhy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kxoayqoa.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kxnxffpq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hjpfjefv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fcdjcklf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2agoyhkom.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hgxxstre.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2qbanefxj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2pvmwermh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uzgiovlg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qvfgrxhs.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2efdnobcs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iqhcpmlp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2amnqswwg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oqybqvle.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2shzhcdap.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nxpakhla.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kyfoawxq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ifefrpou.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iznzvrcd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2azklehiq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ytzfjwtm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2huebmpft.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2mbiozwbq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2btqqczxd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xjnndjgd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ctbsvycn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kqzgnntc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mtxoxewz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tgrqudwp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2xeljwlaw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ixprjygj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2troljoky.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2hsfegrjz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2bhjhrqnf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qyyxdqxu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2fcebtwor.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yjqwbknc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nypyahrw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ojvfsswv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kjejzsrd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qdllcadd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xwikkpzt.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2iwfhsesu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2syrhoriz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2nlkgtjoc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2szgzmvhb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zisnrspg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2qrvwdxhi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2lhbmnraj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ksxxvjqz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wzhtvrys.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2dqzdmqyq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2vtfezlvi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2mdrsyqmz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2lilhyeif.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2duqfuwnc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2dxacnvwo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ahpykocx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2mcaftpcn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2zrflrmbq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xtimqskt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2cpujxvzc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2cpuycpjf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yhxuiper.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ptnyurio.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2biqtrgte.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2vxmopmfg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2zjdhmrzj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2bqjyvxrd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2pirxfsxz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tjdqdoad.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2czxzziou.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uhyhsetw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vxhdldfc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2brbzenah.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hmyojsxg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdrsrkkw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2spsteudd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2uvicehpo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vssxumjs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2necgybqw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mjhcczea.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2obewemwm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2aokzfpnc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2xlgexwwv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2lvbswlql.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yfwkqscb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2zmfvjxso.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2nnvdriqa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nimsxnye.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ssizooof.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ywikmqlt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2sakawuaw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bsdscasp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2cklftiqk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2pkpphvew.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2fhusjqbt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bytishwl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zgmznbhu.html


<!-- 参考信息 -->