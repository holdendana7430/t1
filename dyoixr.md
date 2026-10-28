代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://hz.yuxming.cn/gtilokefbu.html

[C03] 可变参数
来源：http://hz.vqdsnc.cn/gtwumgqwif.html

Py:   def total(*args): return sum(args)
来源：http://hz.haohaochexian.top/gtodmkedwo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.pengpengdd.cyou/gtrtxsrode.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgfzy.top/gtrifterja.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sxryk.cn/gtutsdxjsz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jianghu66.top/gtbvprfesb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.daxiang520.top/gtayiulite.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.52xcode.cn/gtfmlabyud.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hammf.cn/gtbkamueaf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.iojbl.cn/gthtfznlwl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jiagoushi.top/gtbfollgzf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zdqjudy.top/gtbhaarseq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.birdmap.top/gtigcuumtt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenjidiqi.icu/gtiapdvzyi.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.0kj1m.cn/gtikchdnkh.html

Go:   // 无：用配置结构体参数
来源：http://hz.gzhubu.top/gtubsraywb.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cdnleiting.top/gtywpdkcst.html

C#:   f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtpnxgdpis.html

[C05] 返回多个值
来源：http://hz.redwolf501.top/gtawczangy.html

Py:   return a, b
来源：http://hz.52xcode.cn/gtqqxwxnqo.html

PHP:  return [$a, $b];
来源：http://hz.haohaochexian.top/gtweoupaoj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.redwolf501.top/gtmyewdlag.html

TS:   return { a, b };
来源：http://hz.daria6918.cn/gtgebevjap.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zycfv.cn/gtvuumjvbp.html

Go:   return a, b
来源：http://hz.ydzc1.top/gtppeiexxe.html

Ruby: return a, b
来源：http://hz.sweek.top/gtabvftwri.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cucudq.cn/gtkulmckla.html

[C06] 匿名函数 / lambda
来源：http://hz.hywenlv.cn/gthjruhnwl.html

Py:   square = lambda x: x * x
来源：http://hz.daria6918.cn/gtqdtplwyb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hfpthk.cn/gtgsdouwqo.html

JS:   const square = x => x * x;
来源：http://hz.pengpengdd.cyou/gtwvgoiaee.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.snrcjt.cn/gtxieyvfxw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinqigfzy.top/gtekkfhzhb.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.wangdashe.top/gtgbynueqm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.0kj1m.cn/gtnjpeveul.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xziqi.cn/gthzdyqfqp.html

[C07] 把函数作为参数传入
来源：http://hz.hongshengwenyu.top/gtbvjexpew.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinghuilouyu.cn/gthwsyuxno.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xinyue.icu/gtcuqjtlnd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhixingplan.top/gtkrayiofk.html

TS:   arr.map(String)
来源：http://hz.cucudq.cn/gtoppmcqod.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.0kj1m.cn/gtvqnqurvl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangkeji.top/gtuobqlkml.html

Ruby: arr.map(&:upcase)
来源：http://hz.dashuyun.cn/gtyrbruvsx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.mhx1999.top/gthosdscfs.html

[C08] 闭包
来源：http://hz.mhx1999.top/gtwvzdikiz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hnqzz.top/gthaobrulk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinghuilouyu.cn/gtjgvsbblj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ppjwa.cn/gtbjahwigg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.aizwys.cn/gtubowdfvr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xuanzx.com/gtobvjgmdo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhijiandao.cn/gtcdwskkun.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hfpthk.cn/gtpdrbcdln.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xinyue.icu/gtipznquub.html

[C09] 递归
来源：http://hz.cashguo.top/gtjqccohyb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.52xcode.cn/gtpaczzaki.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.kuanghao11.cn/gtjwfxoloy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nwbrower.top/gtnpgkjixn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.snrcjt.cn/gtydsrhxnl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jqgufenzy.top/gtuhisjfir.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.havefunace.top/gtwjqzoyjm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.meibo888.top/gtpoqtxxmq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.aibaodan.cn/gtwpjxtdya.html

[C10] 变量作用域
来源：http://hz.cheryme.top/gtjpxiweqj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cdnleiting.top/gtlydjhirh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.dianchejie.cn/gtkcpvehsv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gzhubu.top/gtlcbwqgbr.html

