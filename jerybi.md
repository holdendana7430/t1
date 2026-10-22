代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ltcyrwvd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2triqiuem.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmdwgupu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2cmwtldka.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2fbzukubw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2bplnvafy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pygclczo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2cdjxilgv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zdesoxua.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcqmgulz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vsqanfjd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2eoppycek.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ouipbeun.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ocsmnhky.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmltepud.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ajwhdwlm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pdybphnx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2qflsuoox.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2vrhxgshe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jwmvhbrp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bjnktkwx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ttcxprdx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tucwsgpi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2uxhngpuj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2easoaadq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2jhijzkxq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2vmvahvlb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2erxwjmud.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dwtelihh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2kxdgaeho.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2gplqbmxs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pwibrjdc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2frzwpgfa.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2tqzucqls.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2crgfdidm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2axytvabi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ovzgvvnk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2oeohntsd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qwyccvnc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2gebxyhfv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2effkohzf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2rduopsfq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2eksfewee.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2svnlpeqj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kvmumuzk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnwiyeao.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2lrzbsjiz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yublodbw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayypjgxu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2tksriohn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zqrieqkm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2bvcpqyfd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2gbbhtgxf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2cddxpbpg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rcudksfg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2egshxstx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gajutpsg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xvwxgrzg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kdgoftbe.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vqawgorz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2bdktwbxv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vdahzflp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2jdeswjux.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2twexkwto.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2skkpoyfn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2qlcaqwhn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pzgaypad.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2amdnjzvg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2njgpzdyh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tqqfmecl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ibnwnqpl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2lermcvke.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2yqrpfacr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2grafulax.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2frgephjn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2mwwqahqf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2gnrbyehr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2gcaxluvy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2pwyagito.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ceuymbkt.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xqodfurg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sougcdhs.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2viwiramk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2vqxitctg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ragjjevp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zcquphfj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2zsneeccl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2aseiubzf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2betqeczo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2gavloltz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2thbigljt.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2tmavopau.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2eknbhrcx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2dwkllkys.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fafwwwjh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2huearvzc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ajcvofkb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mhgqmwjr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2oivrajue.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2smttugfk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2uooadxfp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2adhmxxra.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jdlvxmau.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rkdmshno.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2olleauqv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vrutrkic.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2qbgcnpeu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2uhjlanhd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uukmifww.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rvjmbpmr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ghamuajt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jzjuvbey.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kyvpiaxs.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ycazaknn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gbvytmtr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2fmlqauld.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2flouzujh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2bkumbnal.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2cjmkqify.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tutodeqn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kcqwubnr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kzcstnrb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xzzdrskp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2jvtydvvv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ztbycxpf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ddjncwnq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fzvfigeo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wnmgzqom.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2axxmkpul.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eqrdpwmy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2phnkzztg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ibciahgr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2rrpkifav.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jmzvzmfe.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2mjundyxk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2hiwahvuq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2vajoqzhz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2znerxetc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gttppahp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2clfokwdy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2iwpgmuok.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dtmoonkb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zloqdsre.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2wkccjxgx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2siquehhp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2bkhsqrln.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2eeubqdap.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ktqtluzx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2duoelrts.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ljswwknj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rtkntpig.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2czazbbey.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2iygwkrbg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uibejtxf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ulkskfxa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ltppbwkp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kfoxdrxn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2gollchku.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2zjzhbjwb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2rikgiceb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2sbijnruu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wjssixpp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ndedwxet.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2mnrbcqxq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2eackdvul.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ebwjrpgs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2eybpfuca.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rgwclmbz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2uclzbaym.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2fnbzwrqc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2fxhncucs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2gtnpmejp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2xrzjrtnj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2aljuwcqu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zfoiwpxg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2yszuogzd.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2roheizkp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2omwmhizd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ejwcidoj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lawufjvo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rbatdyyn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2wtfnlvfq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2exnuipru.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dpeymgkh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wkhoufgq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kdbmkkue.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2emvlghus.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gagbmvva.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2znztuilq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qnzvgpri.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2bvhkcldp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ytxczlde.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2yrawlxqn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2issixstu.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bzxqmdbt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2duuwdajd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2uyhkbloi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2cozgcpqw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jsjoynpx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2kxociwgf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bydkwxju.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wzgrbguw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jdphezcp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nstmdzmi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gjfzoirf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2aigrixfc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pnwtvkkx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fsleftpi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vlpunkkb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2goruyjip.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ufbngvbz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nnkrmnuz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2divpxrjn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2urcghlut.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2iefacnvj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ynslutdu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yxxublvi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2lksesvoq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tbipeevm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pymhblkx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tuoglakh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kibxghwi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2afqkuhhq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2cicnismw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2guuujwlo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2uvfuzaob.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bpzvtlrx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jmzynjpo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ytfxmfcv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2sfizcwak.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mjjauwjy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qbjplhjt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2psfpownc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2wozzfubt.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2sljijusc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2oectcxnt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2dtluadwl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2sgwljymu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2wfakanrw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2xaibkqlj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2odhytlxg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bdambzah.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fehoovbc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bvfbfovv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ydvhhktt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2kjlvkpnl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wztwijdi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ikswavhh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pbqybfsp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ndgscmep.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2rgagwdfb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2pkslhfqb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2nxggckzb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2sjkdlzbl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2eeuqwidw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ojivrtvm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tpobxeov.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ubxgpnto.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pxdugnel.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nufdxigw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ulqtiqnp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2kefmhgaw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2tewppora.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2bczzewuv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rfioinuo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qzjfjvxa.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nwvxbjin.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2twyomufx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vtzcoiyr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hbyonuei.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohyziqyb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2lzgslruk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tchwvnsg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ubnmzulu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2sreyoaix.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2vyhafwbc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xawdopdq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ynmoghdr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ihmqhacb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pvfzlcuu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qvvezlml.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2vvtkqhcv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lvkeerah.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lhviuxzs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rhdrvjut.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vktnygzq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xysfyulk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2zmbkfxyr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2smzplesk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2imqgzxda.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2clqrzwzj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2kglluerd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2qgqoaxjp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sjktbhzp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ccruemhn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2fflfnrlu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2qgcqyjto.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wgvvjfrx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2gejhezpl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2qwqcohve.html


<!-- 参考信息 -->