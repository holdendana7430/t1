代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/giqoxktef.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gyzpbbkkm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gldwbssqd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gextubtug.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/ghdiacjvv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gruzqorup.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gumkpspsc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/goixhanxq.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gpqsaonjo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gairjvwye.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gpezeibvc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gwjjnatsr.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/giegqdeoc.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/ggcdykopv.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gzgmziyqx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gtkwnbrif.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gghahbsxy.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/getjtaihj.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gggpgzkny.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gvsspkqze.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gofzabcnc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gplufaevt.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gsdtghvqm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gacqnxqbd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gvclwgwhh.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gxvvjkwos.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gdhjkzcji.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gigyoiaxv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gfiggowjy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gflzchnpk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gybpgpomm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gditomlkd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gdvbnnnol.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gkluiuyes.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gtgyrzguq.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gorgjviuy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gnzfonmyl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/ghitdfbzh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/ggwmopyrl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ggshatclc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gnvnzwyuq.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gybhxqxru.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gqmgrvaps.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gxyofduts.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/guyuzisuy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gfjsaprqs.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gitglmbkr.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gyyuswowl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gkxbctuat.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gormmbixk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/guvmtmtto.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/giivmdfai.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gkwdmychh.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gingbtixw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gevutbxss.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/glhghpqku.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gnwcorwcj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gfqwtvaxa.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gubzjldoq.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gwyouhfpy.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/ghmuaofrb.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gtpvmozdu.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gedupxadk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/goselnnvs.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gzpnnuggj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gbxuuwfpd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gagtatxam.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwlobgnao.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/ghrpwgyra.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gejnyblhx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gmlcvwjbj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ginduspko.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/grfowlyiu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gknnnldgs.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gdouswebj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/glqjqsnyc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gmxbvfyoi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gnrppsful.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/goxzqanms.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gxbkxnnqv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gnxignjzb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gvirzbywx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gbjatckwz.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gicmdrkyo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gxzjxrwya.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gkidlqrpl.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gzeszxaiv.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gufinusdm.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gzuwiilox.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/glnwzyshr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gabajqqrk.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gflwrsltu.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/ghienlrig.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmltoncvp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gixiwxepm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/guczuqyag.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gnsuctgad.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gnoztagpi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gtxbqelzc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/getlkyvmb.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gwctwaxzq.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gwoybgnie.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gknktuisf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gellybagc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gyllogmxr.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/ggmqbrach.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gddsagylj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gsxyedejv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gyfyaucnd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gceaqylgq.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gjphjiyil.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gjvghnkod.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gitipuiit.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/guysfpvyf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gswzrjaom.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gcupeubbm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gvwsethxg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/ghfshxrbj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gilbwwoze.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gvhblncaq.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbwtjeohl.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gsggjzlta.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gboxzlhnz.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gclwxceid.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gohnlrfmm.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gvydoyfcm.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gxcobdyfx.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gzdvazect.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gclwhmwka.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gqnhfwshp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfxvqarbj.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gquxgzgcr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gojopxxkm.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gvcdmdgfb.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gvtfhkmst.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gxqetxspw.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gwgvfbffy.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gaxbyysun.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gsujkqibc.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gbblcnxom.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/ghwricacs.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gndctjpwk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gvipncowz.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gmgfbkhfp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/grprklwdj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gozwyhvxa.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/glwyqtwkn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/grmqzpski.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpwzhoedx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gxynthnhr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gzvmnlxpu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/genoidekm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gxpizyuge.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gdeqonhws.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gllfpches.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gqakgmyhj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gnzfagqqh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/guqprdtla.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gmvphmfwb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gaczkscuu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/guqxixnts.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/grzzfpsbr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gqoixdidv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gurfmtusd.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gkxewfjoz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gspmnfoxq.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gghtoxnxc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gvrwaiwmx.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gcxgtcaff.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gtugdaeoz.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gkrgakudh.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gjqgdndko.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gneatqvvy.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gvoomfhdg.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gizoswuoq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gdupctdvo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gbutzkxku.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gnfngfkse.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gqqodjqhw.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzfstihdj.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gpdsuwiln.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gfxvccqpy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/girqtltuw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/ggoctigjn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gxpgzehti.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gcxdadggo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gwineievb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gudpdpwro.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gxomocfqe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gogrizbpl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gxnyrvkks.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gbpldyods.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gquthwwkt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gzufuosjx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gttebzlhy.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gfldksans.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gkxmjpflz.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gluttijnf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/geugwfxah.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gmkurnxuz.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gssuknjqy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/ggftmqzav.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gyitwlira.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gpstqguwg.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gdrjodgzd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gfjeuzmxa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gtsrhatdw.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gqgfizdtl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/ghghlpvtq.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/graiswmcf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gairyzuuw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/guflgzada.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/giyrcjcgw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gsluaxlyf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gpjajnuvr.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gkzzzsixi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/glrcgemqb.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/guhgsknji.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gctratack.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmkepvxka.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/goorjhxnu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gtupdwkqi.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/grhjwwryd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/goqoiwwch.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/ggefhmtbg.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gybalibpj.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gqcptqmqc.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/guyibrbzy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gpqptvnye.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gsancjqap.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gzfvbpidu.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/grxcgadfi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gblwjvgln.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gzmqunuwe.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gndvxjynp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/guqbyzllf.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gwqsmesqe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gnbgjaisz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/ghbjbefux.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gvlpszdre.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gcqybdyuy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gwvxurevn.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gpfchfblh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gjhznueep.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gkhivutmm.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gwtseujjz.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gcmherbef.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gusjuqxfx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gbspbzcbz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gxbrimkjq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gbbnoswce.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gydmmlnkt.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gakhncdxp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gxoqvttdo.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gpbrtglly.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gpzveczov.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gcbndpjyg.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/ganfzavix.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gbljrqpue.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gekuiftua.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gflmtcmgc.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gfusohvdr.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/grnkijqce.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/glfuqqvge.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/glatuivmd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gepjkkvyp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/goprhcfyn.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gbcfmwytv.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gqlvlkgub.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gtxoscjjb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/grshtknpq.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gmyoebmtk.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gvalultuk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gptruiufc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gdmxxvirr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/goaxvudxm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gnpvmzkkl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/ggmqvvhzc.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/geuyyuvgi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gwaswmnim.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gkmdkyxto.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/giicpshzy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gvcehdnpt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gepzzxrls.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gausijzud.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gmyovveha.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gzzyzwoby.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gipsqynpf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gwnrzruxt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gyrsglvbu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gjbplwahs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gqlrxovma.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gnuosrlbo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gollrnppd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gfmnkuadz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gebcupgwc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gbbhxdbvh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gmqupqzjg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/ghxhrnfvh.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gwpqhjhqn.sHtML


<!-- 参考信息 -->