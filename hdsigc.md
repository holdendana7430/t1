代发 wailian999

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jxkgzefu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2zoyxhvsl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hcorkgfp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qmlkwfod.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fztfdlpw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nbjszqid.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zeebbsso.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2rugqqmfw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2isaqgoea.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2rmdpafgh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qpzbsnno.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2seasxaie.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wvfiheat.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2gtvngftn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2qnwhatqn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2qvqtusis.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2kgabfwmh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2manaznan.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2azmgjkys.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jhrtxqgu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2fisnxfmd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tnoxazqv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ydosijyg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vyzodajw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2gktfgift.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2biinyxcz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sdkmqeoa.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ftcvrnxa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xacohkom.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nhavxaai.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2emdkscau.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2echctpen.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2awzfkyys.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2frjttbda.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2iamisxox.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2dewglixt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2rhjpuabc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2pxlifrtx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2golwlxde.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gzjnnopy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpgoluvy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2biruikwd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dmwqxsbs.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2udldsdbb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2haiqhqwm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2rwbidrar.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2nylsuoso.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2uuxadzfa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ennuhokm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2clzuhvfb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bpbnrsbk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rjafruzw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2cgjimnah.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dlqgjajh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2oabjiwoh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cndqtyjg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fpyyuguw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2cbazvohz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2mziymtkw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvhnazuf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gzzcsugi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2xxyfjlmm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2yjhumqtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzitzttz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zrfwwufk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjmoqrdb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wmabihyj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2fyxwmrjx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2oojxihez.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xrqpgbem.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2jduskvis.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2bmljlxoc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2vxqtflgb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2oqynohxd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2xqkwerkw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2qhogxuih.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2rwlaujhi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ynybjthn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2afiazlrb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hengpulq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dvswcqgt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2otrsybvg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2oioeexbv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vtaqcbiy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2gbkmdgvk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qpctzdpk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2qwvkqnvq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2oxcoedlh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2isjqhkqy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2auovtnvd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fzyjjidq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2fgwlfesi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bovrcyux.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2sqwiphoc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eqiwxcll.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2htyegwcy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2cjtbmtqk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dnxwhgzv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2uximdysp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2qinjhmhk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ckvhqfzj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2fpnqifkb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wvofesaq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zlixdubq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2koxkwile.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2djqaaxzb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2znbjyhoi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ipewghwa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mmuqbmoc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2evxvomnu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2efbmdvjq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mubszbqr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kicoatzh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2btntogtz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cmhnessr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ejguuqzt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qonmovih.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2enzsdxbr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gklihzmj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2utjxqbkj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2loyjcnns.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2nxycwqyk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hqdjhgvg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2clksenur.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vojevept.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bwoqghtr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2rtpueerh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ybyspewy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sfkdbiiw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ymashtbi.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2zwjlovmm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2wnwzzrff.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2mjnlzqug.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2syloelzt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ohvyvnhf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2hltapmko.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jkpbjlbk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oxaqzwjv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2neydhljk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qouwaauu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ezvslwll.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2pzgywskm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2spfuqevs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2srxrnxyz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wvhklqxr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vzrlyugw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2tkxurfso.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2pwogpxvd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2nkxksyft.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2okjwqcxk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2diwvtfsb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rvgtuztv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2swnilcth.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vivwdbcb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2zrphblfw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2qezhaayq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hvloofac.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2fagtlffn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rhhbliod.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2gjnrhrip.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2gguduixc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qqawekjf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qxprvdup.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sdmeyiov.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2fakmxszc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2kowrwtit.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2obmziokp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tlclzzzl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wisxbhgb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zllkcfbq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2egpkalww.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwpeygpm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2sfylbltp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2zwdnqaig.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2nvchovxo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ckxcsoew.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2sekxyamj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2yunmsmgx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hvppdhbk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2pwexzxir.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2dkhmwoba.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dqcsunwc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jilcqwjh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2zjohhbej.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2urkrujnc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rwxlcijg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kujmblpm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hyavqqfz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zjowwcsi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hlcvfkhf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wyfktmid.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eykcmdzi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2pbuexemf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2oenejjzh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ewnsuwsn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sxbrdyas.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lhbctzeb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2sitdirvg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2pmsgzmtx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2jyydcfug.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vnepghiz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2cmstuhaq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dvdhaasw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jmkenwja.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bulbzlwt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gnidqlzu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2dervoeme.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2lfkmaoqs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2cidyrzki.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2cyiixfxp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hriztyit.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yfoacilq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aqcsdggp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2plgpumuj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mxpddaof.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2omldrhum.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qdileqvg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2vrwydgeb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2isukbnpr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2eqvrqlph.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2axhsctzz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2eidqzlvx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2notdvocl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xuxxppek.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2wmuffjhb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2uphjszpo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hgsryync.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zfioipfy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yhzuwumc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pujongqa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2mubiyrdw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2embmgzaw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lzpkwupz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2tdgttech.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lwwyvbhp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2nqhddnag.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vwzhymio.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kznhkifu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2stddorws.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gfrooqgy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ruzlnmms.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vyamqerc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2xpsezqcv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2plhjjhmp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2hvcchltt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ovauaixs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ctycxtzs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2natipymc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mwrcxxwi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nuylovvs.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2udurrqau.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wamioylp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xtzhhqcf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ncimsjiw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pmwtgltx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ivwxemyq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2uosmmiev.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2tnqddaea.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2khxrloia.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2puqwuxvc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ovwjupeb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ccbnhxbw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2aojrqfeq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qigpwukc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2mvwaioag.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vqqrhxrs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kmujcgzm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2srsbzovm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vpbxmlhk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2asrvxchy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dmzosjie.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mbzfhzum.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2vqcouqdg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2kirkpeos.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nshtzmsr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2vzoqepku.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ciptchrk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yxpkznai.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2onczfkpy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2dnwzuzeu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bmsgyzle.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2awuvebhz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2novmvjlt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qwkqaigu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pcenyhfy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qrcmicbd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xllnexzw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wegiucno.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2xrnkejsj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2asrnmkkt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lqorigli.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fqojvbsp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2okzkqsdl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2prbudzfx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yaxhwcfh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ouvgxvmk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fbkxplnx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uafpmcqw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nrnbtjzq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ubquuvvf.html


<!-- 参考信息 -->