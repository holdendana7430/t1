代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgfiutdh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2piieoszt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ggsqrjms.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hqngjeel.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2zazvbkpg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2nxxoufho.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2spbctbab.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zlgyopdh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wgcjzbgg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nwlnuciz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nlddrisf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ywxlpbzq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tjlvyhrf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2eaigycxj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ebttkhgk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2fkrubisy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gcufrasq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ljmqwskr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2veutmsny.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pjpzctte.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2evfgxgpr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jdyxyebi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ucxeytee.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ekkvvrdb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2iinynvvg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2negssxcc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jqxnkvif.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2pzwzmqzh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ycelbxxe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2dagicylk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2eyzxusit.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2afqbdihf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2nourzzsy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjpigcmw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2cefjtiay.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ozahqbro.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcquqtep.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nmovrepc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2jnfavfug.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2vbkjcgcr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2fnzeapfw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hxulcduy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jhphhmpt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wdsldksl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2afigbnvv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzpawnpj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2pwgrvmsr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2oeeklswz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wsvxbymv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2pncfgsjc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2tnbcqhiq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dbcjzjrt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2eengwuvb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2dwktqjql.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mxniybxq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2yuesgydf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2snievqmi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jbrmouoo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ewllvbug.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2oqwtfdyc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2oxredget.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2uxwperkf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2gofntxrs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2arkfombo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2lkyznilz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xegevwgo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2qbndfmod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcmuslda.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2mnqwdnft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awqgwigt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gnutesgv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2nqtdcqdb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ntqclrft.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kztwvxch.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ckeoslwn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2edvavpgh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2dqkfplrp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2btvberbv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2oqnwuere.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wfrscdeg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2nvnetemk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2awbongir.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rpiihmnn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nenfwalt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gqpcxkjb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2dqlnxcrk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2pnbmpbbc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ezyzjale.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2dvccuqdu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dzgqmpzn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ahicfwzi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2teolpgfc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bcjufvnp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eukmrthc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2agojretn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xvnkgoaj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rsbtdaqu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2srnzjwpf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oxgbnedv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ssjdvuqz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2debhcryk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sppvshvu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ngbosszs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hozdrejy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kdsigqvz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2psesjfrm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2buuesrtj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lmwctfcx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nwldpmww.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hehzkwwm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zqicicsg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2iarcxtxa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pjunbyww.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xhqwbkts.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ueazbihd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dxyxjxbk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rssfedlw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jwxbaqcp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ltwauach.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wexjcopm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2iujbbvmu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nuixqyqy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qbbqubkm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wwyqgali.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2olaiyoeq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xklrbnvr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zhtbqhpv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ghthcyvm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ltyftgfd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rrlkxhlq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qgdmnlud.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2xwtpbpsx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hubdwmdr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2rnvokfwr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2trrswngb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2mqxcnchu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2gzkftjaj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2mqfoiage.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jexzhmem.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ygtccaes.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2gzgrwliw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vvamughf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2xivnpknx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zwbamuli.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2oqrackhv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wedrphzr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2vflohzmx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2moexdsvn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tymqlbkq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gmiglvsg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2pqlmpmya.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2pcuahycv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lxufknbs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ptamvbqr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rimcorbd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yepwbfnx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jnhumjqu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2inobhdlw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ciuvwjgx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ytseafuq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2alpxljjr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2nlujgbpa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2krahusru.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2aowpctqf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tvlpyapq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2azabjpkq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2itobebqk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2swhsnjlp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2egukbrvj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2aagbxjyn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2crhvumeq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2soppvqad.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2owgobemj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gyttvqba.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2rpbzuwer.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hygzzgid.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2dehjmtue.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2bcwpphhj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ldsqiuad.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2aixqraey.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2stylspwu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2aotauqsx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ehftdocw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2tmozewef.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jldahgkw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bgfyiqio.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lejlvmmc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2vxteamrv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sdfyrylf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uzjfeblz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cotubdze.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dsyjiqrf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qhtjpqlz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eswrvehp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gnzsuglw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2odardssd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2gcthmfpp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wlcxucje.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2offdimsa.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fgmfkasg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nrdivvnm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2xrwjqsam.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2rvohjgvh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2kpnixnbl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cccfvsnk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bkfzudww.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ntrottim.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ntonsegp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ztapqhxz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ghquxiks.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2pgrcwgcf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2dvumrzpd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2harrhpxd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2mjvhziaq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2oxdykylz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mrcbhkyv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2zyfvrvwb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iwismdyi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2coqvclcu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2zmhskosf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nbfhihqt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2lhaavrvb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2cexjrjlx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2bsyltfzx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2qtdlvyzi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ltomvwsc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2nidzfaqe.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vjwukrfd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2njnkkiqn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ohsawzkb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tfwtncrv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vlgbtocm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yjrexazk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2etgnfezg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wkhsivsk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qsnmocwg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zjkraknr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2kciyeita.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2kqwtbkwj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2lufuqqpk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2npdtezir.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2djzyjjlt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wqmywhap.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tgsslmtw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2teymvqgp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ckyysgsp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2bvlmravx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dhzwkapp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2aabywfub.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2klqcnplm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gjavkmyi.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2qxygrmge.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pwhmpvtt.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dyjmleun.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zvvwpfct.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hcvyfpsf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dvgvoqta.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tprxbbxc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvkcfigv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jocrkkiq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2iteqswqe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2kteltxct.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ixqvnhnm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2wgxnguif.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2pggorhkj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mwsyxelp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hxwcbhgd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xdpdjkff.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2retfjzae.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2frdgqdzy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2spfmfinv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cticqefc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yndwuspn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vagxzsjt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bdhoqyth.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2mmswidnk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gdaywgfc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2basvudnj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2vnebtpph.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2tloyopmj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aazygvto.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xdnvvwep.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2fulydhbj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xzaphpzd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hgjbmylb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2xueplntk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2zzbzlagw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2fjzawfnv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ncwhewhr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2hijpujmn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2draqtroi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uflmnzct.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qcboyisn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xurdbhzr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2togmeywb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mkesklbq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oqfkqnzc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eckwubzo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mrpdhnwr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2grkzmwvy.html


<!-- 参考信息 -->