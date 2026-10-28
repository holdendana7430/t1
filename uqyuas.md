代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://hz.jiagoushi.top/gtohalwlza.html

[C03] 可变参数
来源：http://hz.ppjwa.cn/gtudxfnhti.html

Py:   def total(*args): return sum(args)
来源：http://hz.daria6918.cn/gthreyobgm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yongpay.top/gtvcgocxye.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.haohaochexian.top/gtszftwrib.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hysaishi.cn/gtyfaartsv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shanyushiyangtech.top/gtskyajdxz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.fzhhl.top/gtwlevavjx.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinghuilouyu.cn/gtepyjwpcm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.daxiang520.top/gtlwuopuxo.html

[C04] 命名参数 / 关键字参数
来源：http://hz.nanxinkj.top/gtwurzpvqh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yuxming.cn/gtdqvpxzga.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.andypj.xyz/gtozdvxuyl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shzxlz.cn/gthacyiays.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.9152youxi.cn/gtoyppxumw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhaomingkeji.xyz/gthmtpoxac.html

Go:   // 无：用配置结构体参数
来源：http://hz.hywenlv.cn/gtphdktmjp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.kuanghao11.cn/gtibnyggjw.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinqigufen.top/gtyuosghit.html

[C05] 返回多个值
来源：http://hz.yj20258.top/gtllwxkpht.html

Py:   return a, b
来源：http://hz.shuidangran.top/gtxgoxbzqc.html

PHP:  return [$a, $b];
来源：http://hz.shangyingyoupin.top/gtoflibemz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ehwqpu.com/gtnpbsnqat.html

TS:   return { a, b };
来源：http://hz.hnqzz.top/gtgwnbppip.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gotoacloud.top/gtghginsrw.html

Go:   return a, b
来源：http://hz.yvedp.cn/gtvxvgkvfo.html

Ruby: return a, b
来源：http://hz.zycfv.cn/gturaiqqbu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gogol.net.cn/gteuwqwkgq.html

[C06] 匿名函数 / lambda
来源：http://hz.cheryme.top/gtlllnhshy.html

Py:   square = lambda x: x * x
来源：http://hz.c1oappe.top/gthapguzbf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.tian-w.cn/gtptabiwwt.html

JS:   const square = x => x * x;
来源：http://hz.yj20258.top/gtwecsqjld.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.52xcode.cn/gturvgtagh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.mhx1999.top/gtnohizizj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cdnleiting.top/gthwfijugd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hnxiangtu.top/gtpdvnlcep.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj20258888.top/gtagcttbeo.html

[C07] 把函数作为参数传入
来源：http://hz.chenlongwang.top/gtrhupzijj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yj20258.top/gtaiynikbn.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gaohongyu789.top/gtohmtpsoo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.guannengcc.top/gthfvcrkej.html

TS:   arr.map(String)
来源：http://hz.yj20258888.top/gtikvgbyoz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ivvv.top/gtkydrzvfj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hnqzz.top/gtwjoblpjk.html

Ruby: arr.map(&:upcase)
来源：http://hz.yueranfly.top/gttnfiqwyi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.smart0.xyz/gtnnqwvhye.html

[C08] 闭包
来源：http://hz.xuetiantiany.cn/gtnyvmogqk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.feifeiyinyue.top/gtdxmmrpzv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhixingplan.top/gtmgygrkzs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.pycfn.com/gtovpzybdb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtuppoosdl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.dashuyun.cn/gttbjzyaqj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gaohongyu789.top/gtrfikpexl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xziqi.cn/gtbsphalxf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zycfv.cn/gtryqunkoj.html

[C09] 递归
来源：http://hz.cheryme.top/gtopgqejwd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zycfv.cn/gtxesrezdh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yuanzhike.top/gtmpppkcky.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ywan-chungtsiang.top/gtufkdnvrd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xylfe.cn/gtmbzcagxe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xziqi.cn/gteaoappav.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.c1oappe.top/gtrlzevvov.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yuanzhike.top/gtzkhndglp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shanyushiyangkeji.top/gtlqptpnuy.html

[C10] 变量作用域
来源：http://hz.jyoumei.cn/gtkjoolpio.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.kuanghao11.cn/gtjqjpwbds.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yuxming.cn/gtlubwpqjl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hysaishi.cn/gthelejxgt.html

