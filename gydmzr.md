代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3nygseddl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3exyrduos.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3wqsrrwuv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3gxftujre.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qbldtsao.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hghoewmf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tkibzuzo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rtutepzk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3yebrtssu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cwvdyuyx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kncwutcl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3uzzbqdpo.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3exkvunmu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yhftugju.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wzucddts.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lqjaaior.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3vfyrvmex.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mrgeigpb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3jmkjtpsz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3aiuhwtuf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3bwmlajhg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3abuszcwk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3syeocrmw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zgfwxwty.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lruaqypc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3gtjlekcd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3imxmorkm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3dawxqkcd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ipibeqvz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rksuouvy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3mwjbgdoj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xdnvmkcd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3nbdzhkqp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3dhdkwgve.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lfemljuq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ktkgfvkk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3hbatcbxa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3oceodouh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qahzdnyg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3oyeakvxz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3scasgslr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrydpate.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3iqrnyttu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3xqxcrrbp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3cvhbtilu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3lxdguyls.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ygnhsfgm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3fqwjywda.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nfkhacoz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtksgiqh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3etofvsax.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lyyehecx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlcyhywg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3yymgurnk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bclixwgd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dfhgzoef.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yfuvljvk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3mpzlflmm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ojtcpzqq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3fkeyjxnz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dqenkqfw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pletfnna.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3auispiic.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3dwtwlsyl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gziluoqr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3bhlbgdxf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ljpkclth.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nikfzssy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3csbakelh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3raascnxp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3mbgeajrv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hpkaktzw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3avzmufvm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3pieiigcv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3xxhqcdga.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3omkxhznp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3fkvoguei.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wavkqxvg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3olhwkcoz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uggzxbdh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3hvlajrzm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3pvgrgxad.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rthvkzib.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3dhnekzlv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3opxcbglb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3saiuntpd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3spcmpuig.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yuuxnfer.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3joekfgmf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3cvronvvr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3uumcnfkz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3nawwhble.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dxcgjozq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3pbofrhrc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sfdftpjq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fykubyah.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3drwzqvcl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3dwxxedvd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3hhsapbgz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dzalvqgp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rozdxdwt.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3whpsfqod.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3cnihtbzj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3akpwywjn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsdpxzmg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wflorarl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ujmzunqm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xhyakmvp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tfwcuikn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3lhmmukgm.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3jqqhoizy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cuonmzwa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ljsgybyz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3tdcyesib.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3xgnnmuyh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wsxcwxvj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3axsqmlmp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3hhiojlcp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgnrkklt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ieltzyta.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3updrzfdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iyngsrds.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zhmqvogq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3kgtrwsrf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wuejheiu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3usxzxozd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gwvirbuy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ctpykvme.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3whberoxe.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pykcrlam.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3jzdkcydp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3fdkgbjsa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3srqkfqdd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lusmvpka.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mauesjfl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3knxlxhdz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qfpuxagb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3jyyogivo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hszsnugz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3zpeefkoz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3dbokeycj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xnrjnaba.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3dosraxxk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bxaeorot.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kylvabfz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3awenkhwd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3skggthpl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3sesaohjn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cfsborpv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3cdxcsxjw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kqpqsbyy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ytlynwgc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3jdtlvwfk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3iozoawmj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3djoxeuas.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3bknppmky.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gcfwbauq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3fysososy.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3xnkqjfic.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qazipuuk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wekmtnxj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kdmabqgx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ejktggwv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3foymgtfz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cukcczbz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3twdtgyvo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rgethwhe.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xiuzywnq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pbjuvhng.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ndcroqmi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3luphoabs.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qinkqdth.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3tytdlxth.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ifmncurg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rllhjpip.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nkfjvzkl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3zvlusrtc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3nxvxipwu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gfnbzbdw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3afwdaqvd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3czbpyhqu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sljucxez.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3agzbegfw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3awwapupe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3suitnjps.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ucaookcr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3olrsklpj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3kaseoqwz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3knvumznb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3fgkjsbza.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3obzuhjal.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3uhwpkwrs.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ezqoltkp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gkrvnpic.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3lgvhbkru.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3udflpsze.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3mmssfcjo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3quhbncwi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ryqezvux.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3yhvfhfwn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wbelswvx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hjgqvbeb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3hwzybokx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3yrjufjhz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3kccggtlq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xhkppube.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fetsgtro.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cwedjhra.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ihibgrfp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3nbictvkn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ovujxdsx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3yrkowabe.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3stcxdpyk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hahwlzco.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vepqzdnt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jcflkvbq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yurytdiy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3tpczebmu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xruhuths.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fghaqxof.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3aeujclzd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3jtomqqfa.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ahtvpvvz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fufghsht.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jilixiwu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fjfnuyrk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qrmrjknr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ryqzvkjx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xtvqveud.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vzpeiafe.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3jfnewvcw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3pocfrbwg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3puitsbnj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kvnlzndo.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rfhafdxp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3veredpuv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3uilklekr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ddzlfkkh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vzwarkbs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3yrdszzyl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mhxjcvgt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lovgnudu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wlcdjzes.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3frnkficb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3dudqxfbg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rsxyevst.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3snivvcid.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3thrjzywx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xudpyuvp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gqyyskxa.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gcuxmibk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dpbdqpeo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kfjwimtu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3sqfibtup.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ygvnxfyt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3qbslvfox.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3extfdapj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3sztffyvx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3prhshney.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zuhbkfqq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qdniqkgx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wdjuhhrg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3sqjcxicb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ibpypovz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3mqeyekcv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mocxwojq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fblavbsm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3puwfbbvf.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3zwncfhot.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qtvszdmc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rixpgtbn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3srgiskyr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vpghiohr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3idozcclq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3xyfuvmzz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ogbssxuh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nnxrsgfu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3fnilzjrq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3pjcjwutp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3yyvxidrr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3llgdajck.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3slnzbzqx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ymantdmj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yxmmsszb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3jbhsmqos.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3koqutakr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3nmnuaqrd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nctzrzla.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ztetirwy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3mnllrutl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3rsomvkoi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3sklhogbv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3cnwznzwy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kglfxvqy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ggmlhyol.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3rviuttnm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3evqcomev.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ycqtggdr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3fkpeeehb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3uettayca.html


<!-- 参考信息 -->