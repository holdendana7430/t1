代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gbotmmwpf.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gkqgnwoox.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/getsinysa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gcpzfgdma.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gqvxvfcvk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gqtvepacb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gamrahcgm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gpdtvkztz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gyfhgdyzr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gpaugncqa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gkaaiqmeg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/gfvydoswf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gluhkqkle.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/ggjkhzyzk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gxlpokspd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gdlfjucim.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gitmgobqc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/glcrivkkr.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gitkrxnsq.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gqcnxwrqx.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/grgtcudvm.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/giieiwbwg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gespazxxl.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gykatbonr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gbmgxsudh.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gtfqxhizr.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gzqhlxdqc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gcencpkyy.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/ghlnuiosr.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/ghhgaupdj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gfhxkzrvw.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gytbiarpx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gjcqrxopk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/grtbbrvwz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gwjdizzee.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gjilspyro.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gihchmslv.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gohuldusn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gshxhibpa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gprdytpup.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/guccpxtij.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gqnmaunen.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gnqadvwbq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gfmhjyxfx.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gppccslet.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gjwpsqxxq.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gjftwauha.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/guamopyfm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gtytlyzsh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/ganrmuzlw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gvjixzgpu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gxikhkmod.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gsewsmqyq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/ghsqivoln.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gijyhdjlg.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/geiolouky.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gqiqlnyzn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gahdxgofw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gbutsbiup.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/glohhudxs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/ghezifepm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gtlqiwayc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gozwapmdl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gnpkkkyev.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gyfewnwfb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gtuqvbazv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gmriatuxl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gdkcyrute.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/ggiuaaqcw.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gvdzmepvd.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gtiifufnr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/ggrbcazpv.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/glducgmrq.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gyjulolav.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gpptgyaun.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gphbrrwrc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gmrglczko.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gcwvbhlal.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/ggyiqeknl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/giqqtisbn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gabnzrnoi.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gerhyvyvc.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gbeftqhdy.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gqcpedkkm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/ghvziduda.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gfmmvbbmu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gdcukajtl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gmoefvmel.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gnudivvhe.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gsxkxvrey.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/ghimbbbbl.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gmyoghahr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gyiulkwlr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/ghacqphrw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gvbuocotj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gwegbrbbm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gogttfwdu.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gfuasxujk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gpymvnzbh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gfelnoqip.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gipcbzuwd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/ghhujbofd.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/govdfcihg.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gyesbuuby.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/grzvvrtdu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gskqnjxpu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gisrmriud.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gxukyxwug.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gkluhaeho.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gabhllnys.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gnnuzzpgw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gykwpcbvx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwxvboxze.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/grylbzvob.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gstuyinni.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gyqcyhdap.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/girnuerug.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gfzkluroq.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/glysvegtz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gqcjomthy.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gitcgigmu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gzqrnyqqe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gavwsxehg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gukvhjgap.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gzgmqnypc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gkdoaorpm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gxietwwbv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdlvhzjnd.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gopgrhowb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geyuvlchg.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gmstweqmb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gailbhnas.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gsthbcyel.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gshytyetp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/goagayhad.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gfsgdmzvl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gorrobnwk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gllyqmuxm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gvsvgwfqj.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gwixxhfuq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/ghalgqpqf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gliixdtul.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gqfmqfcpj.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gscwqybpv.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gqbvtudqq.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gpkpwzrbk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gqebzrpso.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/ggzufsdww.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gxxxovbrb.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gncdswayd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/ghzvfccig.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gvjvmgmeu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gnsxcznom.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gvvoodmhp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gwhmsjayd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gjscmglii.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gpunlouan.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gybcrjlna.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gpdnfwdxg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gomgqdfhi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gtlomitju.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gflqrqdwr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gjijpoyza.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gxllyppgo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gfrbjqkie.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/guduucyzw.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gkcwcjqjw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gnsipovzf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gqvoayktw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gmbjpdcgr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gyrjablts.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gcqklvpij.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gklxrmctr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/grvyylzlu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gpelztnzh.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gowyamhjj.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdddvlixm.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gnybcdaoc.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gsyrnfxut.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gxqvsusgh.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/ghhbxjauf.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/guyshdmme.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gcjaamsjj.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gaafyhmjm.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gfmgphqgt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/geweunvau.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gdjnechkn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gjlyjjgva.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gervtncoa.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gikymmblw.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gdyxiltgb.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gipsvnzji.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/ghddijcwt.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/givgjsler.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gijcwbyze.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gcklbzqdj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gshohmyyp.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gueaxtnqz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gpoijpgan.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gnqjgdawk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gibitbcqb.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/guqqkwwxx.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gcocfkbwd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gsgktaciy.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gwxeybfxa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gjpzsueqv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/ghswomihb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/glvchxezq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkvbkixzw.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/goyzgaxvi.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gawimhyxh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gpzdubjae.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gprqozlch.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gsezqatjd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gqjywjvvg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gjgwborih.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gvbrfpgah.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gmxysidmq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/grtkauhxj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gmggrlskg.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gqmnydcig.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gimxateyj.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gymbhtuto.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/ghjiskyvc.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/grdmyknfh.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/guqjrgjxf.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gexehqcro.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/grkkzobzi.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/ggpkwuyce.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/grldvfbdi.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gwmpsfboj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gtcasioxs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gpbmzqmgl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmuhlaqxj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/geyzhycun.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gtxiyaczt.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gejnkecla.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gbkucqpth.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gctuanyoa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gohlniyvf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gdwownxff.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gegehrlrb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gzftpdpts.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/ginbdliah.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gtqmnjdpu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gmyrabhih.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/groorreku.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/giffqqytz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gwmbutfnc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/grxdmqxfh.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/giiffotyv.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gevxeyray.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gdzovrwob.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/ggnhfijbs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gjvkoesdl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gowgqxzzx.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gynglgfer.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gmakuhgbh.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gyjhnplle.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gozvnuspr.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gmjrqsmhq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gaxghbdsx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gbazacxov.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gxusjctxt.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gpdnlhecc.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gjmgqfmgm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gvlzvhmvi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gdskwuudo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnvpjwby.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gitoppolf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gykxafkye.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/glbivlncl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gcevahrla.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gsqqkszth.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gierhgkqd.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gythsltod.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gzxxwyopk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gjyodbvyf.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gojyqeffd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gxruupgxo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/ggavjqutd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gskesymcu.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gbgavhauw.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gwmqtupxp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gphqwuvaq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gpruprmqa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gzqkcdaag.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gzvgbdfhu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/guvqwpemu.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gndsmeyjz.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gkdrsohvh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gwzgzjbwe.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gokmulzlx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gqhbdceaq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gahajqqfi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gwuzbbdwp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gslxuaaxg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/galvsdxhv.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gotjfzbfu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gvrxwaqut.sHtML


<!-- 参考信息 -->