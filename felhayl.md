代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzfflvrt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fanxiaobao.xyz/Article/details/gvqjigjgh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gplxszzej.sHtML

[C09] 递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeutrrnx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfialsdv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmmuyyed.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsfvvnqs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzgncxff.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/gtwhhxxbq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fanxiaobao.xyz/Article/details/gypzrjwyf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpwpwrmq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoixvbis.sHtML

[C10] 变量作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrioaqax.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfkhsvha.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fanxiaobao.xyz/Article/details/gjhjaaxih.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gtswrigpx.sHtML

TS:   同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gveseusak.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjzkljhb.sHtML

Go:   花括号块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gjnhkibwf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfxlwgbt.sHtML

C#:   块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvvrckzv.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfhbemye.sHtML

Py:   from module import func
来源：http://3g.fanxiaobao.xyz/Article/details/gbnldsizp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaomrrwh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gootejghn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqdfuqqs.sHtML

Java: import java.util.List;
来源：http://baike.fanxiaobao.xyz/Article/details/gyufctqmc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fanxiaobao.xyz/Article/details/gcfbvofdc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fanxiaobao.xyz/Article/details/gikhsevdr.sHtML

C#:   using System.Text;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdivibvq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkvhlmtn.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcipvyri.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcpfocrk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fanxiaobao.xyz/Article/details/gomfmdqxg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/grnhaamja.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fanxiaobao.xyz/Article/details/gnszswbnz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxjibzdv.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqacxega.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzjnekgi.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fanxiaobao.xyz/Article/details/ghoxpumxj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gtbcilhtg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxjsfdol.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfieyjac.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjlxyscd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gubtbnbdp.sHtML

Go:   func add(a, b int) int
来源：http://blog.fanxiaobao.xyz/Article/details/gliwssauj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fanxiaobao.xyz/Article/details/ghnimdwsi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbixgagp.sHtML

[C14] 泛型函数
来源：http://mobile.fanxiaobao.xyz/Article/details/geqilucrg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fanxiaobao.xyz/Article/details/gojhjnbug.sHtML

PHP:  // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspbwrwye.sHtML

JS:   // 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gofeiicij.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvvzfyay.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gnktsyeik.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdsugkyk.sHtML

Ruby: # 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gdmjafqmu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeicidzv.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxgrlwpr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fanxiaobao.xyz/Article/details/gnuxzgzoy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fanxiaobao.xyz/Article/details/geyhxgqof.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggbwquntp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gbdzwmkfn.sHtML

Java: // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/ggszodlrj.sHtML

Go:   // 无解构
来源：http://blog.fanxiaobao.xyz/Article/details/gidyssiiw.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwnurluk.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrknlptz.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpwitzqb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gorugxznf.sHtML

PHP:  // 无重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscqnhneq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwfmpidd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnlvvkpl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsokhdmrt.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkfsejdw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsenyvbmp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmywnses.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gocmnyyxu.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fanxiaobao.xyz/Article/details/giuemrlpf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmdgrgqld.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkwlibqv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fanxiaobao.xyz/Article/details/gmpgmxaqe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fanxiaobao.xyz/Article/details/gcbhdfoxw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gackzjoml.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fanxiaobao.xyz/Article/details/gygcyfxts.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fanxiaobao.xyz/Article/details/gjcgsrqnj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fanxiaobao.xyz/Article/details/ghjdkvtlq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfvbtmle.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fanxiaobao.xyz/Article/details/gzleembvp.sHtML

[D02] 追加元素到末尾
来源：http://3g.fanxiaobao.xyz/Article/details/giqearkfu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fanxiaobao.xyz/Article/details/gwdppijdo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhciywue.sHtML

