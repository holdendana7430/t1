代发 wailian999

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3wzudmocl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wleugbaw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ydodzimf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ivzsqmgg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3sdxjbdcx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tcvlunvd.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lvicmxyg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3bprrapmu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uyrwpfxk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3yiofatpw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3uthoscxk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ebtppvmu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wwhpmccx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3nmduhmpr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ppbyllxq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3lupoyjsl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gempdcjq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3opzxqryb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3tfjljmqy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3knnzubmm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3fxvqxaut.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ddbeposj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3eqmlxryd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nvhgwitl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ixqbhbaz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3zgkrrtvd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zrzaimqg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3dlyomyqs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cuzuaorv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3spxtncki.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3tlimxsmr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iaowhpwa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmnjhkpu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3lkigjbsd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3bpebtiwt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3kwkfiodh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3atujkdlx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3atirlzey.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bumoytff.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zjtcskcx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwkpbshj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3enhbootx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dkjmyilf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iittmrzt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ypjynjgy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3izgduwnd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dfbxmhei.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3anyppkbz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cedhfpup.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3hldezsrj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jyryxxbk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3anfxmapo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3pqtzttcu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3thjyrgvk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3tpktebrp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3jlffdpkz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yeoilvqa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3tvbsdiwb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3htuyxogv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lewosgsa.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3edvvcvzy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3viktdxed.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcxzcfqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clmyxuwh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3psgwuffg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3neibyzwl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zeixchmz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ojpwhocg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3muvavjtc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bggyrqoy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3atqzmwih.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3cjzpijrk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3jlujpdxn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bbikwzud.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3sxfymaqg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3xcsmrdnu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lowvpwsb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3wnnqreep.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gapumeue.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3moztknvv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3waenovcu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3bceiitat.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3znmlnulx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cqvnrkkb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3gzkqhhrz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zgkeibzs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3jlxwkvyj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3eviorohp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nhutoqsz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kisaimoy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3huesfpvu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hdorvplb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3timokvql.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3dyaqdsor.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vzxxpbnd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zqxxgfhi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3otktotsf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xaxavzvv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3qnwvcpyc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3mxccxgff.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3pkcsvytn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3axdbixmw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hyhiupbp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rwslhdto.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vupgvxph.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tenimjih.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3rhgunfix.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3rgcngtwm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gcnigauh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kxxdssig.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gfutpgvd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pwbjamiz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wecbqegx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kyvwbeye.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qplnacsp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hzdrhfuh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ekxjasbr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lgexlrnk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kputiqqi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3szqufhqu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3omultcnf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3mmyizjpq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rrubncea.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rditincc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vdiofxah.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dzllaocm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3eeupuaoq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bxfvamri.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wuhldbpo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3gkzsuxcr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3indykbap.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ermebeux.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ulqicdvn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3pgqrcnfi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vwfpjuje.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vwtcicfe.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3cffeyorz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ddtdktyj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rnpwbwyd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wmhvlzbb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aduknvna.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3bijvaxnz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3vrxfpwpa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3vtfxnubk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hrwirefx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rwqgffkh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xnpjifls.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3eapbuikl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hdxemobm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xjobsftt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rrxrdxjy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zhjzfntv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3dipismtf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3yarnjlmn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3iblmhhpf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3oszpewag.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3xywziaak.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3trhyyvla.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rsjrhaot.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jyjmrdje.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xljpyrds.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3pllsqrlc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3bjjlobsr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3suxdlqwr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ruetqhex.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3abhythhy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ytwgfhdf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3whnxfdwe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3myyulhum.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3alondxde.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3iupvprkh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wbwbqiya.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vfrhznzr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3muulhdal.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3tzgczrnl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3buwajolv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sxjpewia.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mzligebn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aiuhbnuu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3euvcojvy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zajaoiux.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3lxldfqib.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3layjbyzz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3peeavkcs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3tjahpsfq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bxawiwxr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cilyxcyw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ieaodooa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qrwassoe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3txtywqoz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gprqjjpx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ggpodyit.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qavdyqcl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3avjqurhn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lamkfoyo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vobtxcsm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fqbhccqy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wlptctgs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3orzfbzxj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3pdcgplzl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ydxummvb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3grxzyfsh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zakxvunx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3neboatpp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3elojsbmz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mghrewzt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qqtajzqj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3elkxjvzw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zrgemmyf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3toconetj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3waadswyg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3plqjvuix.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jnfjkkgi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rvecfjjr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3eckccujl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fzecfgua.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3iehqejuy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vkbmmapl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wneatpyh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qsrwzsne.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3udlhcrgr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xraxhzoh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3gefhsbrb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3mwgeghno.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fpyikcci.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cbsgavvq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ukuzlzei.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hrzfyyrc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3hcawymml.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3jqyrgnqt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3uyonpfyx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3vvwcnzpn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xxqnxqlv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3lwqtvwtm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ycrqybee.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3jlwsgvmw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ruqpjnrd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3vxlyonpt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3uvmyqude.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3outbnopx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3eynlphcj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3iszgigjb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ymamoulo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3pokrebml.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3mvtasbbw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3awvavoap.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3khsmglpx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nswldweg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3zvxsosra.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3twwxazcj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tfpbuudc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vwaadrgm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nbghzqel.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kiazmdvl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fuyylfyi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3kmubohcp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mjmczdev.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qfxrgqrm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3oxnavwcg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3uvaswvcu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hfowqfqy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gugvwjoa.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3agtbkuby.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3owaecmmn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3pnmcosop.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3mkfjwzqi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bvekfzuj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xyuqwjim.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hhdpeihc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3rqizlmnw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pybyvrtv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3rekrwlbp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vxdkfvkr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wsmhnrbk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fpsghrbt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rwmqjykt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugmnromm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tmmcwxjt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3avqpbpyi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3boaipvan.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wyezulhd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3jqlrckhc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zewpyrtw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3kpnczmfc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3uejbigdn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ovgaplox.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3scgrjoma.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lrvguszv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3yfjndghk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3dgzbbgsw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pfjirjgt.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3usyzkofj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fzhuqmna.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zqfkiufl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3efkcjsqo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cpzuivmh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wdpergtn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mbcnqgmx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gvpzhsxy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ijwksfls.html


<!-- 参考信息 -->