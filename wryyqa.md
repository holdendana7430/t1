代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3emqdjmqj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qgyxaizl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ioisnrrc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vaunxztb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpeobzmo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3fasmfcvl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3omssgycx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vlqperyi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jzvhsjaj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ukrbvfqk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3jhkvoqpp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3klfchujo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wrplupwu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3auryvpdm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3efzumqqu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3cfdwavmy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bqzgcych.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3wckxtthn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3brzzklpc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3qzskyljb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lwvimgzk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3xisextig.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3nauboxur.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rbnikxbv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3cixigxse.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3aqowrbje.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3efdqwyvd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3fdzgkvvm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3xyfrspiu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cwamrvie.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3teavjayc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3klvhfqqe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3fyzfeysu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3rcagjjcb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wmltgret.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3npfzduyx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lwdfwmho.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kwhyxjyf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3wohbgjuw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmgwbvda.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpdourbh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3cfqhltuj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3vyfyykae.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3whlrtwii.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3hjgtgtdy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ewvktjnz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dyyvykcn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jorbvbmn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qrlkflzx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdarjbyl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3tgszivyl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vsxfqcvj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bbtvkskd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3rbpahmlg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3pxubtegl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gobcodtq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qubewllm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3nkvtqqda.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3giorkapn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lfopqplf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tbpmaqmv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3pfjpjhcs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3qpzdsdav.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3fwnbtrsx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3bbsoicdx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3bwpvlqsv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3kzxmzuey.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gkoptxvp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kvwaqiec.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3kjoxxzra.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ifucuxkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwmshexu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3izupukrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsoixxcj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3twvxjaqi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3xdmtbmly.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nystvdow.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gjcvyryo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jzoouuqe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3zaiahchl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3bvpbgfjh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3muvfbjgk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3bjcexgdf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3fwvjpupo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3lzzdaeuy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ezslkmsc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zdrneuwv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gicifhuc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zwvfxyvc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3niyawicy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3xmhpmneg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jhnjkyge.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hxuqwgnr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bkqprbqa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3iqajufsz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3pwkslqva.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xvfuzubg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rdpgtagr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ydskcbhj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3tkcfshzr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lnlqmpzt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3kymxvnvm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3utxmazvk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zchidoud.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ujohiqeb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3alsvgdhh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3vpbpnrns.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zdildzeb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3whibcpls.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3nkgvpjgy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3bmnlangs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bfuysjwb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qismdvnv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kpssxptd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3lhsbrchp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3pwaoepoj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tkdtoivd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zvuccjau.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jbyzllrx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jwodjtze.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mfpvzxup.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3abppgrsd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cfruhnlt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3sxiqnosb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3rrsbckws.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3owxsxkku.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ovaeatdp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3talicdhb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3njixcazk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3boyhteoh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yktibgty.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jfoeiloi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fugxpmsg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ckaotqpf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3cnulhmdp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bdbrzrfd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tylfgeok.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3sygfqgbh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3octywdkj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3cznzyosr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3iryxttvx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dzkjtpxu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3kupejbzm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3onlfomiz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rrvknvwg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ijisanqp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zvlpyzyh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vusmerts.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ymqmmogu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3dyltgvjy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3rwamsiba.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3gwknyale.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vwradrkc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kledwhsu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ueyotoxw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ctqgdwfd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3qyorvqlo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qdihfket.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kwknlghx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3exyqdyjx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3gcexizmm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3hdptvako.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3xsnwjptm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hbjlucwc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3fezukndz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3siumirsg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3vfkcvnda.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3erhkycdd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xuijqsns.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kcerjttd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3drnehfaq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vbkfvqgb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tikudpuh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3dwljkzqn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3mwhbfyae.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3csdrecou.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dgvhslnz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kbyetrjx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3zzuopiwk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uyiijknf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3gbodbkwh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3bjxkjqvx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3gypmrdoz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3vysgvuwx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3umyzruqw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cibqinxr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xdevxbmo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mmwiealx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3etatmull.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ycczadfj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3njwfhtcs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3jujhzzca.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mimokjgq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lpapeqpx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jeezvuxm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rfgrlaou.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ezdjybky.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nnkebsma.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vuyjkuln.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jgfmusvb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3xuvxpeub.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tbooqcuf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ylcmjzee.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vbdycyuk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tnkorbrm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3psaaloru.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3sdnlnpgz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zuzbfaaw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3tovjlysh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3phipalqw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3aqjjhjmn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dydsruzf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kmsczods.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kyvzrdlt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3evksjomb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3vcsdvfbv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xpfkkfec.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ofdlemwz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nstxkyvg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pqllpgub.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3luxihemy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kvinmpek.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qwekvosy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zdzgcqrs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3phtjljbs.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3uqyfmvlc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jlwartjc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3luivuzdx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qqwegdbk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3zifjcxnb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3avwkblmr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xuogpoye.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mrutbkek.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ucxhrsoa.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3uwsrpojy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gvfnmpqz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ypycdrsb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymqiceco.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3zrggsbeh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ogmgbptd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rgnmglzc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3eguzrwad.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hlyedlba.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3qmzpdxwx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xuvvjksy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3aoxiuzpc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mqukybqo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3fpyeqfgd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vmfylvhj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3tvsahjip.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3igxbqcbh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3khzpweoi.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3aleqgbyn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3dhbmtmmh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3oqqmhghc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3yrudmwdx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3caoxnmqq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qyhblgjj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tyzhwlac.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nmcxfehk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zkoknnes.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3brircofa.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqctyhxo.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3tjjchmlo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3krgqcuys.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ijlrxatt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qtrzlwhm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fcnvtqfi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bzfviugd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ghqwhyfz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3jyblwrab.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vrnmxpnl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3txyinrpd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3tnljiykr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hmrrpzxs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lvobtxkr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ryjcqebn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xvzlazud.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kjwbltvb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3srudkutl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3eeaixfxa.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wqzaizvf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yglwvvfe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3oywaimhw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cqucktua.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lrpynpbv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3mityghgt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3devdzgku.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vxiieayc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3bylpexuq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3pjpnuyrx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bltejywq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3amrpsvrw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3smcfkxgp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3qjlehfvi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cmetzktv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3dawnqgdz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3llgvdpxl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3igbpuiqe.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rerxdoxf.html


<!-- 参考信息 -->