JS:   arr.push(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlhwakcb.sHtML

TS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdungmfiz.sHtML

Java: list.add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gskmeodvy.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/glgprildf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjofcmvt.sHtML

C#:   list.Add(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkidhfptq.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyafufig.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gskmzaoco.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnvkgdja.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fanxiaobao.xyz/Article/details/gbxyzbdsx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgoarevh.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkkfpmhv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gvivjcczt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fanxiaobao.xyz/Article/details/gvnkwcfbk.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gmgnfooca.sHtML

[D04] 删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gljpnzxhw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gaptfdenz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqekayhg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgqslgke.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuimahxt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gxdgdkqvy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fanxiaobao.xyz/Article/details/gorhlrsdj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gphdldpjw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxguumzy.sHtML

[D05] 访问与修改元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ganpolgdz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gbasfaiiz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gphbyctud.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gpnvrfedq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqadheplr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzdkvwbe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxhmloov.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/genqgjhuz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gwupudlgy.sHtML

[D06] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcsvkwmn.sHtML

Py:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvnhdsgq.sHtML

PHP:  count($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfojwvkft.sHtML

JS:   arr.length
来源：http://mobile.fanxiaobao.xyz/Article/details/ggekkbwus.sHtML

TS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjnxvgky.sHtML

Java: list.size();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecpgqicm.sHtML

Go:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gnqywztuh.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkxkhybt.sHtML

C#:   list.Count;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmrmbzjl.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fanxiaobao.xyz/Article/details/glwxhjcqr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwrfawmz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/grbssrvpa.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gahesyrwp.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfopjoxm.sHtML

Java: list.subList(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gkqntzqzg.sHtML

Go:   arr[1:4]
来源：http://blog.fanxiaobao.xyz/Article/details/gbjgznxau.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtfsbsfk.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/geuwyizzb.sHtML

[D08] 合并两个数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gpippecth.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gynvidlnb.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gshwzqikh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdsminup.sHtML

TS:   [...a, ...b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvaxpsiw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjyxkntb.sHtML

Go:   append(a, b...)
来源：http://read.share.fanxiaobao.xyz/Article/details/givuvpqbn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxxjlnnu.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzctrpoi.sHtML

[D09] 排序（升序）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoitsxon.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafjpqvsx.sHtML

PHP:  sort($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gqravcnhi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fanxiaobao.xyz/Article/details/guhuntrch.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvdbaujz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdajebsy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gklmppfyu.sHtML

Ruby: arr.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gkzfsvila.sHtML

C#:   list.Sort();
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhezwkcj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fanxiaobao.xyz/Article/details/gpxybwcrq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gybtlkkmx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgtrciiq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/grqgmdnaz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fanxiaobao.xyz/Article/details/genickbhy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsplgpnce.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fanxiaobao.xyz/Article/details/gnjvntpby.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fanxiaobao.xyz/Article/details/gifebpzwb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyxfonbj.sHtML

[D11] 反转数组
来源：http://baike.fanxiaobao.xyz/Article/details/ggctibjdb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkzethgy.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcshrjrry.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvdfagmr.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/gevnnfotq.sHtML

Java: Collections.reverse(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gjbzjakdt.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gizycyhtp.sHtML

Ruby: arr.reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gfavjcyen.sHtML

C#:   list.Reverse();
来源：http://m.share.fanxiaobao.xyz/Article/details/geahbyikr.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guswkxsbr.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/gaqumgkhc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyofucdjt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwobnivhh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpygbpwl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fanxiaobao.xyz/Article/details/glvevyssd.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzdtygry.sHtML

Ruby: arr.index(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gppnbiebp.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fanxiaobao.xyz/Article/details/gsawzgwzy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxcvnsjn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiedtovz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaripdbh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljutzwmc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gapwilslq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govjlzfib.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdxafzja.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvewdenn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gzzxpunvp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fanxiaobao.xyz/Article/details/gqbikpeoq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gijlsfmbg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/glmrroeui.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/goryrafeq.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzgiskqz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gcepxvhcb.sHtML

Go:   // 手写循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoiwnjfq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gsrbtjdve.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgpnacsx.sHtML

[D15] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/givbaiunc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzhvnetl.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdorsdbl.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvimnsxmh.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gegvebmew.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fanxiaobao.xyz/Article/details/glbfdnsnk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkjonesn.sHtML

Ruby: arr.uniq
来源：http://blog.fanxiaobao.xyz/Article/details/gpshqglux.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gccfbtycb.sHtML

[D16] 求和与平均值
来源：http://3g.fanxiaobao.xyz/Article/details/geabfmycu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoodxjdi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqmbxckd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkunbhscy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwliwmyog.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fanxiaobao.xyz/Article/details/gerwreyle.sHtML

Go:   // 手写循环累加
来源：http://baike.fanxiaobao.xyz/Article/details/gyhvswklg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fanxiaobao.xyz/Article/details/gcijopsbk.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fanxiaobao.xyz/Article/details/ghurddwqg.sHtML

[D17] 最大值与最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgvlirga.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gmfrlqetb.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/garuusdsi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigcguxqm.sHtML

TS:   Math.max(...arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gqjswfknl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbshobeu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxalobat.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqvqukgy.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxvgqqsk.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fanxiaobao.xyz/Article/details/gzhrtbdzs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fanxiaobao.xyz/Article/details/gwfegfywh.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fanxiaobao.xyz/Article/details/gnuiljcuo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegbrnlrk.sHtML

TS:   nested.flat();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfijscftg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkctmnvf.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggomfccbg.sHtML

Ruby: nested.flatten
来源：http://baike.fanxiaobao.xyz/Article/details/gxcrzhpgh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gqdlaskps.sHtML

[D19] 按字段分组
来源：http://3g.fanxiaobao.xyz/Article/details/gztjeilgm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gnjvyrdob.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fanxiaobao.xyz/Article/details/gktedqurl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxdxtcqp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwumuksk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fanxiaobao.xyz/Article/details/gffjlptnl.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fanxiaobao.xyz/Article/details/gdvgnbqny.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsotsrahe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdnyziqy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpywtlgi.sHtML

Py:   Counter(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrdwjult.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gplvitdmg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gifyiqsxx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvcjbakc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fanxiaobao.xyz/Article/details/gssqamqis.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geczhbibr.sHtML

Ruby: arr.tally
来源：http://3g.fanxiaobao.xyz/Article/details/gplizkcza.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlbabcix.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fanxiaobao.xyz/Article/details/goytnvqdm.sHtML

Py:   x in arr
来源：http://baike.fanxiaobao.xyz/Article/details/gcgfgppat.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fanxiaobao.xyz/Article/details/giuxoceoy.sHtML

JS:   arr.includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaivqphvc.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygzusdqq.sHtML

Java: list.contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/guzptxqrp.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gwruzejqv.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gusffznww.sHtML

C#:   list.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gcdbmioaz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjrrpggw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwcrzjib.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fanxiaobao.xyz/Article/details/gvakzcjth.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdofolay.sHtML

TS:   [...arr];
来源：http://3g.fanxiaobao.xyz/Article/details/gpdxlliko.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyzmllje.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/gwhmwcumr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fanxiaobao.xyz/Article/details/gyjrptyjt.sHtML

C#:   new List<int>(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gbleflrhf.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrdybipb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtszkxphf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcqgfldh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtpjbgyf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzatmcguj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fanxiaobao.xyz/Article/details/gpxqpzrgy.sHtML

Go:   // 手写循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbjkzrjd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fanxiaobao.xyz/Article/details/gakbbsjjb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fanxiaobao.xyz/Article/details/gxmefsczj.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fanxiaobao.xyz/Article/details/gmfplglok.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fanxiaobao.xyz/Article/details/glbxevlvh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gdakkkrib.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gfllzoypu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgxuntbu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fanxiaobao.xyz/Article/details/gyvlpxmbc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fanxiaobao.xyz/Article/details/giagxsgny.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjntqibhm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnddolte.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fanxiaobao.xyz/Article/details/gaazetody.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbxpxuzl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/gpshxwsdf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/glmjjelds.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fanxiaobao.xyz/Article/details/gmytobsrg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnikdjkx.sHtML


<!-- 参考信息 -->