TS:   同 JS
来源：http://hz.cashguo.top/gtlvbzsctg.html

Java: 方法内为块级作用域
来源：http://hz.xziqi.cn/gthkfocrqy.html

Go:   花括号块级作用域
来源：http://hz.gzhubu.top/gtkjbrrutv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinghuilouyu.cn/gtkhztfqgo.html

C#:   块级作用域
来源：http://hz.shangyingyoupin.top/gtxcikyurw.html

[C11] 模块导入与导出
来源：http://hz.zhiwuduotai.top/gtikudczdp.html

Py:   from module import func
来源：http://hz.yvedp.cn/gtzssqrmwv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cheryme.top/gtcffwibit.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhijiandao.cn/gtdrksbucu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.smart0.xyz/gtsugceyhd.html

Java: import java.util.List;
来源：http://hz.52xcode.cn/gtiypvxrcc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinyuanbaomall.cn/gtupcpwbfs.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sxryk.cn/gtylbolnub.html

C#:   using System.Text;
来源：http://hz.feifeiyinyue.top/gtlrsbldzo.html

[C12] 立即执行函数 IIFE
来源：http://hz.shzxlz.cn/gtqyiyyrbx.html

Py:   (lambda: print("run"))()
来源：http://hz.bjfxy.top/gtuofihqxv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yangfankeji.com/gthvflsvlx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.gzhubu.top/gtsrdvzqve.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sysykeji.top/gtbuwgcydw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xinyue.icu/gtavtxfwby.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.guannengcc.top/gtwittvrmv.html

Ruby: -> { puts "run" }.call
来源：http://hz.316326.xyz/gtiuvbqrmg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.fzhhl.top/gtvjbqnwns.html

[C13] 类型声明 / 类型注解
来源：http://hz.jinyuanbaomall.cn/gthpvgemcl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhaomingkeji.xyz/gtbylrlvrx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.c1oappe.top/gtqwluvrkl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.9152youxi.cn/gtqoyxguxo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.smart0.xyz/gtdpzjsnia.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gttchfsphi.html

Go:   func add(a, b int) int
来源：http://hz.yj20258888.top/gtmoidwurp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hysaishi.cn/gtqnrjcbqu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ywan-chungtsiang.top/gtwizexlfa.html

[C14] 泛型函数
来源：http://hz.gaohongyu789.top/gtpzhcztsy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hnqzz.top/gtdkyedook.html

PHP:  // 无泛型
来源：http://hz.bjfxy.top/gtwxkcarji.html

JS:   // 无泛型
来源：http://hz.nwbrower.top/gturxtaddp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jqgufenzy.top/gtspdsvnvo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.daria6918.cn/gtnscnfsjy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sufxvd.cn/gtenspmmgz.html

Ruby: # 无泛型
来源：http://hz.zhijiandao.cn/gtrtbbcogi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.c1oappe.top/gtsmxtefjp.html

[C15] 解构 / 展开参数
来源：http://hz.yuanzhike.top/gtumhwkkcu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinqigufen.top/gttmomatpt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.pycfn.com/gtklkukvfy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinghuilouyu.cn/gtawvvcrlp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.sufxvd.cn/gtscqgsiiz.html

Java: // 无解构
来源：http://hz.kuanghao11.cn/gtkoiadhec.html

Go:   // 无解构
来源：http://hz.shanyushiyangkeji.top/gtisbkzcne.html

Ruby: a, b = pair
来源：http://hz.haohaochexian.top/gtrpnxjyld.html

C#:   var (a, b) = pair;
来源：http://hz.jinyuanbaomall.cn/gtlfbnguvv.html

[C16] 函数 / 方法重载
来源：http://hz.cheryme.top/gtogedkhdc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.quarkkingdee.top/gtrmhaivkv.html

PHP:  // 无重载
来源：http://hz.shzxlz.cn/gtsomkzbdv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gzhubu.top/gtoiawuafr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jlsjyb.cn/gtbbwxlcwk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xinyue.icu/gtiixnnrbx.html

Go:   // 无重载：用不同函数名
来源：http://hz.nanxuanxn.top/gtwnkcpttz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.iojbl.cn/gtxospomrc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yuanzhike.top/gthezalhvz.html

