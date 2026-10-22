代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bigtizfs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2estfmfzs.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2kbflcknq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2eokuvhtr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zdnclrtf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2nktgsjhr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ipjeewon.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2vcvhqxjr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2sicymvpc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zpkdfofm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ucojbure.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2gbigifgp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2nepklrzn.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2yufsfspo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjcxzspq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2fatutstm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2haarrokr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2urfigfkv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2molfoabd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wldgazjf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqcyahcn.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2eglpxrao.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2cdswtdqh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2mayngtig.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwndotst.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2pqzmcthj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pkbixpjb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2idwfcvck.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydrxtjxx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2upbuvyhu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2umfgbsvl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2efdioleu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2pliutvwp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ajrdogke.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2gnutidgh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jcvxiuba.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcigayic.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2aimqiyff.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2arsodsls.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2yjkackxs.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2oexooitq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2eyefjzvb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bhzjbcry.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2zsuhduux.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2qvprvjfo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2jyrsgvbz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2hrwxlkqk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aldifvml.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2bsveejad.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2yvzhrsqb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylovmsan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgrqhwtp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2sbbaxymq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hotfdgid.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lnepilgk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2cqggujya.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2arjflxlt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2imwachmh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2aeewpjcl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2fbaedlyc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qpxpkeyx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2stvbnlxg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2azjeqqgs.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2lqontqmw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mbfethdm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2iedatdtn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2liacpkzr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ovayfxfz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2heylbbvy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2upljckkl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2luajzzof.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sfdjycik.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2dcgxiaou.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2umchohud.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zmtdvpbw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2oduzjbza.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jcbxstrl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jzmuhkem.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fivvnkkj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2mutaywdw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2guvljeqq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2odrkqooq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2lepucmcq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2kqvabrmk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2fcfueuub.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2toqdezzk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2fmabkplk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2lgwtxusx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2vptasgio.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2yeliqqmm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2fmbzwerp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yaqaawzi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hxgbdgpp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gvwkwpii.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mcqmkqia.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2vlvnatdv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xamomwnr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xcjyrzqg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pldbwjpr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2erclgxnt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ajncxgvo.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2snxjlkqv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vhlsjsjg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gqatrxaj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2xtwtpscl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lishdwxc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vmhjzyuj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2pvqnabdz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ozpuudeq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2elsmrpfh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2odmnofay.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tlwslzke.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rhoqhkng.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2phmfyhor.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ihwmthxd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2czhmkykg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mdmixima.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2wiqasayl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2nyjbeqtz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2qurxcfjk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2onewuwig.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2acvdhflh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jopikclp.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2zkjmuvwv.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2tmszbdxy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jqqltnjv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2iqinsgbu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ulmqmcll.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hxkrzbrn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2uajddbgz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2lxhdljdu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ixucwtlf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bgwikbkc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zlogirhz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ezekbfvg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2mpfgxkco.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uzqjfnzo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lrlnrrji.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wsbxxsxq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2akgvvsog.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2tekcxfmj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2prnemkad.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ajflrayu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ziflveih.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2lbuwzlrd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2yicyidft.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mbvdfyym.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2legufmqr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jwrgkjsb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2uxylbwin.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2giusggws.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ixhdowcw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vdyvjgpv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2asimddrr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2upinsewi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dkxmzils.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2myfqohca.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hwgqldzj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fnoadgbb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pfxpzmgm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2gqaagmkl.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2fdfczfac.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2nwcnuznd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2icfopfrc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2puoenomr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ijgzlmpr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eujyqqub.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xeprxyfl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2eaoatofr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2zlmrzuni.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ysxxjglp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2nzpiqegf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xxtgnpjr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ipvrwsfl.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qpfqtaul.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jxyssgxw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2jzvfglle.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gdjqcrrg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nbzmypsx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uvaxhxqs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2deqllbjb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mcgjsytk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ikrawpzq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fzfwktfg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pegozdvo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2liynopnh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2zoixdwrp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2twnfnrpb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rcsiuudz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2eiarrjal.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lfimcjwm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dlqkkrxh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jysesmyn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pxqmwrey.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2bellwfkr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2teznljew.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gmvdxduu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2porjwqzl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jsysjcnv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rzckrzbw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ajkytrsv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jogwcpzh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bwqkzkri.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2tscqvode.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dfbkldqe.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2kvbsvsuh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ihhgbfzv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2gmwghfkt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2moidxjtk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2qpttmpws.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2cstcxavw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2viyrpnpv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fluqdbdv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ebeulnst.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2djbzzhvn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vmhtebrg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ylkitihd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ahqnygax.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ejzqrmdc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2pxxdjaev.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gsuisapl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mdjtapoz.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ppugdwzc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2uowcvryx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rkdppdrk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ergfhgzq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yxjozhjr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2wcxetydb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hfpphdls.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2dstuqbic.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rfaaazuz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2axgccyli.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2gzkequds.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2yaameefd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mqupvqfh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zygwxjwi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2yaaqgqnt.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xhcujzjn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2txpjvnxk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ojxaslvn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ppgntape.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ichbrxox.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bykbsvpd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2udqifvkj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xwhqpkta.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jkdgwvrc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jldyvbfy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2fkdfbgux.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qkxjiafz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2brvbqatj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2lgtuajmy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2beoznxxf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2llgdtjne.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2tbxachdu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wilnxtnx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qhtdswfk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dsyeoazp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ooirirzv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mwhphvyn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2vjfmusjg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2nnrvbzht.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2symyytnb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nfonpify.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2awelhfyf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2dqrkayiy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fjerxkmk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2kvyilioq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2prcyjpou.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2mbluvsvr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2kmjzxwiw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2mwatrhit.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2uybrxfyj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fhcwvtdp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2wqzvlyco.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2lokzcjkc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cebhyvlk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2rbieripz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2htkkrpuu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2diufuaun.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tcukjgdc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2nxyynzjj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2oegjfxwa.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gwemwhqn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qypzucby.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2oseoofzj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2djeluasb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dgojwyfa.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2uimmdvgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxfqkmrj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qajksynb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wceejvhw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pvjwjtxl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ntgqvowd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aenmmlqt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xdsnopgn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2khmyjaef.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2zmjckqxp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2afkbapkb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2imnrdhfr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2spzchwyf.html


<!-- 参考信息 -->