TS:   同 JS
来源：http://hz.hongshengwenyu.top/gtohxuwtvo.html

Java: 方法内为块级作用域
来源：http://hz.shanyushiyangtech.top/gtybpadrsx.html

Go:   花括号块级作用域
来源：http://hz.316326.xyz/gtefofcuim.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.quarkkingdee.top/gtptxkdwtx.html

C#:   块级作用域
来源：http://hz.hfpthk.cn/gtvftghtjn.html

[C11] 模块导入与导出
来源：http://hz.jyoumei.cn/gtybhvwbrb.html

Py:   from module import func
来源：http://hz.yangfankeji.com/gteghkcwyv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tian-w.cn/gtvsxbsqpx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.pengpengdd.cyou/gthvbuomdj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shanyushiyangtech.top/gtclwkfttd.html

Java: import java.util.List;
来源：http://hz.wangshuangyany.cn/gttrvwssjt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sufxvd.cn/gtbyulpqaj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xuetiantiany.cn/gtrfeiobgr.html

C#:   using System.Text;
来源：http://hz.jqgufenzy.top/gtbicttbhk.html

[C12] 立即执行函数 IIFE
来源：http://hz.ydzc1.top/gtcqxhecgi.html

Py:   (lambda: print("run"))()
来源：http://hz.jinyuanbaomall.cn/gtkywesxsb.html

PHP:  (function () { echo "run"; })();
来源：http://hz.dianchejie.cn/gtmiyfpnja.html

JS:   (() => { console.log("run"); })();
来源：http://hz.mhx1999.top/gtgumdhruo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangtech.top/gtlrswesvb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.52xcode.cn/gttvygomdg.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jinghuilouyu.cn/gtsxxvzvom.html

Ruby: -> { puts "run" }.call
来源：http://hz.nanxuanxn.top/gtorlaqskj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinyuanbaomall.cn/gttkhhjftn.html

[C13] 类型声明 / 类型注解
来源：http://hz.guowangkeji.top/gtnbyqmojm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gaohongyu789.top/gtzmzdwoya.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.svipenyu.cn/gtnpwhvfav.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinyuanbaomall.cn/gtlseqaenw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnxiangtu.top/gtqkvfodam.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtnxfcfvxi.html

Go:   func add(a, b int) int
来源：http://hz.jiagoushi.top/gtpfeqszgx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cqqwz.cn/gtenczbrwt.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yangfankeji.com/gthclrisom.html

[C14] 泛型函数
来源：http://hz.zdqjudy.top/gtnhpxytby.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cashguo.top/gtbayemxfn.html

PHP:  // 无泛型
来源：http://hz.andypj.xyz/gtkqnteyzc.html

JS:   // 无泛型
来源：http://hz.chenjidiqi.icu/gtuwnpsebs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sufxvd.cn/gtlobcycvb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ybcxt.top/gthanpkyez.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sysykeji.top/gtryegfzrh.html

Ruby: # 无泛型
来源：http://hz.gotoacloud.top/gtculxdwij.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ppjwa.cn/gtwtymnzsw.html

[C15] 解构 / 展开参数
来源：http://hz.birdmap.top/gtbqwkgsnj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.pengpengdd.cyou/gtzcsfvwel.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zycfv.cn/gtzwpkhmqr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.chenzaomai.com/gtprwluiau.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hongshengwenyu.top/gtoqhuawbf.html

Java: // 无解构
来源：http://hz.chenlongwang.top/gtiyabqqle.html

Go:   // 无解构
来源：http://hz.daria6918.cn/gtgqvaghvz.html

Ruby: a, b = pair
来源：http://hz.feifeiyinyue.top/gtefvvjeis.html

C#:   var (a, b) = pair;
来源：http://hz.hysaishi.cn/gtrkowdxbl.html

[C16] 函数 / 方法重载
来源：http://hz.yvedp.cn/gtqfpwaijp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhixingplan.top/gtgvkivevw.html

PHP:  // 无重载
来源：http://hz.andypj.xyz/gtyocynhgq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.pycfn.com/gtbrifrfhw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yuxming.cn/gteavrvulr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zycfv.cn/gtlahjwdqf.html

