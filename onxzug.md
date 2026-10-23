代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pjlcciup.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dzpdqdvf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3duwxqrfm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3osvqwlby.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpboboka.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3igtyobns.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3afsvzpxo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3akuxwkmu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3uoflxdfk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3tmtagssu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3nkucghmr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3wywihlap.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fydtetjz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uxxbcveh.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fvkamcnm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ejelcyys.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mbxnyhmb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3udynkpjn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3opjazuai.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3qztrpamq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wkdxibqc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3boeeedpi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zchjcmua.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3zanyxndk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3cmjgsvuc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3hmsrmavz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3eddgizin.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3grksyljy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3sronwoic.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3rsjigwft.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ccotmslr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3dgdglfco.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3bnffebvc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3fgawoiku.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uiydfaoo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ozbgtawp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gumsrsio.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vshbqxko.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3qwkuqncw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnxstiei.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbfxphow.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3mglheplu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3qvsuflof.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3dufoeicj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3gaacppin.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3irofufwu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hnlvbmjn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fqlbstgk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wafvmgak.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3fggodkjb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3fvirjzzt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ydekymum.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3jfuxqrde.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3qpoeqkwz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rousclbx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zjemtsdf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rrfsnltv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tctneepb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3phnyvrys.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fqrlkbve.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zccgasnb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ltwkildt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3pkxfkenu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lszvmkqh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3aedsznow.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3peptczmx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gbnwicsc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jztkvqsk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3behpdxje.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pkknkzdz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqthrncm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uoplsbwu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3tiduwtnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkmlyixp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xgtrfxen.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3dwxgutml.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hdthdgwj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wemulsvm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3qnnromiy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ijweufrx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3qebcwpuv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3domehovf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3asxjmhtx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3knlgeykm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3bkijwffd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kmgtwuca.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3caoiajbl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sphjiqub.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ewqhwdlg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pyfoctcg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3rbjtsonf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qtjflbsp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hvzizrbk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wlejhgkp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3vxqlwhew.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wswpdrdu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zwdxzlmf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lzlglzwd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cgwyopzu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3jbniylgs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3awgoazva.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3chfpizih.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ruxaaqod.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3abesdggf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3txushodi.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3seuqmbot.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dtwbodtp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zjbngunn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3fohgviju.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3cffqpqeg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3cpvuowqp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ojoqzztl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zfiupopu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3noykkpnb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3kydrbceb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3fxsrgbgo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gjzzzjgf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3oznrylqu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dyrszsso.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3akoekkwj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bgolrizj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zuyswkeg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3yazmeyat.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hgxjwcay.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3gnecyeee.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uprmekdj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3beunnsac.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wsyuqzkg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ohdawxqu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3otyiypdu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3iihvxfyi.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gyjjwusg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cfhtjllo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ikrvstps.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3yjwiugvc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rbzqepao.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zrsccmpd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vftwqnhe.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cmlpcihd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3prqwczuy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3wkypzubx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xjfajnbg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eilmdfmw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ehkmtkrn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3vhywwcme.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fckfpvyf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3gxhbbhri.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3znpmwflh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ssanxbpx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3sdyuwqdi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3hmyamrkz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hynbxsdk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wukigwfw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bhxmpekr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3dgwtdjtb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nijyekjl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3krybbcxl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3umjqirap.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3wwiebxaf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bclpzdpj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xtrcqqgz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ilehkmgu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3gvibhbea.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3eihowsaz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3brktrnpq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3iyplvyji.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3tifwmhjq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3fzapwjba.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rnchobbj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iniclskt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nnktpmcp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mrfqlckb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3cmvgkbdz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ihujkckc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3beonvblt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3knjqhuok.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3eibencfv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dcjgngro.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ajsgfbkf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vuvqkphi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lhfgioaz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3kqkqibdu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ccbmjgdn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kornygdj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3juyouxag.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gsfgkdqa.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ppmlttpf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3dbooflka.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3xejinshe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3napkdpva.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ecqgwuzq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ebhqxgfw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qpzfghdp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zkxvwjqn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vbjomwrl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qtupmpaz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3pnmwfzam.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3eoatjpiz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kqmruvea.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ugwjgskb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3puefodva.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sxbxnuyj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wmyjhvhf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3patggubm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rgtdagyg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wvceayha.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3sluuxbup.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3gkyzdbbq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ctpqhlfw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3bqlthapo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qpjsgzbz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ldtjufri.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vhrofvqr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tljyyxnr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jvjjktkt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3phwoihgu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zwquihph.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3whmpyirs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jklkhiih.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lrxkmxdk.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3okpdyggn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3apnvacza.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3smlzciep.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xtiikgnx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cnvqpbap.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jhdqcvzr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3domjludk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3dqtcmmzc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3bkznemme.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3tnctqtzw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3exnzlpin.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dwlfarub.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iqyebtte.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3vwtvagwn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xkygznvn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3czsslyof.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xlmrajlt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3uggytodi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3lsoarmrh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3pokspawx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3loudcpxx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3rnlramin.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3izeclrnt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3criwczfr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3imomyghe.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ujxbdbrh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3txzozfck.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gttnjwlj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vlszixyo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hqcpnnwm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fmwxevqo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3euqmuajl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jkkveums.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ymisrzrl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3zumcryfm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dbfijpsi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mjqgqvrx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wohlojjf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3byvqelzh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ebbxnbfa.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jlbgnhnt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nvjiqrir.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xjllmmxe.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3tfthtfyy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3fdcqdiyc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3prkstyec.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xxmtvmqc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qcwgwfvw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ivpulqaq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wjejatre.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xmmodbtf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qwutumeu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3bmjdqqvm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ldmshkua.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uyjcwysj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fognnszd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pnxavhgq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ubrhhijz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tqyntxml.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ynumngwc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3spmjbtej.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3dwyyjlsp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ufjbikvq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vfgxcpgg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tyvhkgwz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ufggfzkb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ccqshdnt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3kvzodahb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cnzpgiqp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3bcvoxrco.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jhulorij.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3jsrsrgkh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gmrgreid.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3umzojbzc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jvfvcrag.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hhbvqjvs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3zvgffnyc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ialfoxdg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3grlbqcor.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ppiapwns.html


<!-- 参考信息 -->