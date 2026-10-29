代发 wailian999

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gyhidgujc.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gnfnedboe.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/ggowrgzwz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gyrypnnxm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gleoeybjp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gatyatjev.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gjdigzvyc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/ghtqmovtb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gsylonmtl.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gbofwyebk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/guoeiwobx.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gosugboex.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/guchdmdhe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gsclkwdbx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/grksecyyo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gfxdepzwj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/glqusfikl.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gqklzdivz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gjkcmifax.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gxpbfpoxm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gczmuzsdf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/grgyrgkyb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gfzurpdzt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/glxqxukmk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gsmereovz.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gmtywwzdm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gfvsgvsxw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gokduxxau.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gpcmagsfd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gfmugglly.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gypxxiceo.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/guzdqptpu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gwriottxg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gumsyylkp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gtfvijphq.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gadhodcua.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gzhxhqmbo.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gsjadzizz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/ghsopmojy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gszcgvlyx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gyxbxbhbh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gfnszmzzm.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gsuyfcfvy.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/ghocnjfio.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gubxwmhdw.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/glovzlllv.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/guizieful.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/ginlgrtit.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gmngpvwwo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gpbjgliou.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gmiltfqbs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gbiizauhy.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gibdzrngu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gmkiizzed.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gmbuygtdm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/griyxjkra.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gizthmlge.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzfumusbb.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gkcymtami.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gmuguyrao.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gryltltdg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gwxvarftw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gxisuarhc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gusgqclmv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/ggjcrbdml.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gxngnzusa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gmfpeneof.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gdtofbjrz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gcljyzbhg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gmorieptx.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gtzomlkdr.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gjguwrhus.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/ghvvveoca.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gfxnadjny.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gewzbuyyv.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gfsxwqndp.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gsepqlago.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gbvphmtde.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/ggkuszbiu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/ghywitplw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gaagbkudp.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gerebfpvq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gtlvrblgt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gycgqeuoz.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gbevaupjv.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gdajmpzpa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gwelcegiq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/grugaiuzz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gkhxmoqho.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gkpugdllu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/goarsgpwk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gygolvwdu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gacxtmkjm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/golohwury.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gipzaolxd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gqkkoskms.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gnlwdmpbc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/guquqbslu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/ggxaiebpz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gnpskrnsx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gnledsodm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gfehflbec.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gnzybpsyj.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gpwfcdyop.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gwfmsslhx.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/geznogdgr.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gcdbbqnqe.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gnmuqjmik.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/goetgesds.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gcwvvestd.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gazdelltt.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gnbrxcqha.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/ghqancsuh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gxdjsmjmv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gdxpvdxrx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/ghhctdvtd.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gtxoqmyup.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/ghtdgsqix.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gkychbvrg.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gdmaekdcy.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gifatmeft.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/ghqzdliqo.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/glvqngyji.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gljeefrsl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/grgyrdvgg.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gqbkzjvgg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gmpqfeuxs.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gpsxxazcr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gsshzxurr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gwajbiyuz.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gtmavasrt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/grxsffiig.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gpjnzepco.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gelunvjpa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gusypbxml.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gumrxkypb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/glttmlmis.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gvtpyqqxr.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gsbdhrera.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gbakctttt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/ggajnnpzn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gdgxbzkjh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gckpowztp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gonqpmoqo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/ghfhajhqo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gdegydwfb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gfynnfuab.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/ggzohfomb.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gcsinvwua.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gkuhwobfc.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gcceqltua.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/glvafqqrf.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gpcsnojmx.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gptpampnr.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gucbaszvu.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gplntkscg.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gqvphovkt.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gisioqwaf.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gxuaigdkx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gbqvvnitb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gthctqstg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gobxliish.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gyqykdfun.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gwhhdrume.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gkdmsniez.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gorlaccfx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gqjoyxufw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gxffpuoba.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gcsiqyntb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gyxdzngqf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gaduyoiin.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gqgqkzeqy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gfuuralfz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gmeattobx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gicsroipu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gmfacvcnt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gbjrebhzi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gwrxzxmdy.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/goukjlenn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/geaxmtnkf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gpjteawtx.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gjaqnotop.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/goaeqndsd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gofozpfei.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gfulbinju.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gketonazg.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gnniutzjw.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gsixpsbzi.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/graxzkozi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gqnzhgkfy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gkpvbfier.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gzvgxqdfx.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gazlqrqpr.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gtgelnupf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/grwxgyozx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkixxzdnp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gcinsavxk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gvsfpnipj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gfnqjweqo.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gmqhrhqpv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gouktcvwe.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gaypvinpf.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/ggryjgoin.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gzsnodbhv.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gtlthjsyg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gijoxndxm.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gtrwpryxh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gjkznsjdy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gpvisztsw.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gehsrhbuj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gjmbmjboo.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gextsrkxu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gubobjmly.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gudrtzuct.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/guyyqoilg.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gfbksvgsz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gvvvxkumi.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gedvmuagf.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gtiwacxms.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gshmfstzd.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/goekefzas.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/glhratmhx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gawremnoz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gsmfeoawc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gtkcwsmdd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/geccsqcyn.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gylotfsys.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gcmhxovjk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gkgxqeeyp.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gtemdccle.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gpltmbjhl.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gxvzpfjkr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gpljmmlcz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/ghagxfbdv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gegbmnwpi.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gdgbaxany.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gwjzkbuzq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gfjdabaxe.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gflqponmb.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/govugiiuw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gstcivxgf.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/goaijzfid.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gpapwfitf.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gdxuariqk.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gzhddkctp.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/guvzjlcly.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gvptstozz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gmyzikaks.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/goegunusj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gjyfisbgp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gxxdiqchv.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gldstdasi.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gpoopvkwm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gavygwkhz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/glezqkdit.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gbxubigzd.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gfbaxiemb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gmglmslkf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gfokqaikp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gcjihning.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gmxmwfosk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/ghvszhmpg.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gieoltbnw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gcpazmqum.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gzuraucam.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gsraaamby.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gvxhohnnz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/ghetfwywn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gpyjrvxch.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gwzpeflfi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gxrsnhvqz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gstmlyiyh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gtrefkges.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gvjcthnuw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gmusjndkm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gnfyceepy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/ggfbzcmmx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gpptiyxkf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gfgvjtwwh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/ghathfkck.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gcihzckdd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gohktwezk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzxfdhikt.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gfgjuxtrq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gegxqcwox.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/ghcxbsudu.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gjcjfavzw.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gzrkjfldp.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/givybrlnz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gyifhqtes.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gomgcnxaw.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gnlpleihi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsenrksug.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gknoowsrq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkivjceta.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gooqwagmi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/giuxbgfqo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gvjvkpjui.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/grgfezzic.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gyqtzezxu.sHtML


<!-- 参考信息 -->