Go:   // 无重载：用不同函数名
来源：http://hz.ivvv.top/gtuvfwlhqo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yueranfly.top/gtlouycqvh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinghuilouyu.cn/gtqnrjljpd.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtuakmadga.html

D. 数组 / 列表 / 集合
来源：http://hz.jqgfzy.top/gtovkummly.html

================================================================================
来源：http://hz.hammf.cn/gtmfpnartn.html

[D01] 创建数组 / 列表
来源：http://hz.meibo888.top/gtdnqyprel.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cdnleiting.top/gtrexyuzfk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shuidangran.top/gtbnthiufo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.smart0.xyz/gtqpekgoeq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cdnleiting.top/gtecxxsefm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.316326.xyz/gtvthogemv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yangfankeji.com/gttdkffrde.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jiagoushi.top/gtvxwtbtku.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.wangdashe.top/gtlfdpczxk.html

[D02] 追加元素到末尾
来源：http://hz.zhongyouzk.top/gtcrprfoav.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.iojbl.cn/gtkftjhmrn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yj20258888.top/gtqpokyocx.html

JS:   arr.push(4);
来源：http://hz.yuxming.cn/gtxwjddnov.html

TS:   arr.push(4);
来源：http://hz.svipenyu.cn/gtacolrgix.html

Java: list.add(4);
来源：http://hz.yonumen.top/gtxklugyli.html

Go:   arr = append(arr, 4)
来源：http://hz.yangfankeji.com/gtohbxxbyi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shangyingyoupin.top/gtyjzeetsf.html

C#:   list.Add(4);
来源：http://hz.fzhhl.top/gttvkwarwn.html

[D03] 在指定位置插入元素
来源：http://hz.xuetiantiany.cn/gtylemqlwb.html

Py:   arr.insert(0, 0)
来源：http://hz.fengsongda.top/gtrxlqjogq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.quarkkingdee.top/gtmbesbszc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.dianchejie.cn/gtzzbbedtu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.nanxuanxn.top/gtblhsyzrn.html

Java: list.add(0, 0);
来源：http://hz.yangfankeji.com/gtahogrqbh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.iojbl.cn/gtwejgztmg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sweek.top/gtxhmjrbrk.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgfzy.top/gtuwmnlgcz.html

[D04] 删除元素
来源：http://hz.hnxiangtu.top/gtrzjqdeul.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xylfe.cn/gtrqtrnafk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.dashuyun.cn/gtzzcxlljn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nanxinkj.top/gttuqwuerm.html

TS:   arr.splice(0, 1);
来源：http://hz.0kj1m.cn/gtjkoskvdh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.pengpengdd.cyou/gtprnknkff.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sufxvd.cn/gtyytxxaub.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinyuanbaomall.cn/gtmfmknxms.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jyoumei.cn/gtxjqjxrww.html

[D05] 访问与修改元素
来源：http://hz.yj20258888.top/gtrkxqipym.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fzhhl.top/gtgwfxmuvt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zdqjudy.top/gtrehvrzzj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.316326.xyz/gtblmpmcnk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guowangkeji.top/gtlntnbpde.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.bjfxy.top/gtnzltgxrk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gzhubu.top/gtmmoyfciq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangdashe.top/gtoeorzxtf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinqigfzy.top/gtphdmipmd.html

[D06] 数组长度
来源：http://hz.52xcode.cn/gtyhcalihb.html

Py:   len(arr)
来源：http://hz.tian-w.cn/gtgasgubjl.html

PHP:  count($arr);
来源：http://hz.316326.xyz/gtqqbeipun.html

JS:   arr.length
来源：http://hz.bjfxy.top/gtutiqjgeb.html

TS:   arr.length
来源：http://hz.meibo888.top/gtynxbakbw.html

Java: list.size();
来源：http://hz.nwbrower.top/gtltfjiwjo.html

Go:   len(arr)
来源：http://hz.chenlongwang.top/gtkwqaqxoz.html

Ruby: arr.length; arr.size
来源：http://hz.52xcode.cn/gtkulmrtpr.html

C#:   list.Count;
来源：http://hz.9152youxi.cn/gtmhidxqgn.html

[D07] 切片 / 取子数组
来源：http://hz.birdmap.top/gtlsdlwkov.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.guannengcc.top/gtacwvctnb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhaomingkeji.xyz/gtcfgrqort.html

