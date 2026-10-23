代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3hczrgohb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3oyzwopei.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ckbtxvqg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3fqdtwnew.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ikodsmfs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3yknzcucl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gnrmskti.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ibigdekp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3nqbndxtq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xokptgxa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3juornmzu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3jgqexsqw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3bpnhvuvc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3pzkhpplp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bbcvphbl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3gtvachwu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ouoyoshx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3unmezmvt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pdrmiwco.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kmsygtbj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uozuikco.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3bldczuud.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mmpbwxfg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3mqagqzyg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zqgxxfex.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3hwjehabh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3vaqgcsey.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3svrbhaxh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3slamjalg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fxeyxdlq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ysxxeseq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3utqgvwwi.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fnpxnfes.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3rhfybqzs.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3arxpilrs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ocwcojvs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pgxctmfg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3eapevdzp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3daetzpjj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3izwhjmur.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3sfonwlmw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3hvbynccl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3swyxywwh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3idoakwcw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3pdmvkffw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3cuolokxx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xlmxxmuo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3idhveldq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ckudwqpo.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3belndfhc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3uciloutm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3djekwbde.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gjbhpgvi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gyinrngo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dkevctac.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3orxdhdjq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vnrwkpqt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3xbigigaj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wkiuucko.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3rxqqnmzu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3tlptggja.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3sdodmcnr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ryilmfap.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cmmiiiau.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mafvllhp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3avxjclyv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ismkaump.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3shajmsrt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rvosnvxr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3gpnlfpvk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3iwnmrnjy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3oibokfem.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdccumzz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3udgqxdam.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xxcrhfck.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wanxcotr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3fsxxfbpc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3khdcafms.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3fdinfwoe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3dbzhbvbs.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ltveukzh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ejnnxzfb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3axdveoma.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jpyhpeco.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xfjekrlo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3bnfvuohj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ovpuwahp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3soursniw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3gxaevogd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emrfitwl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qresebvi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3cxtgfyja.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fdnjrbhp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zlzpdzgv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ptlepbdt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3sbyfipdw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3xlmzedsq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3lmodblfl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3mkexwqsh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3smwfabip.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3rogkqdyg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3yfmwavcv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wolpbeuk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zplarpfu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rrfhtijv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qqkmultn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ldmcxwcf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yqveakji.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3djcnfoyg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3dexzoimv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3igyamsvt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zvwlncif.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zhxytpkh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ofohjlxp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3pvaqagle.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qkbekyhr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cgoftprj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3uhknwztq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zlstpglz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3spmzleey.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3nolpkhuk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mrtzbahc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fdirvjmr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ztppkvqu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nkewsxpr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3lykmeibd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3iiprubfi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3biexqjls.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kukbfykf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lmqstgdn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vqcecrxy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3wxnbmviy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xmncmlay.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vyfgmhkd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3srwfyudg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3llspvyqs.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xhodcjsr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ecneazee.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ddjcyeqg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ovuppvnz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3milyobnh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tstaxsvl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3cmwdottk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3zndxweqo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ffxqzgbj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3wcbwaifc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hyflgchq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3khirnrfz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wlamnsxw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tblkbxjd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3nkvtqpod.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3kzbqezkd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3emytjmep.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3decmwrdi.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3jspnxyqs.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3igmcsqtx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3adylwslx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3dqlrmftj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ewhutkcx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3bogrzjfv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qbzxhrxf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dwztolja.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ckosnmxi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ahabgcpf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vguvckhb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3dujqyckk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xjjnpqvc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3wqixiedz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3urhapyea.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3etyrwysf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3kujknibu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3hlvyzlnb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3akxmloyf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eytzufrp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pngingse.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cqbltukv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3chsonhie.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ivwawngw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3kimbhjpq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ikddakja.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3janelils.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3drykiisw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uxvmficu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3fxbvktfr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3atlgwmka.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3prbkosni.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vdzutqrl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3iiblfzib.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rtlfcuzz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3laqcorig.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wvgzwtkb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3usrujqaw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fqptfvjb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rxabktou.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3fzyjipif.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hfezhrlq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3tyrhxvlf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3iwriuivl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3pvfacumm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mlazjcoy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hnbbdbcb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3caxbkwhb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xenrazdy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3qcldecpn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3swluuozm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xjbxibsc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qjocvozv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3tvdhnzls.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ugsthltb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wvnfsxyz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kmsvrrua.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvyfkcsv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3xdxltrvj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3satmvugw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sgspizbv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fnkqbpze.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ewxllmur.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3beydpqwn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rkbefwqo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3iiefiljd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bpirpvgo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vmqjmpkx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3pdrszezk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3nqwyotdj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ktclzfgs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3vzktzcua.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3smddtomi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yldkefmt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ycqfqwpu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wyatiwax.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3znjxklwn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3qkjdzkxv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3eqsrzsmg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qyugemia.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ebxbdycb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3segpmkft.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3pmykvtom.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ynsklqek.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hwkgckqk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pmxyfhuo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cakdemrl.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3gausybrx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3njwstrwb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3mqnkzyyn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qugadjwq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3yoebtlgk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3pncfthur.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3dweukjaw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ecbvmdaq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ednqacqs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3spmssgaq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3urtbfosu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3uwtaurbr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3blodcery.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3glznrlgq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bkodhxyq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3luywtefo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ryhrnlrh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3tdbqedja.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3glbqmrva.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3lrvzykdy.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qpegkcmi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3opkzjyct.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3emagotsg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cctwdjqn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fruoehxv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3daezmett.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3pdewridg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tyuhyssk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ysuluvco.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wsheqcoe.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vyqfvsze.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3qydhfqxj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hvvfgdqy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ozmyebwm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rrhedhkz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hlmeaaoq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3twxtxtmv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3reckwmlt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3smmpyapu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sefambjb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3hrrgdqdq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zspcjjso.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3kvhlbrtv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hcpepklo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3nwxxsnco.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3oqguieya.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3euvjfbzz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3kjtpithh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lmydnnmw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3rkkoraac.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gnsvapvp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ymjywmaf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3qrxdewbs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gghudjgl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3pdkpdnlh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3njbrgdxh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3lowgrqnk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3kzuijzif.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cvapqwgk.html


<!-- 参考信息 -->