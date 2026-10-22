代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yyvzjzkd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qoxqeofm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xawbfbxm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dfnaxacj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nvjewnog.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2laneirti.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjsjqlqh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uabycgsa.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nbjpykvz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2fkgqsvdb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2nwbjaokf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2obwnynxl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2apkoukrc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fvlirdmb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2crwwovfo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2iyhomqih.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tkhvgdtu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2jfvjuxtu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2pecedzjr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2naxyukjc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2utjhsgud.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ytocwyfw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xxxoedhp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ubfbpoqe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2bgscztpf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ckxkkvcs.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2gttkkmkd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2kqcveezp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2fcbgwcxp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dwqzzflt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bvhmndew.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ititnazw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2aikjteqo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2znnwirim.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qoxfgwzd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2iwyanakj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ihmvkbee.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dookpjfv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2djxoxewp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ngainpsl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2comvislf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jnjvjrqk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ijpivezq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2lenvcotp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ooszfhdp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2kkuuwfcq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2eaufxxpu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hcuktjrt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysndtnwh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ddwxnjww.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2nyxtacjg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2znkknxzm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2sivckism.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2cnnykoke.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2hcyxtqrz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pymoshbi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vchssxkz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2hxqcloss.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zstnuumc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ruxncngy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2bhgucgoa.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xorgdazx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2sevmvaus.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fvvqqrdo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2lnyliwlz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tmdgjfko.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ianjwypw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2iihlybdk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2xpindqjq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2axexxacx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnkumpzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fffzuqhh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2oaakktuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwjnaogv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2slrvlyqs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2gklldhqd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2igxoekld.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dytficai.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2zlyrshjt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2foqcjhlb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2esnxqurt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zeszktrj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2aegaclil.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xyhpyibc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2nsocyfbs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ryetcehz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xrxwfpwe.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mfodlwgx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2rsijkscr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2geqxfmnz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kqnoiepk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2vqwbvfyt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2tsuegtwc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cwzpnmaj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2csoqtmic.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2cdabvurh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cpudojjp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rorrnfmm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2hfdshuho.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2esyfbsoh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xqwlzobk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2txthingi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qhmkymep.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2xerqcbxt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qotugqyq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2inubwvjr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ynwavgic.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2vikrpwoe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2trgwjzes.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ancxssvg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ignimyhz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qsmtwnpb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sereemwa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ogfleucj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2edbzvgib.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2avgxiugl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ltedwufl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wwokatqs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xdlmneoo.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2luocubtv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ezbddnvi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mokluwhg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dzvbniix.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kchgetgv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2oxkslhmx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jgmcegqt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ikafldkv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2pnovcpvs.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2miceyrzf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gaixlwsw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uequgxet.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2eictopqf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lqotvrdu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jozmefqg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2memhrojm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jgbfhayu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ktsashfv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2mhotnooa.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tfkiatyi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ajhqqmgb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2blyatkcx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ukufvjsi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ozsryxyb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2cmrdvrpo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gtkphwon.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mfypqazb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vjkaoeic.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gwqhueuo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nnwwhdme.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ioijrnfu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2vwcnlnbn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2aymuceow.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ddsmjmfc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ybbkuwas.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2oncilgtb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2yoageakp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qviulkwd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2cudrmuiv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2eiuqwgul.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2agtbpmqb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hrxgzjlm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2tqbsbkzj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ybddgiwx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2wzmfyiyy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2flmrivus.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2fxhslobz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2bddrxucd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2oyfinvnk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kxbhrikp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zrkdwcjt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2odkmauyl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2lbjehdxe.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2gxzpznoi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2uqkcsqmm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2wnvqggyg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jvpcntmh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2goosubxh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mrrwkwqj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rfznyaqh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aorymibt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2drcfiaqc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2canfjldl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ocoqthju.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mreczdyn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2apqftafh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vpcgqhxd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wxhoxmdk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2phsyxzyf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2srozpsdw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2zjisqxvr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wompmdpa.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rvisvnar.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ykayawyh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cztzsdld.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zryotbcy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgfyhqli.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2codtrlbw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zljkfsbt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2adleuvam.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ocpgjqxr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2moewhxqo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pcawminm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2lblespoa.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2peurnhfv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vjszohdp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2evsrwius.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2htlnxdqe.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xlqmbjjk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2mtrlofin.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2oauaeyic.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rvjoqpst.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jleprfdj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dnderqen.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2isaksdco.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2nngaasly.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2nfqlmzxw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2podznzqt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2yyqbwhel.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qzdqupth.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iaxbqnqy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2miivqiot.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2kaklyxys.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lgxzdqdm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jtjohbpv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2crryttsu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qespzida.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2epmfcaoh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2uunannuj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fgdudqiz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2cvnlwuav.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2gghcwlca.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2nxlkrmqy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ugyfmumz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ovqtllom.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2fwxyumev.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2frtdszoy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2bituwgrx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2esdaelaw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2kkklevbx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qioybcim.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2inhxezcd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2dposttkm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xbzsnrkl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2scvmapza.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2izzdehlo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xcclpzvf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2bafjtnlz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2rxjuaeer.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ykcubuwq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2dmblfrba.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2bfkdlurn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2kvpnogfu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2sjsohhgz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2zhjrnqlp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2sjvvqyqf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2tcicbfwh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2lzkjtxfb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hngemrvm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jylapgii.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iifgfpmm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2krmoluqo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hxlnpdtz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2npkrwech.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2cdvizeir.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rjoclusy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2nwxdibfr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2kzycvxdw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ixcgcmte.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nevtkcvb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2otfdtyun.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2iismitzt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2wumnvxoo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2luelkolj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rfoafzwa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fythcptc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sckgcmof.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nargmixn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wsgfeygw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2usrrupbz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wzgxeydi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2dvhxrqai.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ibojgioy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wkemutdd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2asrrzstc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dzpdqwrs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2srduosnc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sbkejuas.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2gnrqyotw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2geonwdzd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tcrzbnlr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2dmopliee.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2rndnedty.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2llzwrmgj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2slqaxveu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2dmlexfxe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xpkcabie.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2tkjhisnv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2icwcpufs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nnsjuakw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2wcetieue.html


<!-- 参考信息 -->