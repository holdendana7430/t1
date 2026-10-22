代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ruooppqh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tmpsfqeo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2izqppdij.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2afmeheew.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wambxcqt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2gsiwsqgp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zkkzcykh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fhljwfjc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2szddtuqa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xjnudcbf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2avhroavb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fymfnpkw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tiptktjo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tmnohacm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bztbpytb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2miajgcdd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zbxwvshm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xttvkgfl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2oflsqhgh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2izsmtkei.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vqswgexf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2bdzrncct.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2pdiwlsoi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2woulgiog.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2fmbymezc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2namirtqb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2myefjscz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2odwlbmgn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mjoacehc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qdspogzq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qadshrxw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qaraoepl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2trutfksr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2dabmketq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzcpxshq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ilwzhpgs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kqhrstxy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihoffhnn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wldefyqx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jspikbgq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2balgghtr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jweyysmn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2hmtfubzs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2sczezuil.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2vcbelmox.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ugkmxmnf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xmvzppin.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jmztpwbr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vttztkgo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvuoalav.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2tkodzida.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2eemzsyir.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xazlnomx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2sxyrdrsz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xuwhnoae.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bpfnggoh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqjlhxgz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmshiebq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2edokriqz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2evscubnp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2koeahkah.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2naouflhy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2kljbhyof.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fyqwifxn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ecwfmsor.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2uqrdsvuw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ocxeimnm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ogxgucyf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rgadbsxp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2xuugwtoo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2aqdpwvrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmjmhjwg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2lssztlti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msmuqrlo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vbwpkcuo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ljalvheb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tnfkwcrv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ttowacvo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2qhpinfcm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2yekenhfj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2grlbufpl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cgdmevqw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2nzyyehcl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2lfgkjcbn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2auctxojd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2qtnoizal.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pglnorkw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2sdudwdwf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2veigewph.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uhwxqjpd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kvdfeajc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2pdphkota.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2tjhlyuie.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oaoslptz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2vhygdgtf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2tnmgectn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nlcjkesd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pueuxqsj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wxmgnqhp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2pcghgvaw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iuxsbqqc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2hbielcoe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gqzqhxhg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2bpkypbgg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2bszawqso.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sjrjlwzy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2htksikoi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ifnfwxub.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qswdmefs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ypmsplch.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2jwzwgvyp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cszngycr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bglsapql.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gnoctbrl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2opzlkekz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2yinejmjz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2khbcrnuu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gmciczjb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kawyhfju.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2lrsgcrmx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wcztqrjx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lvoxwuvq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zynpxpah.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ctuwregf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2fyxposzk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2viltjuiw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2spaaknao.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2sufyppno.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2uzbwocoh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xvdsqyct.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jtgsrbas.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mhhfacom.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ahkooxlx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oeylvmyq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fwqwvvog.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ccehjaxw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2liaagzui.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2zsndnivm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bjhiabtn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2uladurou.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2sgmvebpx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2eazqozoh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2nnuirwli.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2keyqagmy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2mpycfeza.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jmvkqvam.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mkcoqdlc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zlygydxa.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ragzyceu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2pvvhcyzs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xbihrffb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2liahgjcn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ctmuvxlk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2isscoqwc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2pxenbyii.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2adhafdxy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2prthiedv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fkwynqas.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lvqzaisu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dwuetkha.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xulllitw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2xmbikpwf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2dbsnmypa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ivrfdcej.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2encasdmn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xmbrspdb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wdblmlyt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2bihitylf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fddwsrjm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2aondnhkj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cnfrnknl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2nluxcbaf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2yuphrkaf.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2kztkscsp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ovxexmea.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jbpdqcjy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mzbbrjyo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2aqufvwmk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2jvyaopxy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kgjtkvno.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2xvusuadg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ybgopcco.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2qnuywonl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ejjwblme.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2reovzlnw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qiasujzh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2uwcnuvoy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cxynvjxb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2zvpkfivj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2uzuwruju.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kspdvwxr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2fwpxxzrk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2yxuocdkn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gjszuwri.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xuyarmhs.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zemclhib.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2subopwym.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mgbdxlmo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kbmjqvne.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kzmefuqj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2bhofpjcz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kmszkmcu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gtgalmak.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wqjtdtwv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2msleismx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2nmqlzbiy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2jqrkpvgj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2sspwnofd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fbckdxpb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2atedtvsb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sxervppa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cczclpvo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2diwuzjva.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zalmllpn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2tkgfcjwq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ynzdstds.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rgfxvygp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2qqaaabtw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qpwsntay.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2edshpvea.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2okyulxht.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tttxdmsj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2kqmhetsq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lferjkvj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dmpnztbb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ykuuidli.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2dpcmvypi.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2pajmciad.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2abjphwsy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2kczhonec.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2xvfukxjc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2qmuiuhqw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mciuyqur.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2diqaejsi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2jupkjdhp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2demdknna.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2vwngkjar.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2wzzfxdin.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2gwioldkv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ckuzntri.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2otufbyrd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ukkwelwj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2yyqsrvxs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2anufxvkt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jixlqrxl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ywyoxzyn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2teoygyzf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hjioruii.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dlvgkxgt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2viaviydt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2cjhuywlb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2abupwzpd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2lbfrfrpr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2dfzxpyku.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2dhcqjdxc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lxesogcn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nnvplsoh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2htvnflvv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lzlzuykd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pcrajbtw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nmdmkqxh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yibdvrkp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2idocqobk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wgpwxvme.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yrssgpyt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ejkzuzqq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hwuubcit.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ytqcmmea.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nixkjrah.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qomlzwww.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ggmahdwy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2mpyheyed.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ynvrrxtu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iqlyolww.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pauwqthc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2squghquq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2foyeuveg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2vxgapkjl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xroiqwdk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2sblxcmlb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ystjgipk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2hxbnaxwz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2oupgihke.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qnwggzql.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2czkhxfey.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nfwknmfm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2huatreem.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ndbejfur.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2toveocny.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2pisromxo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2snksoqzy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2scjbiyod.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pvfgwbqx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2idvvbnfn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2uyitqcgt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kybzxego.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ryxikfji.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kjfqorls.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2oyurgtcl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2isejpikg.html


<!-- 参考信息 -->