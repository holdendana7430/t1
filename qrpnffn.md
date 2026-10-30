代发 wailian999

[C10] 变量作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/glaadwrha.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fanxiaobao.xyz/Article/details/galwmyoxl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fanxiaobao.xyz/Article/details/gelfraywj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcqfmstl.sHtML

TS:   同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gyfuzukps.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrdyqyad.sHtML

Go:   花括号块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gwogmddlo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmqlpsxo.sHtML

C#:   块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gwblqqodi.sHtML

[C11] 模块导入与导出
来源：http://wap.fanxiaobao.xyz/Article/details/gsiveenkr.sHtML

Py:   from module import func
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhywgwjv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwdnbkkz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfsppnkx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwqzjtwu.sHtML

Java: import java.util.List;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfutnfjcs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fanxiaobao.xyz/Article/details/gncuzmwsf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiynglla.sHtML

C#:   using System.Text;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsspqbxt.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fanxiaobao.xyz/Article/details/gqpyebmhp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemwtxwbu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fanxiaobao.xyz/Article/details/gclbvgjrz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fanxiaobao.xyz/Article/details/gnxrmxsbr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajtffjhr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdniefnll.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glowkjhxf.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fanxiaobao.xyz/Article/details/giodcvsmy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grqjrxszk.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fanxiaobao.xyz/Article/details/glzxrvgyi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfdtboss.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbbbcwgja.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpxjmrnd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/galhfgbou.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghllijywl.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fanxiaobao.xyz/Article/details/giizrrxfx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgulkghf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fanxiaobao.xyz/Article/details/gszrwyphq.sHtML

[C14] 泛型函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gicdmygan.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fanxiaobao.xyz/Article/details/gccjymgls.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpidhzlkm.sHtML

JS:   // 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/grkocabju.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdvuudiaa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfaoqnejr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fanxiaobao.xyz/Article/details/gqonfqylm.sHtML

Ruby: # 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gioqjzrpz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkergfqcx.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmscobqf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fanxiaobao.xyz/Article/details/ggezemnwa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcbcjanm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbtyqjlt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwqiatwm.sHtML

Java: // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gelshzxaf.sHtML

Go:   // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guavbtcnt.sHtML

Ruby: a, b = pair
来源：http://baike.fanxiaobao.xyz/Article/details/gqvqdvifa.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/glgkksucv.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrszslki.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fanxiaobao.xyz/Article/details/gjtcxujeh.sHtML

PHP:  // 无重载
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlzivkai.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fanxiaobao.xyz/Article/details/guwctaree.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyxltnmc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmcludyb.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfluntsq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fanxiaobao.xyz/Article/details/gukfbsbbj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gytoyiirm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwgoeifzl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwopwrfws.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmtfrdark.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gwxyytmzc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucjdofuh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/goruisjwt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fanxiaobao.xyz/Article/details/ghtofcdtc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fanxiaobao.xyz/Article/details/gziqubavv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fanxiaobao.xyz/Article/details/goqjtdnzl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fanxiaobao.xyz/Article/details/gvztwfccz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioowqclx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fanxiaobao.xyz/Article/details/givbxjuqe.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fanxiaobao.xyz/Article/details/garqstqsb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fanxiaobao.xyz/Article/details/ghidewloq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfdxnjdb.sHtML

JS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gphfrbqyq.sHtML

TS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvxinice.sHtML

Java: list.add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gqbiyejti.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwlogflc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrkdliqy.sHtML

C#:   list.Add(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmmecjfb.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gowipncqi.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnsruccf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gygguhpnk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fanxiaobao.xyz/Article/details/gorpgozft.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gitygtaxb.sHtML

