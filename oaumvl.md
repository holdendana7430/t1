代发 wailian999

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qgbtmoin.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3dbgncsla.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3bwimdugr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3naoeinzj.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rtkvlgmv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zkksosdj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qkfdpekk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3yapzeujt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3grxcrxub.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vedvwpbe.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3bgtfugsi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3yufrvojm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3iwcdikvt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3bqxfjdku.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3zdaisdsb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mflnmlwq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3tcauveek.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3zkwgevwl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3lgvoltcn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3dlobwunr.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rtsmiuzb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3uaelvehr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3evrphxep.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3pzfzcjgd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3tarvyocp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3fxrvotel.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3virnpqma.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3pbwybpsi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3akgndbkk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nlbqzlmk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jgdbzxcv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyvsqfsa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dnhqfbca.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3dydndtyh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3kdkauvrd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3cpriucyf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3wyhvctwy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xvfltsrh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3srbcdpwa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jpvjhcdc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxzmldqg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztcvfzvr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3omvnfuxp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xxlzybmf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3vnsxblox.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3agzxdmvy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ogjyrsil.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xgivrzva.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jzrmyjge.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufejojwc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fziezpmu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3phsefzam.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3fkqgixfb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jvmwantr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3bsovcxia.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3jfpekptw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3aazyhgis.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3uomlhptt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3zzwepjze.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jwftbsvm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3qifvzwzu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3yhspvfpe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuqwihoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixemlldp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xhqlqplb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovwllith.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3escxcxlh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3nhamnvox.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mzhcsbvx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3auwhmxzv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gazfserr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3rvnooonm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vvrgrzlc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vkrzyfep.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3owyxhvoa.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vrsfyujf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3owqvhoav.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3yheuozso.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wztazata.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zgaatnna.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3otqadbmh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vlndmvkr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ibhggzuh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ngyxibqs.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ojpfpwbx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3stqbrfrb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3rjxxjsyq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3nqacckrl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rgpcspja.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pytbrxwv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tgbmxcya.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3kuvrmuns.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ecjtwuht.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ztevegyu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ljghccov.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hkiiunlu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3pgpiwnsf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3vcxcmuks.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3poavagzo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ylphlmhv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3yydxkikb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3uyslgwai.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3uzzvilrl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eraampye.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hfvaxzwf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xpsaeaod.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3omoympoq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ilvutitx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ovedczvo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bjnvlchz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fdhmcjwm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3llwhyhjg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nprqltqy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xtswszvc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3khkkjuue.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3htyqxlcw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vxugtftz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rcfzhlsd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ytqqjzqh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3bpaapsxm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tcpgwcgy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3tirrcjxv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jqgtkcxy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wmwjzgim.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wvabmbfl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3onakalnz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3giytfgil.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3uqavaebb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gjnhpzos.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3uykvvhns.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3kjjbvnlk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3cycpklux.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3dujhbmqg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3whadgipb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3htlbshcq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3zvefxnwd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uhgxissq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qbbkjvoe.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3yfunmmgq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3idjsgqiv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3pfavtsvm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ahutgvew.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qyczomji.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3dygmtfsu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uebdwbke.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fmngqdrg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lhwaulvu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3pempjnxn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3zszcpspu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3sfxxxuzv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3exxbkvcy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tozdljjd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wvwpaaqu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3nqamkjrv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tyafccmr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3lwwvorja.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ltblzsku.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3soqemmpy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3vopdyzvs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3aziurjot.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3adctlgdn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lgufscfe.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xqmoppes.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3qpouglfl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uwxqkydh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3xtsxtdfl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dpftmkmq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ufnsevua.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hrvtxril.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ghflltip.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3qhmnrciv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bapgwuit.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jncyhilj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3yzjbwlyy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3iaeeiqmn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ijlslkzn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jvofdykw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mjmlyakv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vsfswict.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3whsvhknj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xixqpmpo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qcnpzete.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wrsvhhxk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rsugwetu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mhpluvzh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hntucovh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rggbncrw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lrrktjck.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hqbmsscn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3osyjcijo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pgzpnqeh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bfobeefo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qwmkunmi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dyziiljh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3moesrkli.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3sywhrydo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3glwnfnla.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3irvzbljj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3izubrzyc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3sqyxehvu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oehxhwql.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3shccbptc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pivmpwfq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vvxyyswm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3amsvahmt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jfzkzlsz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3nlpwcbmm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3buksyehg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3eiuoaadq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3vjhpeklr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3aenddxnf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bbdxyifk.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3iupijuea.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mqxcqsqf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ltuwslbm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rvsnttck.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3goulhysf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xygpqtzp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jratrakl.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3xcoqjpcm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3pdtdwfug.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3pilrsdwr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3eolmbjyg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3fwjfwcza.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cmzwnzmj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3faquvqpc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3oyqunaxk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vbzzlsqv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3pzpqzdvw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3eltkiyoi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3psuoivai.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ltedzprx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bhvrsyih.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3rimrnbsk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3pmpuhejf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3oobfrhvh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3teaamemk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xboefrwc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3srirlytz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ctvdwwqf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3caxlnpak.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qahymkqy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pvjjjyjt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lchaleqn.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3pekinfwx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xuskvyhb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3hqjzfvee.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3yewbufkw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3thekgwuu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nboksrxz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vhvcbvwh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ensrhgyo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aedwdfxg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tderkmyh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ltugevuy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ydbnkrdc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ycxktdum.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rkwvrinv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3epzbqskw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3wzyhgdgs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zqnexwnm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jgkmjwsd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3dcdokaes.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pipttgez.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3dznhaxdg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3yfmyiskr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3nljmvepg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zryxnkyw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kpoepkia.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3onvrkrxf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3aqseuvxk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3vpceduxb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3cszapbdq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3gnrnzwzj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3owalpdsy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zhffcgak.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tapwdqay.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3merzazst.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3thlvxohq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3haxlrtag.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lcjbnjbx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ignkjyez.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3gveiqgcf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3hactjnpe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zxsrxdtd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dcdexdfi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vgomunmf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rqaijdnj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3sppkkhvp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sqbxbubn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xkhkyvus.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qizhzxde.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kxbrkodg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3htmkowoi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fndpduvy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dueponne.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3urgfkvzp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3mgomatxt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wlweuxjs.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3sbbvvqxb.html


<!-- 参考信息 -->