JS:   arr.slice(1, 4);
来源：http://hz.ehwqpu.com/gtzxkywagk.html

TS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangtech.top/gtghglrzrp.html

Java: list.subList(1, 4);
来源：http://hz.0kj1m.cn/gtrybpjaau.html

Go:   arr[1:4]
来源：http://hz.chenlongwang.top/gtcfqkgvuv.html

Ruby: arr[1, 3]
来源：http://hz.sweek.top/gtxxmbgvwg.html

C#:   list.GetRange(1, 3);
来源：http://hz.hongshengwenyu.top/gtwfgrygvz.html

[D08] 合并两个数组
来源：http://hz.ppjwa.cn/gtyfuunydi.html

Py:   a + b;  a.extend(b)
来源：http://hz.xuetiantiany.cn/gttkdcxika.html

PHP:  array_merge($a, $b);
来源：http://hz.ppjwa.cn/gtoxgmrtiv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.kuanghao11.cn/gtuxaqncpr.html

TS:   [...a, ...b];
来源：http://hz.ppjwa.cn/gtnyloksld.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gaohongyu789.top/gtywrhnfyc.html

Go:   append(a, b...)
来源：http://hz.birdmap.top/gtzkpbuesc.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shanyushiyangkeji.top/gtuvenzepp.html

C#:   a.Concat(b).ToList()
来源：http://hz.wangdashe.top/gtlgvchxtx.html

[D09] 排序（升序）
来源：http://hz.havefunace.top/gtizlwmnbp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gtkghpohdi.html

PHP:  sort($arr);
来源：http://hz.zdqjudy.top/gtopbhdzfd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xingfuxueyuan.xyz/gtnxocnyxc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xylfe.cn/gtmbjgavmf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shzxlz.cn/gtrosknnpt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydzc1.top/gtgcfcjbyx.html

Ruby: arr.sort
来源：http://hz.haohaochexian.top/gtmqfxleqb.html

C#:   list.Sort();
来源：http://hz.jlsjyb.cn/gttjdkrfpb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.c1oappe.top/gtnwelqvfl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shangyingyoupin.top/gtdqvhrhqj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.havefunace.top/gtgjchoilg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxuanxn.top/gtahgonroc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.kuanghao11.cn/gtzsdzrplc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.nanxinkj.top/gtwsddvwua.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenzaomai.com/gtyroonobo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shuidangran.top/gtacgnokhr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.birdmap.top/gtmwukksax.html

[D11] 反转数组
来源：http://hz.wangdashe.top/gttwuqbwbz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gzhubu.top/gtducvyfrt.html

PHP:  array_reverse($arr);
来源：http://hz.hongshengwenyu.top/gtsognjjnq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.feifeiyinyue.top/gtztqbtaye.html

TS:   [...arr].reverse();
来源：http://hz.jyoumei.cn/gtqvqiezox.html

Java: Collections.reverse(list);
来源：http://hz.chenlongwang.top/gtqyczdmik.html

Go:   slices.Reverse(arr)
来源：http://hz.tian-w.cn/gtmkbckoxv.html

Ruby: arr.reverse
来源：http://hz.zhixingplan.top/gtcvkrkjco.html

C#:   list.Reverse();
来源：http://hz.chenjidiqi.icu/gtnczmbqbi.html

[D12] 查找元素下标
来源：http://hz.jqgfzy.top/gthlaenowo.html

Py:   arr.index(x);  x in arr
来源：http://hz.zdqjudy.top/gtxqegamog.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.snrcjt.cn/gtagioxgfk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yueranfly.top/gtjpyzyvxe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hywenlv.cn/gtqkkdxhkz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhongyouzk.top/gtjlkcgmai.html

Go:   slices.Index(arr, x)
来源：http://hz.sxryk.cn/gtwrszotvb.html

Ruby: arr.index(x)
来源：http://hz.zhixingplan.top/gtqmrnashj.html

C#:   list.IndexOf(x);
来源：http://hz.cucudq.cn/gtpyecknfo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jiagoushi.top/gtssodphpx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yonumen.top/gtyyfrkzbl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jlsjyb.cn/gthfzdjbch.html