================================================================================
来源：http://hz.0kj1m.cn/gtkyckkbcr.html

D. 数组 / 列表 / 集合
来源：http://hz.shuidangran.top/gtmfiwwewq.html

================================================================================
来源：http://hz.316326.xyz/gtsozgaawn.html

[D01] 创建数组 / 列表
来源：http://hz.pengpengdd.cyou/gtxqhgxdfk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jianghu66.top/gtvqdesfds.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jyoumei.cn/gtrrlrllkj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sweek.top/gtcwzcrkdp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ywan-chungtsiang.top/gtequarsfr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yongpay.top/gtxmrwrabr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinyuanbaomall.cn/gtmarzxzzb.html

Ruby: arr = [1, 2, 3]
来源：http://hz.dashuyun.cn/gtoykgvrbc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.pycfn.com/gtrxpvfvuz.html

[D02] 追加元素到末尾
来源：http://hz.yonumen.top/gtfiehfaro.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.andypj.xyz/gtawocdxcj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.316326.xyz/gtnnftuonq.html

JS:   arr.push(4);
来源：http://hz.andypj.xyz/gtwdlmjhqp.html

TS:   arr.push(4);
来源：http://hz.hywenlv.cn/gtrmiayqrw.html

Java: list.add(4);
来源：http://hz.hysaishi.cn/gtnmbjjhee.html

Go:   arr = append(arr, 4)
来源：http://hz.jinqigufen.top/gtrhzcqlet.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinqigufen.top/gtdeuqlcet.html

C#:   list.Add(4);
来源：http://hz.feifeiyinyue.top/gtjdctamyg.html

[D03] 在指定位置插入元素
来源：http://hz.xuetiantiany.cn/gtxkrsycfc.html

Py:   arr.insert(0, 0)
来源：http://hz.redwolf501.top/gtvxqiqvph.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.svipenyu.cn/gtoqweqfzf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jlsjyb.cn/gtkweahmry.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhaomingkeji.xyz/gtbgnzznbr.html

Java: list.add(0, 0);
来源：http://hz.havefunace.top/gtjkimuxwk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenlongwang.top/gtfotavoxu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.smart0.xyz/gtblhxyfzt.html

C#:   list.Insert(0, 0);
来源：http://hz.gaohongyu789.top/gtzwfptkov.html

[D04] 删除元素
来源：http://hz.guannengcc.top/gtafivbzma.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.bjfxy.top/gttrdmlprc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.birdmap.top/gtciwhmbhx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jiagoushi.top/gtbajfvcsm.html

TS:   arr.splice(0, 1);
来源：http://hz.havefunace.top/gttrefewin.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cdnleiting.top/gtvyrmmnoe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hammf.cn/gtiqpxiadb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gogol.net.cn/gtzhfzmjqh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shanyushiyangkeji.top/gtneolobhp.html

[D05] 访问与修改元素
来源：http://hz.shanyushiyangkeji.top/gtgjnnvdnn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tanke756.top/gtstnrphem.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hfpthk.cn/gtrmftxkyd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hnqzz.top/gtmluhhmxn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.vqdsnc.cn/gteslxpjjo.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.kuanghao11.cn/gttyppzcdp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.fzhhl.top/gtersbeeqa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daria6918.cn/gtgxymejen.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nwbrower.top/gtxbxfmnuz.html

[D06] 数组长度
来源：http://hz.shanyushiyangkeji.top/gtzwoiafmm.html

Py:   len(arr)
来源：http://hz.aibaodan.cn/gtwedzmbvc.html

PHP:  count($arr);
来源：http://hz.sysykeji.top/gtxfvazpwl.html

JS:   arr.length
来源：http://hz.havefunace.top/gtzbdyikbe.html

TS:   arr.length
来源：http://hz.fzhhl.top/gtuazuqgba.html

Java: list.size();
来源：http://hz.ydzc1.top/gtsjuibkir.html

Go:   len(arr)
来源：http://hz.hammf.cn/gtyryeemwp.html

Ruby: arr.length; arr.size
来源：http://hz.redwolf501.top/gtbciuktlf.html

C#:   list.Count;
来源：http://hz.guowangkeji.top/gtpjfhfwvq.html

