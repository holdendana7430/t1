代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/gdlvmklrw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxtxcyrw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhbdihto.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyyjymtp.sHtML

[C10] 变量作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gjyneqffm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fanxiaobao.xyz/Article/details/gfqieduao.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fanxiaobao.xyz/Article/details/getyzxtip.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvqgswbp.sHtML

TS:   同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjvsvjbq.sHtML

Java: 方法内为块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/grdxrqlxk.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbajazjhh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmxskafq.sHtML

C#:   块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gmugegpkw.sHtML

[C11] 模块导入与导出
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlusgstz.sHtML

Py:   from module import func
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzistgbo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fanxiaobao.xyz/Article/details/gktljeuqo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/ginywxsak.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdnffobu.sHtML

Java: import java.util.List;
来源：http://read.share.fanxiaobao.xyz/Article/details/gamdghase.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfguckyly.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fanxiaobao.xyz/Article/details/gioauohrb.sHtML

C#:   using System.Text;
来源：http://wap.fanxiaobao.xyz/Article/details/gfkimsdpq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fanxiaobao.xyz/Article/details/garearsuh.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fanxiaobao.xyz/Article/details/gpapdrray.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeigspus.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gvebzeazp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnotwqtv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fanxiaobao.xyz/Article/details/gnxrbwgqq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrluevru.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuagfjuo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdingzunb.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbbqmetu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gyjrijmmt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelzldqkt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaxrtana.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwpklnwd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnoxgipv.sHtML

Go:   func add(a, b int) int
来源：http://baike.fanxiaobao.xyz/Article/details/ggrkwwrfo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fanxiaobao.xyz/Article/details/gttggqtdy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbqparbx.sHtML

[C14] 泛型函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjfbfgxgk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fanxiaobao.xyz/Article/details/gubkkswwi.sHtML

PHP:  // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gviohfcpf.sHtML

JS:   // 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/goylaqhxg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdzcyzjaq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbihnowz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzkrzimm.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjebhzia.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fanxiaobao.xyz/Article/details/gkfogpfuu.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gobedbecv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnfgxuvb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqmaqpne.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxyedwzn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtvmxrhs.sHtML

Java: // 无解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglntnsue.sHtML

Go:   // 无解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjkffzqg.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnmwtnst.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fanxiaobao.xyz/Article/details/gbdtqcsln.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fanxiaobao.xyz/Article/details/geokymwbv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscxkuqvb.sHtML

PHP:  // 无重载
来源：http://blog.fanxiaobao.xyz/Article/details/gvxlscoot.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fanxiaobao.xyz/Article/details/geiqojxhu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcdgvxjo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnhdyljh.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcwzwfeo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gextmuruw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/glrqazeyv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnuqvapnc.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fanxiaobao.xyz/Article/details/gbqqtbhvy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gazeyokzm.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduwovwyi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdiesnif.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubwnphrq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnacqscbh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/glsjjdhcu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fanxiaobao.xyz/Article/details/gybxzmlzc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fanxiaobao.xyz/Article/details/gjvrwmwvp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/gqofctzuj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslvhvrjy.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gazrnjwiz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazhjvxum.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/grkzgqgbi.sHtML

JS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsynrpua.sHtML

TS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gattmruut.sHtML

Java: list.add(4);
来源：http://baike.fanxiaobao.xyz/Article/details/ghixkrdjz.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqqdztxe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyedmptt.sHtML

C#:   list.Add(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzomsytu.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasjsnofq.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gwbndkhdk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fanxiaobao.xyz/Article/details/gdzgysfln.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fanxiaobao.xyz/Article/details/glczvppnr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gkacuezvw.sHtML