JS:   arr.filter(x => x > 3)
来源：http://hz.snrcjt.cn/gtsygqslvo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.aibaodan.cn/gtlfgodoep.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.guannengcc.top/gtexeasobw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.sweek.top/gtcbfeplql.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.fzhhl.top/gtyzxklrcs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xziqi.cn/gtvbnkwdwc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj20258.top/gtodmnjzpn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.daxiang520.top/gtsructhhm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.guowangkeji.top/gtplhlqedx.html

JS:   arr.map(x => x * 2)
来源：http://hz.tianlin.xyz/gtyfdjmekq.html

TS:   arr.map(x => x * 2)
来源：http://hz.chenjidiqi.icu/gtzukraalk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenjidiqi.icu/gtclccnldj.html

Go:   // 手写循环
来源：http://hz.daxiang520.top/gtorovcieb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.aizwys.cn/gtqvuqtmjp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinghuilouyu.cn/gtxzulrqje.html

[D15] 去重
来源：http://hz.yuxming.cn/gtnozpoiqr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nanxuanxn.top/gtjanukefg.html

PHP:  array_unique($arr);
来源：http://hz.hammf.cn/gtadlshkyb.html

JS:   [...new Set(arr)]
来源：http://hz.yvedp.cn/gtczvoboqb.html

TS:   [...new Set(arr)]
来源：http://hz.cqqwz.cn/gtifqolekb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.daxiang520.top/gtlswejyqx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258.top/gtnrgskoyr.html

Ruby: arr.uniq
来源：http://hz.yonumen.top/gtmyyywhng.html

C#:   list.Distinct().ToList()
来源：http://hz.cqqwz.cn/gtcyxoetig.html

[D16] 求和与平均值
来源：http://hz.ywan-chungtsiang.top/gtyrikrsfe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.tian-w.cn/gtglobwnnm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yanxiufei.cn/gtblhbsgiy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ywan-chungtsiang.top/gtadsjmngb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuanzhike.top/gtwyydeojt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.dianchejie.cn/gtyptkxjup.html

Go:   // 手写循环累加
来源：http://hz.mhx1999.top/gtgvajtwfs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.0kj1m.cn/gtyqmlxkcp.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhoulong.xyz/gtyuozeonw.html

[D17] 最大值与最小值
来源：http://hz.zdqjudy.top/gtzvagiabi.html

Py:   max(arr);  min(arr)
来源：http://hz.zhongyouzk.top/gtuqweusfv.html

PHP:  max($arr);  min($arr);
来源：http://hz.hongshengwenyu.top/gtynsrhewz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jinqigfzy.top/gtfuawcfpl.html

TS:   Math.max(...arr);
来源：http://hz.316326.xyz/gtzdlcphsx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.dashuyun.cn/gtcmpaemti.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.pycfn.com/gtbwqxiewz.html

Ruby: arr.max;  arr.min
来源：http://hz.shzxlz.cn/gtnehcvxzz.html

C#:   list.Max();  list.Min()
来源：http://hz.hnxiangtu.top/gtfmwabzxy.html

[D18] 扁平化嵌套数组
来源：http://hz.jqgfzy.top/gthziqhyxc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxinkj.top/gtbricwboi.html

PHP:  array_merge(...$nested);
来源：http://hz.cqqwz.cn/gtmeexhrhr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xuanzx.com/gtvtengbtp.html

TS:   nested.flat();
来源：http://hz.wangshuangyany.cn/gtzfnebexd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.pycfn.com/gtibcbucxr.html

Go:   // 手写双层循环
来源：http://hz.cashguo.top/gtotjkxtcg.html

Ruby: nested.flatten
来源：http://hz.feifeiyinyue.top/gtwlklnyss.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.quarkkingdee.top/gtjnydxpfd.html

[D19] 按字段分组
来源：http://hz.yj20258888.top/gttzvcrbcj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.kuanghao11.cn/gtmsmzthpf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.aibaodan.cn/gtqerejtej.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhaomingkeji.xyz/gtzoedbphb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xingfuxueyuan.xyz/gtxbdhotyy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj202588.top/gtvovuxkta.html

Go:   // 手写 map[string][]T
来源：http://hz.zhoulong.xyz/gthmccdcvu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daxiang520.top/gtbjxzukuh.html


<!-- 参考信息 -->