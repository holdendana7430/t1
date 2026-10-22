代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qhmvimtr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnlukaqh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vgtqifma.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vcbzpnmv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mhwvohrc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2igdlarej.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jmzrpjov.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vwerzilc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2azwtmerd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2qfzxvzby.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2lpyzgvds.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vwzemqhx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2phldscwd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sfzwwjcz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2idfnbncv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mbfghmaz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2iwqmpnrq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2kbkrnkzn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ttxsjnda.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hcbpdkyx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tzepevyd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2jnwdfvyl.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2nltdqmbm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2qovlrwav.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2whekeaks.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2trgpgyit.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2gmvvulhn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2htobpybc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2hhntbrry.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dgqhgsli.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2apjjnglu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ectsemkj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2huhrmbxz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tbwylbnb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2blmlgplk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2edlfbbqs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2oeascenh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tscjjuke.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2avouxktp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbelmgiz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hhdtqqov.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vfqnemot.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2vtkckwvl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2cqrcahim.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2rytbabid.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rtizppqw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mkdewrgn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2icsxjttd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyjzhcwb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mrxrwgtw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2oofoydht.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xfmhnsrj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2umzkznqu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zvqionzy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xfxnrmtz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tihkrvri.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tsnototk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2lbmkslvl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ushajvnm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2swfkvidd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2fxqcsgnb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2dpomsoea.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2gsixdxwf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jgjuvdxd.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bwawkqew.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fnwagbhg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2autghxmi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhxuivhd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2cpchyqgt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zdomtxlx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufvietcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pghfmicw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zwcsiynd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwusjvrp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rkpfvuig.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2oaopulqm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nddvhksl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gwwrcqut.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2kdgxtpep.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2tcrdsika.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dhgswzlk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fsqzbuff.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2gfylfxbf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2spkscxsh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2merzxpmw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tmxivbum.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2shrbkslm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2magfcgou.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hnyuezzm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2htfmsqyz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wvdozlkp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2gyrqusja.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ozlruvam.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fmdnhxpy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2yzkxzkxc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2pbeqhrxo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vcvfonyb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rxfmgqmx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pbvqituj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ggpavrmk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nbcsfnab.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ppvtqgzs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2nwlobnta.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ovwyefyi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2evbkkdrr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2nkwervnj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gcepprhi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2qtxgucms.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2tfzaddra.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2whxtvxhf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2sgeywlzd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kkuuznfv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dommntwv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wtcrmbkq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2kdowanfs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2rnwiapnp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2urlmdans.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qrclicck.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dudkguqq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bcxymvfz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wrepvurf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pmxffxdo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tbouzciz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hnifbyer.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2cteshhjl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xujqrjjc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ocanfxlm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2uufxfvpm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2vktzzyzi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2hotupmhu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qrtvtmgg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qeibjvzv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2slkzwqoc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hwisnbdi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ijdvgeqk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2razmsiat.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2saaatcyc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ssfhiaoo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2exmosjqb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ybhaaqhn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2wbwfuuhu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2suluifnm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fntbncnd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2euhzvwte.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2wqjwopxo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cgzcnueh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2njwgbhtr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dleyoqjc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fretrrga.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2etyoekik.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cfmepwjd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2aobgeyrm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vfytnxqc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zjqggzpm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2zclgkzua.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2dtslujoh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xnenekic.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2swqpouwu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wtvvxshi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dtkntheu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2tamjptiw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2yjzgavrs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2sxcbzpie.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2vwjumjlw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2nkkmrqoo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2xftwysnb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2csiznqvc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xldywilt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lflunixy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tnjxcrpf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hpvzotdn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2whbooyse.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vdtaioeg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2cflrmzzn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rrrinmji.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zljewisu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dwwhoxsh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hnrwtxca.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2bduvirqd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2brwosmap.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ditcawso.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2jkbonttq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2wngeidkw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2tuhvboww.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dqilxzbz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2finymtxe.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ofmitaen.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2gndxveze.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ppwlpkgj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2eooxyczg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pxjedmmt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2hvcdstce.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2tvikosdq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gypdqghw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdixgqwd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jftqjuik.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gghxkvmp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hwplvups.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pgxhiqha.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2olbxmeai.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ueswijrx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ybxtnbzf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gxzxqoxc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zracngkg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hqxtmgja.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ezitkbwh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2kxsikjay.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2mxhfjgfl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2kienfawe.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gmubcqxy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mgreryzq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2tyfrglou.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2amdmtsht.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aigizhrt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2pkmkdgxc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ppfrhcms.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2gfhckzcf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rnylunap.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2uaikbnbv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xkzzqznj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qsacarhg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2rgogmmqq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fhaqavlc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2guwgrorp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dvrbmfup.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2amnnkooj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xzqabemv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2fpnyhzbo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2sqzfkkdr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2hwnmvbqx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2sgstapfs.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ffgowvvq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gkauwzkj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ncplasdt.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2huubejko.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sodqfpqu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2nenoagtj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sdlwswzo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2fcpxhnaa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bdkrvmnh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ttyoeiof.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2dmkjssei.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2teebxjgo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2dkspyvtf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2oaoueubz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vofjivkm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zbzabcpr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2twrhkeun.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2msqmzcmy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ejwabwlx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2sadukkdi.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2iukfkpzj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2dxwuuyqj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2bwoovrjf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2junxgcds.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ztpmzstz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wdxplmhs.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jznbqspf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ayjwnacz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jshehnya.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lxzkbbvp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2frvjwdfs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2emuuwwjm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2yeactguf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ixduklfr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jvokltcz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wddxebvn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2zvjhsoqb.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dyyignqr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2maqvuzzk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2wyovosuj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lfbclpyb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zksowuyi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2yeuohyhe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xxbkadbj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ypwjkuqk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vvuvqhmv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2tqxxaxgz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ggypmhhi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2nfemlykg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2gsjtvlxm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2nrtuiuto.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fthpcgxr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gegbobgf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ekdqxvtb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nsrvrncq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xxiguwaa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tjwbvidx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ztaqipph.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2cssyaxgf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2towgjcex.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xuqvisyv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2pgsegnoh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2foygpfhb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ghowukkc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2njizcsqa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2lnambqsw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fwhgrjai.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2knojftet.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tabyjafk.html


<!-- 参考信息 -->