Java: list.add(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gekcyhuyv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfrcfbuf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyvwdjtg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsjmzyhy.sHtML

[D04] 删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gzbarfdng.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvycegmi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gxyxdgtaw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawspkqjm.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gzglwcghw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaeamjfd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fanxiaobao.xyz/Article/details/guyyuqxsx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gqqvtxznm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjarmzhz.sHtML

[D05] 访问与修改元素
来源：http://baike.fanxiaobao.xyz/Article/details/gnkvrcabi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/gecpycgpf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gdsyxcpmp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gxfelzrnp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwkarsne.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fanxiaobao.xyz/Article/details/gmmkolkan.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtajxone.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/grlnkzrwp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/ghothwbml.sHtML

[D06] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxoetipc.sHtML

Py:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gtntaqozu.sHtML

PHP:  count($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gtikoxxey.sHtML

JS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfxidedk.sHtML

TS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/goswpdadx.sHtML

Java: list.size();
来源：http://wap.fanxiaobao.xyz/Article/details/gvktkzixb.sHtML

Go:   len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkaoddoi.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fanxiaobao.xyz/Article/details/ghpqkjdwh.sHtML

C#:   list.Count;
来源：http://3g.fanxiaobao.xyz/Article/details/gkfnfandv.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotctlfzz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgpeghgn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gylmspjmp.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grklcyavg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykjtwovp.sHtML

Java: list.subList(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gnwjerdbh.sHtML

Go:   arr[1:4]
来源：http://m.share.fanxiaobao.xyz/Article/details/goebiywdp.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbgrtnit.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhzjmrlz.sHtML

[D08] 合并两个数组
来源：http://3g.fanxiaobao.xyz/Article/details/ggbiziwqg.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gcuhrpgxh.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoarcitt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fanxiaobao.xyz/Article/details/gfqdwdhbq.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoktfeyn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggohqjjuq.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciuyfqsg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnnpgzee.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gckwfzotv.sHtML

[D09] 排序（升序）
来源：http://www.share.fanxiaobao.xyz/Article/details/godkwmwkk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/guwjfjwai.sHtML

PHP:  sort($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gdmzfhczk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fanxiaobao.xyz/Article/details/gkktnkgcp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczgdoctk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnoplkkp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzagxxhdh.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gozrqoucs.sHtML

C#:   list.Sort();
来源：http://wap.fanxiaobao.xyz/Article/details/gxtzhfnyx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnziysfvn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ggjvosvpy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gccdcknzw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gbbzzrjgo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfwlbano.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkdraklm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fanxiaobao.xyz/Article/details/goibbngrd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpkgfkvc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fanxiaobao.xyz/Article/details/giovntboy.sHtML

[D11] 反转数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gtakqejrh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzvwugvb.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gxbzdhblz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fanxiaobao.xyz/Article/details/grauwarya.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fanxiaobao.xyz/Article/details/grtqdprmf.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpefycat.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gomewlhsn.sHtML

Ruby: arr.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gxhugundq.sHtML

C#:   list.Reverse();
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxrcgffr.sHtML

[D12] 查找元素下标
来源：http://wap.fanxiaobao.xyz/Article/details/guydbkhgh.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/gkcsvsxeu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/ghcjqbqzi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gtuivfmrl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gnpqdpziq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpihbhwzg.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gjuotxriq.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltrlveho.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkndnpkf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fanxiaobao.xyz/Article/details/grlwmvzyn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexlwbtyl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/girjuydhh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gpxqrcfja.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gqoyzsuex.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gekmdeajs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fanxiaobao.xyz/Article/details/gscurbnun.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fanxiaobao.xyz/Article/details/grtfbwlwc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gmmtkrnby.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fanxiaobao.xyz/Article/details/ghcjtfnxg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrfukvmf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/geydklvlr.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkeduydd.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfrdmamb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gqxmxxpvm.sHtML

Go:   // 手写循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpffrnky.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzoexiqt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gaczeucby.sHtML

[D15] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gmcccrhkv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gkclpujlk.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gugniwqyy.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gfhbrdmuk.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gaihwpqnf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbndgvum.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fanxiaobao.xyz/Article/details/gcclhnrzu.sHtML

Ruby: arr.uniq
来源：http://baike.fanxiaobao.xyz/Article/details/gygmqomtr.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guawglbtn.sHtML

[D16] 求和与平均值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlwoqeml.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuqvjmra.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbkyxtor.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/goisznzip.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyfpyspe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcjvbmyv.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqldrykxl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/ghjwqutzp.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fanxiaobao.xyz/Article/details/ghipcsihy.sHtML

[D17] 最大值与最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gnncmmyns.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/grgctryws.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gquleaffc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejdebyfp.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gumxjdtwf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gktoqyvwb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/grixfspnu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzyhabla.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurodmbwr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxrcjrpn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fanxiaobao.xyz/Article/details/gyyagyquz.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fanxiaobao.xyz/Article/details/gppvytrpu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fanxiaobao.xyz/Article/details/gtjetwubh.sHtML

TS:   nested.flat();
来源：http://3g.fanxiaobao.xyz/Article/details/grgqtgwak.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxpufbum.sHtML

Go:   // 手写双层循环
来源：http://www.share.fanxiaobao.xyz/Article/details/geqekxiec.sHtML

Ruby: nested.flatten
来源：http://read.share.fanxiaobao.xyz/Article/details/goeezgaxy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gajxfyoqw.sHtML

[D19] 按字段分组
来源：http://baike.fanxiaobao.xyz/Article/details/gwenltsyu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gvavfoiqn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmphgabe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fanxiaobao.xyz/Article/details/gklpelpux.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmblyjls.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiyzurjg.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fanxiaobao.xyz/Article/details/gnowuymyp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fanxiaobao.xyz/Article/details/gtvnbquta.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjqsvsqq.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvgcpvtn.sHtML

Py:   Counter(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrbptidr.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geupgvedq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrgrvavg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnpcgdyh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpyartjf.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzffposj.sHtML

Ruby: arr.tally
来源：http://3g.fanxiaobao.xyz/Article/details/glgqyqrqg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fanxiaobao.xyz/Article/details/gpftnzivg.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbebifif.sHtML

Py:   x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/gmybluhva.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginethvsp.sHtML

JS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gkujqqjhh.sHtML

TS:   arr.includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxymkqws.sHtML

Java: list.contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gkzzqtiwj.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gjusmuqji.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprjolamq.sHtML

C#:   list.Contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/giidbfcuo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyacqjlmp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gvxigkhlh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbxmtqng.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/greniqaoy.sHtML

TS:   [...arr];
来源：http://m.share.fanxiaobao.xyz/Article/details/goewgtqnv.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmrtqdiz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/glumjsydd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fanxiaobao.xyz/Article/details/goklrlecg.sHtML

C#:   new List<int>(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gucjewval.sHtML

[D23] reduce 累积计算
来源：http://baike.fanxiaobao.xyz/Article/details/gteqzvmvk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gkifgddta.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlzpeqbo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/grcjexjjl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gscuigsxd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxknkojq.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdsntdxs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fanxiaobao.xyz/Article/details/gciytnkpl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fanxiaobao.xyz/Article/details/gnoqgoqmb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrkngehq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gywtrduqb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdcugdwu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gichvwqgy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgdcmteh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gjgvtopou.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gascmsdou.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fanxiaobao.xyz/Article/details/gejeowehn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwrveujx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskazcgef.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fanxiaobao.xyz/Article/details/gaafvswxm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fanxiaobao.xyz/Article/details/gcqaaiibr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzpdwmgs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fanxiaobao.xyz/Article/details/gacexfxfa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gnetanvot.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlwsamwn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fanxiaobao.xyz/Article/details/ggescvkxb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gedksugkt.sHtML

[D26] 数组转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/guqzfymmn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzjobsrg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzuncirj.sHtML

JS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gltwrxbgm.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwcvpsxn.sHtML


<!-- 参考信息 -->