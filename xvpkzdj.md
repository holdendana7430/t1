代发 wailian999

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gcsibdkdb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/ggmvtugdx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gwcyxkxqv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gqcbuotde.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gjczsqrtb.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gfbpqamel.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/godpmnzgy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gwfzypjxm.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gtkemgeyf.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gwmkdsviu.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gumyfekvm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gewikxqgm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gqntnsbat.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gnfalqqer.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gkdtpwrlo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gcydgumcj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gcxilgmgh.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gqqvzypga.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gebienxdu.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gmwvogszr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gaamfdzrk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/ghvcurule.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gfibwwjfs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gcrczktsh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gwsxasmby.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gdfacpzss.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gqfpslxeg.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gljwgapwc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gztfgwvje.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/grofplprh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gyihnovxm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gerapdaut.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/glufgruhr.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gkrisvosh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gzspoexmg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gqyhdqukv.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gdlzizcmt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gowbsyfbd.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gbashjvuo.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gkipsisee.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gdbpdvjep.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gnfjyunnk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gvubvdbzp.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gufnhcsxd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/ggvdwkryg.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gzvstwabi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gdfjucmcx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gubcyvnsc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gmxrzeowv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/girqtpyqf.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gpwlwwrae.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gptiocqfg.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gfwplszos.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gvwiwkkew.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gvjssheug.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/grygludgx.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gtztpzjzn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/geogygxne.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gkunuroyk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gezefrspt.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gqwatzarl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gmauqiqoh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gltxygptl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geamzzzgu.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gtegdtbjf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsuezzzxv.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gyaxcxksm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gbfqzwakb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gwvjvbspi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gjtdbwyqa.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gbmvvpamb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/guvtrmany.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gpvdxuduc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gfpelmjmm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gbbacflpk.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gyqyzdjcl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/goakfyvbf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gbavfeuti.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gjxhxxfqk.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gpqkxgtne.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gslewnnis.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/glyncszno.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gslvwgbiy.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/grqabnnbu.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gtlgjbfzm.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gxzwonbaw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gvhuuuktf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gqforroec.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gmpbvylkd.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gcltqtqqm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gjpyvnvrl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/ghvnyaxfr.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/grlyapoai.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gudegdquz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gesbuetei.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gvthtzdyy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gpzmaypdc.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/grhidcyks.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gwxugtvgp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/ggforifws.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gikwxcgzx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gaeioscog.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gwiyfbkdc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/goflpasgf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gtlenctzr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gaipqlhew.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/ghmmwaumd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gmykybvpy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/ggsrnutzc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gopwduphh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/ggxtfounx.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/ghycaincy.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gxbzizrkt.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gtlwrvkjc.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gjmwdgidk.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gsmwfnvis.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gwmbyzlml.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/garitaxbh.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gzyopssgk.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gdqfgirac.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gsoyzvqon.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gpqduoqnu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gsdbkdpwo.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gqjyhiycw.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gxdlashyc.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gylznsrsj.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gledfbuae.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/grofpfmwm.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gtmiijekm.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gegdqvkvt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gfbjzyyja.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gjcuqnhqn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gugctrtun.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gugnzwarl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbucntnqr.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gqzemingl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/geufsdwps.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gxepypdfp.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gfyxxhsqa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gdceenike.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gcggvyujk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gvcgihyqc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gjinhfeno.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gqcxpgqkd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/ggvgmtqww.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gshpzifxd.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gegrhookm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gedvdjjns.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gvjubdynf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/glrmaujpq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gjoesqexi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gnvebaxhx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gepsrcgax.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/ggppdeoaq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gptjpzznd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gjfmtbnsp.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/glcxbcqic.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gvbjlahqy.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gebmhliiw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gsnbhagrn.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/grtwfsivm.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gebsgwmji.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvafduaum.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gwdvmgnpj.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gidgkhsos.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gvjpeyziv.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gbvlbyxro.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gtologves.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gribgtddc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/geczadqxr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gjcrtjlup.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gedpxzemq.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gtivhfzbj.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gdquhblrg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gnmtkqztv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gpxiuouik.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gfmvftwrh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gotcnuldd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/ggghkzgym.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gjwkexmzn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/ghpqnedsq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/grbrhwpgc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/guhtaxkqt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gwwyypqvo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gaeaqnkbv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gbhqubrot.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gkdkpwnvo.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gficfzblp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gedcykhuc.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gwnmynttt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/guzetwzxk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gbvxzsylx.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gkeoubzaj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gujpgqejk.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gffpdikrt.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gkxhlhcew.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gopjrgjal.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gyekktadl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gaxfucqzl.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gjfocsoqs.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gwlehirxg.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gwgoyxdax.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gyxivedcb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/ghwlzdmbz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/galelwijo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/ggsaryvpf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gdgxhegwj.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gxhfwszos.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gyjcayzgj.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gxyedzdrm.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gxppivsbt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmfkjkhff.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gvfvxxehg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvrhsrroj.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvdqiqnws.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/glaxqevhb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gniluhddf.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/ggcmyambr.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gfwigfllr.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gqfizetjv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gkvokeawg.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gsxhhbgkr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gtesmyyzs.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/garezjsci.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gxlxesztd.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gmwzufqae.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gchhtpeom.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/garkuxgux.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gqpbskqco.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gfvsvbpgn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/goiqrhpwi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gacqkxpcn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gwuvgduss.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gtomifupg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gaendlmmu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gqlfglhio.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/geciqcwdy.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gjevqoihm.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gswcmcmwl.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gwgcjnqfe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/groviggob.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gqvynnkhy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gsvistzrw.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/ghbeomtab.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/ginnyknxa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gnjyclwey.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/glxsevibc.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gxenhsori.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gbbdpxfmd.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gijkkdhic.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gncrjlsvt.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gkqppbjud.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gfmxlxham.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzggsnnwg.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gcieubfig.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/giwarfejd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gtnkmzsrh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gtzgjjdah.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/ghtvjhrfl.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gtxbscjiw.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gnnhpuuim.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gwnbbttvk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gkpnuthjm.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gnclqxmnb.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gkddiixvd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gxezfkqbv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gnrsvkogz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gkascdyns.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gnmvjymxt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gocaqbpsi.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gxucjzjgz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gryctcybp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gomgfjsvn.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/galswotej.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/ggqplrakj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gzusbdruh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbzuremm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gmjebiemw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gmfpgjjjs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gslcsqwpp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/ggivkjqxx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gpclwpuyt.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gnnsrdfre.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gereikqfs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gkspvjqnx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gyfazbvnk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gdygcyflm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gnjoqzfzf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/ggcogzzaa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gzotxhikg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gmrmrxrvb.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gzheoztgp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gdtqwqtst.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gkrvdookp.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gtfssnofk.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gninwgkdq.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gcwvsutcx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gqagrdkto.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gobytbfoy.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/ghdxlnlcm.sHtML


<!-- 参考信息 -->