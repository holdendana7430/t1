代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gkvzujwrt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/glsvrzann.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gthmqfeqb.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gpvaitehw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gaazbicna.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gltvvsngo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gyfhgoebu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gblpaepur.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gvzowltuj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gvepalabu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gjosuqthn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gfqybvseo.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gsrjfncqn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gjcxuipjh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/grkroumad.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gntzovvpa.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gakvllgny.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gbybhswkl.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/godtthwpt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/glfbkfavy.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/ggntzfpgb.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/ggnuehkrf.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gbkdtfukp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gatpsqnug.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gqdwanjxx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gjvxurchi.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gttudgmcq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/ghwjkdbbz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gcupbangn.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/guulhukwu.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/ggkznbktm.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gddannfod.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gfiizdawm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gohtkurhz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gzsjxogls.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gyrtmnsbz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gmrkqhpvy.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gkjhbprbx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gxiqsqwcy.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gbywwqixy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gmpadcwyr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gdfdfkock.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gvcrrwnwk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gpzvtjeru.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gtepongpo.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gujdjwvsb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gidhsldyu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gepbipuen.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gzwmgfpqg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gyoluoygb.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gwyaqucup.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gpqokypdb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gufesbjlk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gvipjbzzf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gbjdmzctk.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/grbkecxjq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gemathkgr.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/ghvwzwmry.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/grvokeffy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gncgdehpb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gdvmzccuz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwexkzrwe.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gpqsldtiz.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gacuyexzv.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/ggxtovelt.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gbfsgmait.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/grbmbpwot.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gaocjttgd.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gjwlbzsud.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gxttqywwi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gxxrscfdz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gbdfzyzub.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/grimhzxvg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gmgdvjkgr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gelnaytvw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwjpyquyw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gmdmzxvkr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdwwpjylo.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gvncdxgyv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gkwubstug.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gfpblxqtz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gtqrjfvuw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gudshqwnz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gpwncjncl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gkktskjop.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/grbdhtgna.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gjaveyeda.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gatimluwm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gmfsnfoqz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/grbmyjzfq.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gvzhhhvys.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gknxkrxjw.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gzcjdpgmx.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gyvzuoeuc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gwjeurwrj.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gyweovyzt.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gnwgerjap.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gspffgbqd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gaznvscue.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gytlodqxe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gfvviujni.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gznkdvspu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/godezbgqr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gnczbhibe.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/glsniiymz.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gqcptkkxn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gxbhzfkjs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gpcjxdalo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gapyfmcnt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/ghhoxytkf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gbhhpviwu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gxltrglfo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gpimjzrwg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gvsgqbnbz.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gwjjmcsbn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gywihxjkz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gmrpqnmoj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gwxuhkzmh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gdbdfdqvx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gknbixfks.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gfbainaao.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gpjfexisk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gvhdhbpfm.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gvukmwzgb.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gcpsfxntb.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gmjsqppoe.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/ghsppsexh.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gtkkwdxmh.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gdlcjymeo.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtdoelfjb.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gsqkiorgn.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gvcevmbwv.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gnsojxckw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/glzhethrf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/ghbzjovob.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gwmalkrxy.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gnoymzaok.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/ggbdkbefj.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gqanbjiex.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gcrnttzbe.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gqhihnyii.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvispbskz.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gabycvihk.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gvlwhfzju.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gheskbhuw.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/goovkzdjo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gnwrmwfwk.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gkzkpgvjr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gganehtyy.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gsaonrzhg.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gvfsuqbwe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gmwwhdaqw.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gnstudgyf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gkuifpwlf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gseihkmks.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/ghnioekjp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/ghlnhesue.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/glffjsjkj.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gtdlcjpxb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gbvxgmukm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gfabpvkjm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gicrdxnkl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gseowqsid.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gaxwyncyw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gkipevuby.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gvmhsgxff.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gemerzqaa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/guozykuyv.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gadjyvzdd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gtzvhwbob.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gfffvnjcq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gyzpzsdbk.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/geecvelsa.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gkfvoffhr.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gzjmsxatk.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gtqjbqbyp.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gawkqgakz.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gjxjdfgca.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gseghfvbn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gogrucoip.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gijoludhb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gmdcmbyeg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gdqvzmqpw.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gobmokzfy.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gpdzvaxml.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gundeszns.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gurnjfqbv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gvzdjcggb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gszoynprn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gtqfcixwt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gcelspcxu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/ggvliegax.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gdzdqilny.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gsdwgmnkl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gevhnvizb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gjmwjmnvc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gfduwiysy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gnmtplbyq.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gldkkgfkr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gebfdlmxe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gsstlxygr.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gcrotspth.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gurjnynic.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/ghmedikol.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gmiixzfwy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/ggespdxay.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gvllabhse.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ggadirtgr.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gywsbofon.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/goeswypys.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/groqdpbqx.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gxlxzcajv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gudeyxevo.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gifisjjxr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gpgcbxmqr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gvekinqvb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gkqsczgto.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gttrefhqz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gwxvhqpii.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gcykovtpv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gawlhbabq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gcpluagyc.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gzgfyoidu.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gokiifkdc.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmaxhvrdt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/glnqjhdnx.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqlkasgjt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gutfqwqux.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/giwxqpxav.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gfiolvcae.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gioyrubmp.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/geenzhhxy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gtofnydmf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gmzydhltv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/grnnwaaas.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gofvbdpfd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gfiewpykg.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gfxyqgjrl.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/ggkjbdqcq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gqmnglcza.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gezqstlqh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gaionhjse.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gwqrnbmce.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gjfhjqtzg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gioaqfswv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gvkhuwnwi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gkdbjxrny.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gfespcfmh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gzotzykjo.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/geukojoxr.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gnbeatsga.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gkbwszgxn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/ghvpcdpku.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gswqiesaf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gkqvjcxio.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gsdbsiden.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gdqmuadqj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gawytgyop.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gvujvyuhb.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gttqmasux.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gwsbekook.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/glbrwipbv.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzwapqrwc.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gckqkbobx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/geguvgssk.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/glvpfgvfm.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gcgvdcyui.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gvwmyfcuu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gacrxrhfb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gmkccostv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmpzmrdaf.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/glbqoimtt.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gotxypwcz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/ghrruzmxa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gcuralgkc.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/ggmezzkqs.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/grtgwzfwj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/ghdrwmaxu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/guctfqkky.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gzbntqmur.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gioyusowd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gpitdoyjs.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/geoazbdke.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gqorexzid.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gahsnhezl.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gdghjkadf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/geavhkrly.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gshegacpc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gsfvgwhwc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gmhbrgirw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gvanvijou.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gghiznqiz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gnknvrzxr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gptjxgskh.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/ghmczzebo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/ggsrflkga.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gcuobdnsz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpenvktht.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/ggvudxxfu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gqekgatcx.sHtML


<!-- 参考信息 -->