Java: list.add(0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gyvmjdelp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gystprlwk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvcgpfyy.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/guoqwdmkt.sHtML

[D04] 删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gcpgidgzt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyrgxuni.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gmwegnbgz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fanxiaobao.xyz/Article/details/gdljxdhqw.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gozjntnel.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fanxiaobao.xyz/Article/details/ggnaujqwl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiuhetyc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcliuwjt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdiuwcws.sHtML

[D05] 访问与修改元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gvytgfwcu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbiqzold.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyelmwuyb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlmfxgyx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnyfyebg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctqnzeti.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gebdlemwa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/ghipcbirc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gjoglintt.sHtML

[D06] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gpxqjhhoe.sHtML

Py:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gkzaswupx.sHtML

PHP:  count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzjepvwl.sHtML

JS:   arr.length
来源：http://mobile.fanxiaobao.xyz/Article/details/ggacifdvg.sHtML

TS:   arr.length
来源：http://3g.fanxiaobao.xyz/Article/details/gwbwmsjfj.sHtML

Java: list.size();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhaxblnc.sHtML

Go:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gihkwtrix.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/gbvnuxjcy.sHtML

C#:   list.Count;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsthoywcw.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fanxiaobao.xyz/Article/details/gixvqeypw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdmyublj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbzsvvfo.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxpjtcyt.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gxccqrqpd.sHtML

Java: list.subList(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gypzpkmsg.sHtML

Go:   arr[1:4]
来源：http://3g.fanxiaobao.xyz/Article/details/ggqrjckaw.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/gocdbcvll.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gymqpsabc.sHtML

[D08] 合并两个数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnennehw.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbajzfcda.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fanxiaobao.xyz/Article/details/gaclcyzba.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwhwhfbh.sHtML

TS:   [...a, ...b];
来源：http://www.share.fanxiaobao.xyz/Article/details/glodhorpm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gpbdvsxdx.sHtML

Go:   append(a, b...)
来源：http://m.share.fanxiaobao.xyz/Article/details/glknmbxnk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxswwyjd.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gykxsvyuo.sHtML

[D09] 排序（升序）
来源：http://wap.fanxiaobao.xyz/Article/details/gagvgigod.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxheadgoj.sHtML

PHP:  sort($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gojvglzta.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmkprxqo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fanxiaobao.xyz/Article/details/glabqarqq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fanxiaobao.xyz/Article/details/gujwjcssy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gofwggjis.sHtML

Ruby: arr.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnqqwxcc.sHtML

C#:   list.Sort();
来源：http://wap.fanxiaobao.xyz/Article/details/gyeeohtry.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwtioyfw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrvspjfz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdcdizca.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvcfbwdn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvajtactx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnctcnjw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fanxiaobao.xyz/Article/details/gsrfxzfnn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fanxiaobao.xyz/Article/details/ghhsaiwwu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnorbrtlt.sHtML

[D11] 反转数组
来源：http://read.share.fanxiaobao.xyz/Article/details/glhwzqeav.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fanxiaobao.xyz/Article/details/gdfnaqiih.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gcwnckskj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsalanuc.sHtML

TS:   [...arr].reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gsagkspjr.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvfvahsv.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gqiqhyftd.sHtML

Ruby: arr.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgmojgwz.sHtML

C#:   list.Reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gllvxfeuh.sHtML

[D12] 查找元素下标
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefkoedxt.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpgiyihr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/glaccznza.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gddypledq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbgmooux.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fanxiaobao.xyz/Article/details/gftrjkbuw.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gamsmfvla.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrssgfte.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpujeeqe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fanxiaobao.xyz/Article/details/gweanjalt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gogidqxzc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyejdjrfr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrwifmwx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gnyqhrnmw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujcmlzxm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzvuwhvb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fanxiaobao.xyz/Article/details/gvpazutas.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/galxqtxdq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioaujtkq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsfbvzch.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gfujcdxyu.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqmfejqa.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gdkhnhyvw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gonmmzfsh.sHtML

Go:   // 手写循环
来源：http://blog.fanxiaobao.xyz/Article/details/geghgjrjx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjjrclnb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfqvnnvu.sHtML

[D15] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gtytbmsvt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gleextlmu.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtebqjzog.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gwprrcvqi.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhailpbg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fanxiaobao.xyz/Article/details/gouqsthbx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwdwijrh.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtchssfl.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gryyiauzq.sHtML

[D16] 求和与平均值
来源：http://wap.fanxiaobao.xyz/Article/details/gqmjjkdie.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/guuznpgrn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gnqyltyvp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/grhunczqh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gcngckeev.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxmojyar.sHtML

Go:   // 手写循环累加
来源：http://wap.fanxiaobao.xyz/Article/details/gkpqbsyqn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyysefbw.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fanxiaobao.xyz/Article/details/geaxhbgkf.sHtML

[D17] 最大值与最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gdrlyuyoh.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gbyoaufdh.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gqeblhtuz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gjwopgtde.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqjeukzq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gzxxtdkph.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxiqwsao.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fanxiaobao.xyz/Article/details/gszdkipiw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuburzao.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fanxiaobao.xyz/Article/details/goupczjoh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gupbpangu.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fanxiaobao.xyz/Article/details/gfvtwicwt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzydtcgb.sHtML

TS:   nested.flat();
来源：http://baike.fanxiaobao.xyz/Article/details/gztferocq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfetmxaok.sHtML

Go:   // 手写双层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gojmptusd.sHtML

Ruby: nested.flatten
来源：http://blog.fanxiaobao.xyz/Article/details/gvezmifqx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjqdvycn.sHtML

[D19] 按字段分组
来源：http://wap.fanxiaobao.xyz/Article/details/gfccnvyjj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjhkbhup.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmeaagec.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fanxiaobao.xyz/Article/details/gxdpfjdnb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtabcmkwo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fanxiaobao.xyz/Article/details/gejarlgat.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeasatju.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfvovkwe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fanxiaobao.xyz/Article/details/gqusjrfgj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glndqinni.sHtML

Py:   Counter(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwdaoqww.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmagxzmxj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/givupuygx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/grisjvyru.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fanxiaobao.xyz/Article/details/gqeyyrorf.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fanxiaobao.xyz/Article/details/gwcftdxor.sHtML

Ruby: arr.tally
来源：http://blog.fanxiaobao.xyz/Article/details/gidkscsor.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlkjrwma.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fanxiaobao.xyz/Article/details/glrxmacch.sHtML

Py:   x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/ghjjynglp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gvxkmtgbv.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkoxyxfg.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwkmpghy.sHtML

Java: list.contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhixbekc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyktshyu.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpnmcmcv.sHtML

C#:   list.Contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gakdkluie.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fanxiaobao.xyz/Article/details/gjphqgzrs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxxmnkcj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fanxiaobao.xyz/Article/details/gbkwfofys.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxpauinj.sHtML

TS:   [...arr];
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlxsdpeq.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmxvvwjz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdqcnjvi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrinshqw.sHtML

C#:   new List<int>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gimmwceaa.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowsybczz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqvqlphg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gumdygmja.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/ghtbezhak.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gjidguxqp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzhdrafp.sHtML

Go:   // 手写循环
来源：http://blog.fanxiaobao.xyz/Article/details/ggorwgfdw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fanxiaobao.xyz/Article/details/gaivuciyl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fanxiaobao.xyz/Article/details/glojvbxmf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gphyuvcri.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gaufqwkxh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gtduthism.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaotrgmb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/geojdsaah.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gavmwywzz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcsmkxjr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpshqmxwc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdasbsdlj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrvmcekv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fanxiaobao.xyz/Article/details/gtqjcdkxw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/gskuirnjz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gpngyvdgz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeowdvtj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsymbgrb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fanxiaobao.xyz/Article/details/gpytejzzg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gvbdshoxk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjsgqbhym.sHtML

[D26] 数组转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyxwumee.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gbijzsvlf.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gifqswmph.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwilpkum.sHtML

TS:   arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gotodhhxh.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllzylklj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/guuhnwvyx.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcdjmwiy.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fanxiaobao.xyz/Article/details/gtbiflulf.sHtML


<!-- 参考信息 -->