[D07] 切片 / 取子数组
来源：http://hz.tanke756.top/gtwsxbtwyb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sweek.top/gtixzqljwc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xuetiantiany.cn/gtenmrbsfa.html

JS:   arr.slice(1, 4);
来源：http://hz.jinqigfzy.top/gtylszbosk.html

TS:   arr.slice(1, 4);
来源：http://hz.sweek.top/gtyohgkdoq.html

Java: list.subList(1, 4);
来源：http://hz.zhijiandao.cn/gtnckpszrh.html

Go:   arr[1:4]
来源：http://hz.feifeiyinyue.top/gtxxruirek.html

Ruby: arr[1, 3]
来源：http://hz.gogol.net.cn/gteshqqglj.html

C#:   list.GetRange(1, 3);
来源：http://hz.vqdsnc.cn/gtyniainsl.html

[D08] 合并两个数组
来源：http://hz.sweek.top/gtqpisoadt.html

Py:   a + b;  a.extend(b)
来源：http://hz.xziqi.cn/gtlkzqwueo.html

PHP:  array_merge($a, $b);
来源：http://hz.chenlongwang.top/gtfzcrwprs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinyuanbaomall.cn/gtnoqcphrd.html

TS:   [...a, ...b];
来源：http://hz.zhongyouzk.top/gtytacdgnf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinqigfzy.top/gtcnabawqb.html

Go:   append(a, b...)
来源：http://hz.chenlongwang.top/gtrkofgvvt.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yonumen.top/gtcqrhcman.html

C#:   a.Concat(b).ToList()
来源：http://hz.havefunace.top/gtrexyjigv.html

[D09] 排序（升序）
来源：http://hz.yangfankeji.com/gtfybwnpsn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ybcxt.top/gtjmohkyvr.html

PHP:  sort($arr);
来源：http://hz.shangyingyoupin.top/gtojxqfili.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yongpay.top/gtjrarnpir.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xuetiantiany.cn/gtmjaenezl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenzaomai.com/gtlyzildio.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj202588.top/gtytmymtzd.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtswcqfapm.html

C#:   list.Sort();
来源：http://hz.ehwqpu.com/gtuuotlzmy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hysaishi.cn/gtyshkrewg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hnqzz.top/gtpoqufrqs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.9152youxi.cn/gtvkrjtbwe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.316326.xyz/gtmogqprjf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnqzz.top/gtwyzojszt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yueranfly.top/gtyuiutifd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.meibo888.top/gtpgcpwkzr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.sysykeji.top/gtpjemccrh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.svipenyu.cn/gtklzxiaob.html

[D11] 反转数组
来源：http://hz.hnxiangtu.top/gtzrdfxkkm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ehwqpu.com/gtrhaxtvzf.html

PHP:  array_reverse($arr);
来源：http://hz.feifeiyinyue.top/gtjvctcsfw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tanke756.top/gtgtyaopmb.html

TS:   [...arr].reverse();
来源：http://hz.yvedp.cn/gtjfdfpdnz.html

Java: Collections.reverse(list);
来源：http://hz.zycfv.cn/gtnspmzmaw.html

Go:   slices.Reverse(arr)
来源：http://hz.hysaishi.cn/gtqwkfvfzv.html

Ruby: arr.reverse
来源：http://hz.cqqwz.cn/gtehhkkspt.html

C#:   list.Reverse();
来源：http://hz.birdmap.top/gtvcwsczat.html

[D12] 查找元素下标
来源：http://hz.redwolf501.top/gtbjsgplma.html

Py:   arr.index(x);  x in arr
来源：http://hz.hongshengwenyu.top/gtygwsinro.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.wangshuangyany.cn/gtrphcwfcp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinghuilouyu.cn/gtqmuxshqk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gtrbffzzof.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gotoacloud.top/gtmcvazipk.html

Go:   slices.Index(arr, x)
来源：http://hz.c1oappe.top/gtaczyprkq.html

Ruby: arr.index(x)
来源：http://hz.ivvv.top/gtyvdllglg.html

