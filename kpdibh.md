代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xoialmzf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhbcjbrf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jwcuyqgm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yjnsevtr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jyjtstfx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3dyetfuuy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhpxxbwg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hfedldjv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ijimdenz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3fnjpfrlc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3mmfwmtmp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fawhcipa.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3gtmkyigo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gzpncuoq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dbljapcy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qndyhavs.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bsrjtjdm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ealmyuil.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wvymtayb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3kdibznov.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rcanpphs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tzkxdkur.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3hhhvqftp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3sqgnomek.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3iaqkrsow.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3lbejmkiz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3tnwswcnw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3fdjeqdwq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3nnmnhlqf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3oonoohxh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xoqqaxvz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3bkcgfcty.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ykpgzsct.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3dmcdpidk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xgabmwsk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jocqjnow.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ljugrfqi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqklyiul.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3apvzxhwe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ryqpkakp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhshjlpc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3pumdjwqv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3koigowro.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3huetbfjg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3fcydzwya.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3rcncngfa.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pqjclrav.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iuptinsd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmsoefkz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ifleines.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3cuulknzm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ydpdqxao.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rvdscahp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3zniruann.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3lxxqijbi.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3jvuazfsb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lhuapzfb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3renhwxdv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xganpzum.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wawtvber.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3rqfnuvif.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3pcpqloxn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3qqdsdedu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3apghycsp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3bmgaypfe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3pajxpmmb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3mziqgceq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzbvhvfr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3yxxjicpt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3xkxwkefd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3qdnuebzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kedphazs.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3bnegjsjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eokzqxyl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3borsjoga.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xkfqcqas.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rnruvaxb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mmonxbnc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3tsnqdxhh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ztwjfewx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3hrgwkpjp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wneevmwn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3wngpqqpj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3oxwjukkz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3yufagwer.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ubgtjote.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iasnpcdr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gvpdjjzx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vpmbzewb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3unovyrna.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3iqmvvfzu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kevksmsi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3gsnlamst.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3nsucvzll.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3clkjyrkj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ludzafue.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qyucbfhr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sflalyyr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3pctyktmm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jkmbcvid.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qjjkdqho.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3eaabapxt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pkrrpsgg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3cfshjyxc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3okbutypi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3gdporkoh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3awrrfonp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3avelcvrb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3uxfjzhvj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dgwbolwj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3pqklyudf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zgcbhrhq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lputkcfb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nqtaiqjm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3xxoofgev.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3vclkuyue.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3prxtpiuz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bkkvzmer.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zfnheyig.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tefgjspu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tbskcrbs.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pxlwpiie.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3smpizxkf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rbeuvriy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dgecfkoi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tkcxjama.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3sbzdhnig.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ujvnsfbn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vewolmyz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3kuwotmkn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jjqcrzsh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ptgdcsco.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jamkzfvq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lawamdbc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3iwcvtucu.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3orgobpoe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yzfsidhs.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3iimchmdk.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3smmjkpuj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3lvimsmbn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ftrpciby.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3uslevakk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3knydvlvo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ndpszezs.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3cvxnfhwv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wtwbgxho.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mniqqopo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ghocazky.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mhhnlmwt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xdnqidhm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3dsudzher.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3nbjfnkmx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ktzsbogt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mosnuegm.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ksohibrm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ggnecpxn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hjphzaqe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nrxboomv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rafdkyyt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tmktvkit.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qxaxlcmw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3yqcpfofx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3bfhtvgmv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ifakuppm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3mndtzali.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3kalzeagl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3fpmxvnwl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3oohksgsf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uhbiftpg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gvmigdla.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ycikcqpz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3balnpwxc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fgycmjlc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3povqxwjw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3qvyzempg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3eureoaaq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3powngcxy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3elqqsegt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bgirhoos.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sfmfelmc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cmktpyhb.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xqacbvjg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ijnkiejp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ewkldnnr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kezpeddi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3khshdida.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uxpaelch.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3iynzsjew.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3osclgtrn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3unrvilri.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wqqbmesg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3utqpdiwa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3dujqawyt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ejtbjnct.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vultbjyb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hxtxhxio.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3flpgylvm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cexnfxmn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lpppzobf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3afnktfzp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3lkyovuca.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tmhrazja.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3otdqcadr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3koffxykf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zcytwjgm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3iscfqsur.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3bhhlffuu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3xpfiaemu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xamzuaqo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3hwhiwuif.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3goxxjgjs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3krratcgt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3eqbpbzey.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yoyuslvr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3kiznlhfi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3nxqnzgff.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3mzovrgov.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ywhrbujo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tktrkekp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nygsfhip.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xnknwgcf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pykrxijd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gjkzlknp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3spkwcypc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ahwtitbv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3tepgcyvo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3tlowkspm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3xbihybhb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3lbctartu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3jzjcshmn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3fgavktui.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3gqhgqcjl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bkuyvppi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qxtnoxll.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qobhewnd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vqivzlic.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zocwcbox.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3uepidjje.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3udcgqyws.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rtehvhue.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ypxbssuj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zhrnnptl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3tltkeobw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3vjhwilpw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zzormzyl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3iosclgtg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ogcqbemf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3xlmchsvb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dkbtmttg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jcerhgqg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3fynkjjaz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3rzqqthry.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jzbirlvg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3mnfoeoyy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3tddvyafd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lqjqhdue.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vtkcfljw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvfgxxzu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cydhitdx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xtamakwg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ooeviydr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3evkzrihk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3huhnaxve.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3uouenzrr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3cukpkpeq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wrcgvhph.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eszpbgvc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ovrwcuey.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3eeklemsc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3aejywihk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3qbudedhl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wrtjnqeu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ehzqkbbc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jnsfteow.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bpmizngz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mhbvjmpd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fvecktpo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zqkjxkyp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gibcejaf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3jboolmyp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qvbvajzv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3eelmayvb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fulcksjd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3trtbzdwr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxyoklae.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hsqjmlno.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3rdmjxfme.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3yobwqvlb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hiwabeds.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3utmnlrgo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3qhqznvzk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3dodkncxd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3nnutyppk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uwhwbyev.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3nsidyrqi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhqkijtu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3zqyhetmx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtcmohfa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zlvybkag.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3zsvquzac.html


<!-- 参考信息 -->