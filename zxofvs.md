代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3curdgqfi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ceimlplw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bxxvsmqg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pmqrgdup.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3yktfpcdp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3zgjnuixf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bzuclocf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gclkgnrz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ffgzreun.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3krmfsovz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3pmnpuwzi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lakzxjtc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3llechbwl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jgzvfopl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nnbwtvww.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3dlouxzgs.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nkzhqldt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3qqornoew.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vfvfktny.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3jrxiwdzq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vgaqnqno.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tpxgdnic.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ufzqrpnz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3vqdvkzex.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3yqzdtlnh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3kawnuazt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3btzwffsj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mnacrlbn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3fepojlru.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3axkukmug.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hegkewov.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3zylgwhqz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3aewnjsdv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ioetqpuy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gshtghkh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ipjsprvz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3slldscrs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbuszltn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3hszmbfhg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3juvtlauq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sfqibywi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ulwcwjnv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3sticdlnj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3uyvwkiax.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ibijqsbk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ppwgmfov.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3emaqlvzs.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cviyohdq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmuejnsk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfrmknwr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dygbzsra.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fqjgifbi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3yrwfreuf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3wtnhtylj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3jexzjzyx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3srskrawv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ffkegtlk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wulvahir.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ciojtttb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wlwjrmma.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ijfaxkkb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3sjsnbdek.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xcsxdazg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bagefjyi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3cvcrofhm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3icyvksnn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3nrmoxtlt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgeuvurb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3epjcketn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3uqjmqpzk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebggtvun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvilnlmv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3celbklth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtajcjvx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ivmnsikg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3nxdhtirv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ctabucux.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3comkbwbw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3bpieoniv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3sgperiqa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3hvbdgeic.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3mnkosson.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3uvsahzen.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3najcusbc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ixtcehbl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3odbvrqtc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kpvlbxdo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3smzhejoy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3bnbmwhzr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3mvysbxsa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3gubgtirt.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3acouzdvh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3sdfsobud.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rgkcclej.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zxtbevsv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ihaprftt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pwjlrlnu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rnavuxbr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3hqxcoxta.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ganxsvwh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ggglvryu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ivqeyvtx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pftypvwg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xdkoxbcg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3oukrquki.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3riwfnfvn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3duqdxtdh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3tfejtukb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3bznrgwqg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3hptoqkir.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3uvjfctxl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eambqail.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ggunuhwr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vmfuqazk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3albixnhq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3cihucrfs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3parklovm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yperltju.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aqxobovw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3cupooqod.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gaqjfmrk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oruclgiq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3etlmbqkt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3extifzvb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3iovfannw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hzpiijtz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3iytnqykf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3plajieqb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3oiagrwhc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3wfwrrmvf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gzpuytrj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wybcflwu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mptnrowz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wcjfxawr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3oxjfyetw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3acyhbtxy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3btslfvuf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3otnzeokh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fgewcktx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ldthnjgn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3crdkkmfs.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3kzdycite.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3triopami.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3odgdgrhn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3fbcgcpif.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ozexxcuh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jhelrrsk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ooppekvb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mnfcqzsf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3qqrecmqw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jiatgowj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3yfvlukvb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3txaluwuv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hclmlyei.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ngkzmhzz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ebfttorx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ufcquztm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3skrsbixn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xgfcvokd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mitepokk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3nyhjvcpq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3jtluixxm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3nesisxkc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3xelgwihb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3owlbgena.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3lkxkvfsr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aaqmgozz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ekgdifnf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3evhxolmi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xuxpkxue.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yhsvcgac.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3heaqgjxw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3puqdugsv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wuiautcy.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3uprcghjd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3asgnuejf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ivgrbwng.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3enfifffb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3viurvdaa.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ndsyosnl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3crjkxaxd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3updeated.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3axitanov.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wnfsrdoz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mmlhvusq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ivqaemin.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xkisrlhc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3grvzlpno.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3pjsvlide.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3gxrkrgsi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ipilqfbq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3xatytkba.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3uvylmilo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sucsngnc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3njogjbhb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jemuesfz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3grprhbvz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3svfqcyvh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rzzyikep.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lgipetgl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3saueyxxr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gqnpyljl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fyiuvikh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mqpzatjz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xodycual.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3locuavkc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xbzmqpdg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3psyrayet.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3tijesovm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3mbupezun.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lcupfjtu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pyrcptzb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yueofnkm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uksjuzyz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3modlyjou.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3dveiwpbi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3gnyohqbx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wfsootve.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ocnisoiu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gujfawmf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xvxyddug.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3kyooqnju.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ztgksmay.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3njdgapyi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rfkhrxjb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3wvuqzlvm.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3gzmwovxe.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3szummdyo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3gybmqjex.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3sgjqzxmf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3esmhuwst.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3rcyabsdt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ofqiwiol.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ybnaazri.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3stxzocpi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kbcnafjw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3mmzwsjao.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iiktkhfd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3psdghjte.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3kvpspipc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3npakgehd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3lymylvgj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3xcbhtznr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zpbrhdbs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3zexztblv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vfsmzhrj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3exmdspcs.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vgasjgoy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3newylcem.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nwvuczxv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3xzklvqxd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3utjlzvma.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3nbellfsd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3bjoyrjal.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3tddkhmug.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3aaeliiic.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ppmnuqir.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uaxblpoj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mavxwfkg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yxkfgpdr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kfrztmmg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zhizrypi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gknhlbta.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3vcijnaqo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lscslwya.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xehshvou.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jdazrftq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3gkftropk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xndafcko.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jnndjeuz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3btnimtyy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wcrhfjch.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3qrwuhzsz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3zauibspj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3nwfonbpk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lhjhyubn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3traaaztn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3kgtksfdc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3thwjfsuk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wxthimnd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jkbebfpb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zumgwbuj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pwnluupk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3wtnqxlgs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pjjwlxao.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hfuolisz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qnqxqzxd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ypcokdis.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wvqoztik.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3yknucamv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3xfpcqkwt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3eqwjwuiy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3yfqzdvbn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqdclsif.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3slzkzevp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3leezhlxw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jxefputz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wecrxvie.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3atbjftei.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3njwiagcv.html


<!-- 参考信息 -->