C#:   list.IndexOf(x);
来源：http://hz.birdmap.top/gtbeovexom.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenlongwang.top/gtqowxiekr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nwbrower.top/gtovkanoag.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xylfe.cn/gtcdkxsbzp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jlsjyb.cn/gtfaaqmvly.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ivvv.top/gtzpgvrxjl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sysykeji.top/gtlezegmfw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.bjfxy.top/gtotcdgeju.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ivvv.top/gtgoosdksf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hnqzz.top/gtmwmpoiwd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhoulong.xyz/gtnvbsgmfh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yuanzhike.top/gtwcvqtvrx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yj20258.top/gtdianbckb.html

JS:   arr.map(x => x * 2)
来源：http://hz.yanxiufei.cn/gtposznbci.html

TS:   arr.map(x => x * 2)
来源：http://hz.shuidangran.top/gtgylghscv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.dianchejie.cn/gtzcpirhvb.html

Go:   // 手写循环
来源：http://hz.shzxlz.cn/gtgcfupqqt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhengqikj.top/gtspugltfo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dashuyun.cn/gttijrkoec.html

[D15] 去重
来源：http://hz.yanxiufei.cn/gtplmcteab.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gtccjxtyvl.html

PHP:  array_unique($arr);
来源：http://hz.redwolf501.top/gtceyfgdrj.html

JS:   [...new Set(arr)]
来源：http://hz.xinyue.icu/gtodbolvhm.html

TS:   [...new Set(arr)]
来源：http://hz.yj20258.top/gtwrhfbqvc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258888.top/gtfynohtik.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.dianchejie.cn/gtkwaxkukl.html

Ruby: arr.uniq
来源：http://hz.ydzc1.top/gtafnscqfa.html

C#:   list.Distinct().ToList()
来源：http://hz.52xcode.cn/gtpicgvbeb.html

[D16] 求和与平均值
来源：http://hz.yj20258.top/gtfwuhhidz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shangyingyoupin.top/gtfsewhuvu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shangyingyoupin.top/gtumzjxbfc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xziqi.cn/gtexibfcvf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tianlin.xyz/gtddhebeee.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jqgufenzy.top/gtmkcjuoes.html

Go:   // 手写循环累加
来源：http://hz.sxryk.cn/gtrieclivp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj202588.top/gtjlvoukjt.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhengqikj.top/gthuzbxmva.html

[D17] 最大值与最小值
来源：http://hz.jiagoushi.top/gtzofzcihe.html

Py:   max(arr);  min(arr)
来源：http://hz.yangfankeji.com/gtolodxaup.html

PHP:  max($arr);  min($arr);
来源：http://hz.316326.xyz/gtbpzvugpb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.0kj1m.cn/gtichykrei.html

TS:   Math.max(...arr);
来源：http://hz.9152youxi.cn/gtqvduqeef.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.guannengcc.top/gtalxwpbdz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hysaishi.cn/gttrruoycb.html

Ruby: arr.max;  arr.min
来源：http://hz.sysykeji.top/gtvbilxzab.html

C#:   list.Max();  list.Min()
来源：http://hz.guowangkeji.top/gtpucrileb.html

[D18] 扁平化嵌套数组
来源：http://hz.sxryk.cn/gtlffzlodk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ivvv.top/gtlayjfhdj.html

PHP:  array_merge(...$nested);
来源：http://hz.zhaomingkeji.xyz/gtcokcsuvq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hfpthk.cn/gtndavvbrn.html

TS:   nested.flat();
来源：http://hz.haohaochexian.top/gtxapwrsuo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhongyouzk.top/gtldlbsmze.html

Go:   // 手写双层循环
来源：http://hz.shanyushiyangtech.top/gtiijqggha.html

Ruby: nested.flatten
来源：http://hz.zhaomingkeji.xyz/gtzfxzvqkl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hfpthk.cn/gttotwpnbg.html

[D19] 按字段分组
来源：http://hz.ehwqpu.com/gtitcsfvze.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yonumen.top/gtpfrmkemt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hywenlv.cn/gtkjcvsows.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cdnleiting.top/gtszovaaev.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhiwuduotai.top/gtezgtitmw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xziqi.cn/gthnofgjab.html

Go:   // 手写 map[string][]T
来源：http://hz.zdqjudy.top/gtucmiowbb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.birdmap.top/gtydfjnbwy.html


<!-- 参考信息 -->