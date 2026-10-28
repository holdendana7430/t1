代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://hz.fzhhl.top/gtjyyapbah.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.xziqi.cn/gtjhxhwwti.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ywan-chungtsiang.top/gtfmzvkorz.html

C#:   do { i++; } while (i < 10);
来源：http://hz.xuanzx.com/gtijlsmxwj.html

[B09] break 与 continue
来源：http://hz.andypj.xyz/gtyzhdfleg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.cucudq.cn/gtbsqlevpw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ppjwa.cn/gtbhpbojhy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hammf.cn/gtcuafbcjl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.meibo888.top/gteizhcraj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.andypj.xyz/gtnmiaejec.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hnqzz.top/gtprlzbizz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yongpay.top/gtcpsvbxsi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtpqoknipl.html

[B10] 遍历同时拿索引
来源：http://hz.shzxlz.cn/gtytczogln.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jlsjyb.cn/gtvrdjojxj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.redwolf501.top/gtibnszwtn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yuanzhike.top/gtixctvdue.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ehwqpu.com/gtfhazbmbe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.havefunace.top/gtxtdylhlj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhaomingkeji.xyz/gtzjvwgucw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.chenjidiqi.icu/gtwuiypunh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ydjk.org.cn/gtwsvvcnzs.html

[B11] 生成数字序列 / 区间
来源：http://hz.zhixingplan.top/gtghnsooyc.html

Py:   list(range(0, 10, 2))
来源：http://hz.9152youxi.cn/gtfredaxzm.html

PHP:  range(0, 10, 2);
来源：http://hz.cqqwz.cn/gtealbavxh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.havefunace.top/gtxaqokmdc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jyoumei.cn/gtaqabzkjo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.wangshuangyany.cn/gtkzkfntuh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yanxiufei.cn/gtjmzgwilr.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xziqi.cn/gtllnmpgmt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhixingplan.top/gtasfqgulb.html

[B12] 跳出多层循环
来源：http://hz.yj202588.top/gtxlbgcuku.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.meibo888.top/gtmfwtdlyw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ywan-chungtsiang.top/gtisvhddfy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.redwolf501.top/gtgleqrndu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhoulong.xyz/gtbqcsudje.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.daria6918.cn/gtxprzvxzv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.pengpengdd.cyou/gtjkyuukvb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shzxlz.cn/gtupnmmxrn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shzxlz.cn/gtdlghmicd.html

[B13] 判断是否为数字
来源：http://hz.pycfn.com/gthbnidaox.html

Py:   isinstance(x, (int, float))
来源：http://hz.fzhhl.top/gtyydvespd.html

PHP:  is_numeric($x)
来源：http://hz.smart0.xyz/gtxwprtmen.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jlsjyb.cn/gtrbmgejci.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.haohaochexian.top/gtxsjkrdhy.html

Java: x instanceof Number
来源：http://hz.smart0.xyz/gtksbewcjb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.shuidangran.top/gtjwfbfibr.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ivvv.top/gtcvmluupb.html

C#:   x is int or double or decimal
来源：http://hz.tanke756.top/gtuvcjtcrp.html

[B14] 判断值是否在集合内
来源：http://hz.hywenlv.cn/gtrbprbpoh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jqgfzy.top/gtoqtbiroz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.aibaodan.cn/gtsrfrpfbp.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.pycfn.com/gtwijefupu.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xinyue.icu/gtmfzsbkrw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jqgufenzy.top/gtxcvtwwsr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xylfe.cn/gtnrvalkgn.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cashguo.top/gtwxnaaiqp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhixingplan.top/gtolnolkmh.html

[B15] 布尔运算与取反
来源：http://hz.jinyuanbaomall.cn/gtluwkexqx.html

Py:   a and b or not c
来源：http://hz.dashuyun.cn/gtdcqzsxrr.html

PHP:  $a && $b || !$c
来源：http://hz.tian-w.cn/gtkrhkrazo.html

JS:   a && b || !c
来源：http://hz.hywenlv.cn/gtvibhxvqt.html

TS:   a && b || !c
来源：http://hz.sysykeji.top/gtyvfqpbgk.html

Java: a && b || !c
来源：http://hz.havefunace.top/gtmzfmvrda.html

Go:   a && b || !c
来源：http://hz.gzhubu.top/gtiuhabecs.html

Ruby: a && b || !c
来源：http://hz.shanyushiyangtech.top/gtodeopwue.html

C#:   a && b || !c
来源：http://hz.dianchejie.cn/gtmqplljzg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yj20258.top/gtdqslxbgf.html

Py:   if not data: return
来源：http://hz.shzxlz.cn/gtinhwbzza.html

PHP:  if (!$data) { return; }
来源：http://hz.shzxlz.cn/gthjbezply.html

JS:   if (!data) return;
来源：http://hz.ehwqpu.com/gtdidfjbdy.html

TS:   if (!data) return;
来源：http://hz.xingfuxueyuan.xyz/gtnjxjritl.html

Java: if (data == null) return;
来源：http://hz.cashguo.top/gtnskktoxe.html

Go:   if data == nil { return }
来源：http://hz.yj20258888.top/gtlthnbelx.html

Ruby: return if data.nil?
来源：http://hz.pengpengdd.cyou/gtryyswync.html

C#:   if (data == null) return;
来源：http://hz.zhixingplan.top/gtidqdjdnl.html

================================================================================
来源：http://hz.ivvv.top/gtcsznhefm.html

C. 函数与作用域
来源：http://hz.hysaishi.cn/gtdrggcdce.html

================================================================================
来源：http://hz.aizwys.cn/gtkouafhgp.html

[C01] 定义函数
来源：http://hz.yangfankeji.com/gtbmrotwij.html

Py:   def add(a, b): return a + b
来源：http://hz.jqgfzy.top/gtzgithsec.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shuidangran.top/gtlgblajlt.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.daxiang520.top/gtyqqdnjtu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hongshengwenyu.top/gtzhffcmul.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ybcxt.top/gtpmrgbilg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.chenzaomai.com/gtjzegqudz.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhaomingkeji.xyz/gtkufvjdfo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtsefdhptf.html

[C02] 默认参数
来源：http://hz.cqqwz.cn/gtgueozjdl.html

Py:   def greet(name="World"): return name
来源：http://hz.yj20258.top/gttlnywuni.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.316326.xyz/gtambssncg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hfpthk.cn/gtdxgwwywh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.pengpengdd.cyou/gtgdprxabf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yanxiufei.cn/gtukxtjqdv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cqqwz.cn/gtbtexgxlm.html

Ruby: def greet(name = "World") = name
来源：http://hz.tian-w.cn/gtalyzoorx.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.sweek.top/gtkqfjnfvv.html

[C03] 可变参数
来源：http://hz.jinqigfzy.top/gtjiwrtfph.html

Py:   def total(*args): return sum(args)
来源：http://hz.yvedp.cn/gtrabwdryn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hysaishi.cn/gtnlgwluyt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.vqdsnc.cn/gtrdlvdxkf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.9152youxi.cn/gtitksrwpp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.dashuyun.cn/gtapbcvqxt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinyuanbaomall.cn/gtpvcjnzun.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nanxinkj.top/gtijmyzzey.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.iojbl.cn/gtefmccyuq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cqqwz.cn/gtjhypocdt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.fengsongda.top/gtrzgdswuo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shanyushiyangkeji.top/gtrndichll.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yongpay.top/gtedzhslwk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.vqdsnc.cn/gtabtlsozb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.316326.xyz/gtgfycvxnz.html

Go:   // 无：用配置结构体参数
来源：http://hz.chenjidiqi.icu/gtpxhohalz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gtdnyebdcp.html

C#:   f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtzyedvjdg.html

[C05] 返回多个值
来源：http://hz.zhoulong.xyz/gtvluiaogj.html

Py:   return a, b
来源：http://hz.chenzaomai.com/gtuawdixsg.html

PHP:  return [$a, $b];
来源：http://hz.pengpengdd.cyou/gtoifverud.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ywan-chungtsiang.top/gtwydczfea.html

TS:   return { a, b };
来源：http://hz.jinqigfzy.top/gtpxsosjvt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhiwuduotai.top/gtorsukybq.html

Go:   return a, b
来源：http://hz.ivvv.top/gtvcmypytn.html

Ruby: return a, b
来源：http://hz.chenjidiqi.icu/gtnwhokqxf.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.birdmap.top/gtqmvdwdxb.html

[C06] 匿名函数 / lambda
来源：http://hz.jinyuanbaomall.cn/gtbxzhiepg.html

Py:   square = lambda x: x * x
来源：http://hz.ybcxt.top/gtbtahirim.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.aizwys.cn/gtgdkztatu.html

JS:   const square = x => x * x;
来源：http://hz.ppjwa.cn/gtgqzjbfbg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yuxming.cn/gtijwqrgde.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhengqikj.top/gtcywcdafe.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ywan-chungtsiang.top/gtekcghnnu.html

Ruby: square = ->(x) { x * x }
来源：http://hz.birdmap.top/gtpxzticqu.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hysaishi.cn/gtydoqnwyu.html

[C07] 把函数作为参数传入
来源：http://hz.sufxvd.cn/gtmmjwomod.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cashguo.top/gtvvdpkrcz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hysaishi.cn/gtszoggwks.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jqgufenzy.top/gthdgqkmyf.html

TS:   arr.map(String)
来源：http://hz.xingfuxueyuan.xyz/gtcrliegjf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.vqdsnc.cn/gtasymqljd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.9152youxi.cn/gtjuttbbox.html

Ruby: arr.map(&:upcase)
来源：http://hz.bjfxy.top/gtmnuxngbh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shuidangran.top/gtbgleejrg.html

[C08] 闭包
来源：http://hz.xuetiantiany.cn/gtwipznfob.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ydzc1.top/gtdteggivz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cqqwz.cn/gtppuvavdj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.meibo888.top/gtyhevsjrf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ivvv.top/gtsoewxgrl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinqigfzy.top/gtnbrxmdub.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sweek.top/gtwyhvlsci.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shangyingyoupin.top/gtvzbyilpu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gtrqdtycwf.html

[C09] 递归
来源：http://hz.yvedp.cn/gtqthgdgon.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinghuilouyu.cn/gtwamhalps.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cheryme.top/gtetdseszn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.snrcjt.cn/gtfswwgmhb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhijiandao.cn/gtqiybhilx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.havefunace.top/gtdzehdenx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.nwbrower.top/gtqwbmjgel.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xingfuxueyuan.xyz/gtqojrucjn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenlongwang.top/gtpgbnhqjk.html

[C10] 变量作用域
来源：http://hz.nanxinkj.top/gtxtfcpyqt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.9152youxi.cn/gtvyymngdc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jyoumei.cn/gtkbqnsufd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ydzc1.top/gtadxedzlq.html

TS:   同 JS
来源：http://hz.yanxiufei.cn/gthkrzwnag.html

Java: 方法内为块级作用域
来源：http://hz.wangshuangyany.cn/gttofgsiti.html

Go:   花括号块级作用域
来源：http://hz.shanyushiyangtech.top/gtwysbtjiu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nanxinkj.top/gtwasqanvx.html

C#:   块级作用域
来源：http://hz.jinyuanbaomall.cn/gtmuqfrjbd.html

[C11] 模块导入与导出
来源：http://hz.yj20258888.top/gtkdxbdupl.html

Py:   from module import func
来源：http://hz.hnxiangtu.top/gtskjeqgay.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.dashuyun.cn/gtmyodlvnm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hnqzz.top/gtcsnfrtug.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj20258888.top/gtpdoeahyj.html

Java: import java.util.List;
来源：http://hz.jinghuilouyu.cn/gtvjhehmoi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shzxlz.cn/gtcwikfnes.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hfpthk.cn/gtuuxkbrmu.html

C#:   using System.Text;
来源：http://hz.cheryme.top/gtpysfeebg.html

[C12] 立即执行函数 IIFE
来源：http://hz.cucudq.cn/gtbamybzmt.html

Py:   (lambda: print("run"))()
来源：http://hz.yueranfly.top/gtrbcxalbi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.guannengcc.top/gtttwpgovw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sxryk.cn/gtnvlecldr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinghuilouyu.cn/gtdiccqpcf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ybcxt.top/gtslubhnhb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shangyingyoupin.top/gtfmndrqxd.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhaomingkeji.xyz/gtidmkaaer.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.316326.xyz/gtobfrexds.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj20258.top/gtvxmfguwr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sysykeji.top/gttvozmhux.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuanzx.com/gtrnljbjoj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yj20258.top/gtoqjiowri.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtxutrjosi.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhengqikj.top/gtpcgqnscv.html

Go:   func add(a, b int) int
来源：http://hz.cashguo.top/gtmhfgpkhs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.aizwys.cn/gthqucybia.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinghuilouyu.cn/gttsvhhojx.html

[C14] 泛型函数
来源：http://hz.sysykeji.top/gtokmfvtho.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.aibaodan.cn/gtjhotaair.html

PHP:  // 无泛型
来源：http://hz.hysaishi.cn/gtpvinzenh.html

JS:   // 无泛型
来源：http://hz.mhx1999.top/gtqaqmdtfw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.smart0.xyz/gtyjyahkgj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shuidangran.top/gtkizwvzhe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.vqdsnc.cn/gtcwwkifka.html

Ruby: # 无泛型
来源：http://hz.vqdsnc.cn/gtqrhayxgv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hysaishi.cn/gtagknufwm.html

[C15] 解构 / 展开参数
来源：http://hz.zhixingplan.top/gtkmhfrgjh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zdqjudy.top/gtdmhlihqq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shanyushiyangkeji.top/gtdkeghdcl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.feifeiyinyue.top/gtcdhbotkd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shangyingyoupin.top/gtxzbozkaf.html

Java: // 无解构
来源：http://hz.pycfn.com/gtrqhtmwyb.html

Go:   // 无解构
来源：http://hz.sysykeji.top/gtiogpdkiv.html

Ruby: a, b = pair
来源：http://hz.wangdashe.top/gtpuuoyfgh.html

C#:   var (a, b) = pair;
来源：http://hz.nwbrower.top/gtqtzisymq.html

[C16] 函数 / 方法重载
来源：http://hz.hnxiangtu.top/gteqxxatxt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nwbrower.top/gtduxkkebd.html

PHP:  // 无重载
来源：http://hz.guowangkeji.top/gtyqqqcnqe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xuetiantiany.cn/gtjuqxefrj.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.smart0.xyz/gtyztlbxxg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ivvv.top/gtxnuctilp.html

Go:   // 无重载：用不同函数名
来源：http://hz.ppjwa.cn/gtnycspodo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yuxming.cn/gttyfuwhlo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.316326.xyz/gtvhselwjn.html

================================================================================
来源：http://hz.vqdsnc.cn/gtfhacknua.html

D. 数组 / 列表 / 集合
来源：http://hz.svipenyu.cn/gtrxruygxw.html

================================================================================
来源：http://hz.fengsongda.top/gttxzwuxoc.html

[D01] 创建数组 / 列表
来源：http://hz.snrcjt.cn/gtbdjuevyo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.snrcjt.cn/gtaaekmitr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.aibaodan.cn/gttxxbmibn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhiwuduotai.top/gtxkkesiqh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hysaishi.cn/gtdxmdfkzz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xylfe.cn/gtkqkdddhu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhijiandao.cn/gtivrfcvdj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhoulong.xyz/gtmzhugkbt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xingfuxueyuan.xyz/gtdvwdkwhk.html

[D02] 追加元素到末尾
来源：http://hz.yueranfly.top/gtjjikwrll.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.mhx1999.top/gthmvbcvdv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sweek.top/gtbhnzozcn.html

JS:   arr.push(4);
来源：http://hz.ybcxt.top/gtkngxfhrm.html

TS:   arr.push(4);
来源：http://hz.zycfv.cn/gtinkxhauc.html

Java: list.add(4);
来源：http://hz.52xcode.cn/gtkrcpcfdz.html

Go:   arr = append(arr, 4)
来源：http://hz.shanyushiyangtech.top/gtoltmlaij.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.smart0.xyz/gtjmburevw.html

C#:   list.Add(4);
来源：http://hz.cashguo.top/gtpvgmdnzg.html

[D03] 在指定位置插入元素
来源：http://hz.shangyingyoupin.top/gtxyiegnmu.html

Py:   arr.insert(0, 0)
来源：http://hz.chenjidiqi.icu/gtwvkeyehq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sufxvd.cn/gtzdosbsgi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.birdmap.top/gtrtefkari.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jlsjyb.cn/gthywelkox.html

Java: list.add(0, 0);
来源：http://hz.cqqwz.cn/gtwnvunlrw.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenjidiqi.icu/gtkwkseesb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.iojbl.cn/gttpyqphuw.html

C#:   list.Insert(0, 0);
来源：http://hz.sysykeji.top/gtgfagfghj.html

[D04] 删除元素
来源：http://hz.52xcode.cn/gtdernfksc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cdnleiting.top/gteqfccxlj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.pycfn.com/gtayvxaogu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gaohongyu789.top/gtnspjklvs.html

TS:   arr.splice(0, 1);
来源：http://hz.xingfuxueyuan.xyz/gtayxrwlkg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shuidangran.top/gtxukapaan.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.quarkkingdee.top/gtklvhjaep.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.havefunace.top/gthxcgzkec.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.kuanghao11.cn/gtxkmjprzj.html

[D05] 访问与修改元素
来源：http://hz.xuetiantiany.cn/gtlcfvfemw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daxiang520.top/gtsfxsqzjz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cdnleiting.top/gtjxriyujj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ydjk.org.cn/gtdcdqgdvv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hammf.cn/gtyqtfylwt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.snrcjt.cn/gtnjkhfjjw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gtpfjuxvjl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sxryk.cn/gtgqzefruc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cqqwz.cn/gtzslldmgg.html

[D06] 数组长度
来源：http://hz.xylfe.cn/gtqpfdwtrl.html

Py:   len(arr)
来源：http://hz.meibo888.top/gtkkuoiqlm.html

PHP:  count($arr);
来源：http://hz.redwolf501.top/gtgyqcszgl.html

JS:   arr.length
来源：http://hz.jinyuanbaomall.cn/gtuetonwug.html

TS:   arr.length
来源：http://hz.snrcjt.cn/gtcwbyhtiq.html

Java: list.size();
来源：http://hz.yanxiufei.cn/gtmyybertk.html

Go:   len(arr)
来源：http://hz.jinyuanbaomall.cn/gtooqhruzx.html

Ruby: arr.length; arr.size
来源：http://hz.9152youxi.cn/gtptvtwvll.html

C#:   list.Count;
来源：http://hz.52xcode.cn/gtsstjywgw.html

[D07] 切片 / 取子数组
来源：http://hz.ywan-chungtsiang.top/gtajikxkol.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.feifeiyinyue.top/gtwbbayfoi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hfpthk.cn/gtpolhshdo.html

JS:   arr.slice(1, 4);
来源：http://hz.feifeiyinyue.top/gtfhjilahf.html

TS:   arr.slice(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtahnxlidj.html

Java: list.subList(1, 4);
来源：http://hz.meibo888.top/gtzhmpktoj.html

Go:   arr[1:4]
来源：http://hz.smart0.xyz/gtyircommb.html

Ruby: arr[1, 3]
来源：http://hz.hnqzz.top/gtjmtjxliu.html

C#:   list.GetRange(1, 3);
来源：http://hz.kuanghao11.cn/gtekyhgyll.html

[D08] 合并两个数组
来源：http://hz.shanyushiyangtech.top/gtflwckchu.html

Py:   a + b;  a.extend(b)
来源：http://hz.52xcode.cn/gthaheujbh.html

PHP:  array_merge($a, $b);
来源：http://hz.xinyue.icu/gtvcrkwowz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ydjk.org.cn/gtpokeozyk.html

TS:   [...a, ...b];
来源：http://hz.gzhubu.top/gtvtwplcvh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xylfe.cn/gtpgqrazsn.html

Go:   append(a, b...)
来源：http://hz.chenjidiqi.icu/gtdfzshqht.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhijiandao.cn/gtwsvmyxhh.html

C#:   a.Concat(b).ToList()
来源：http://hz.sweek.top/gtfnsxryop.html

[D09] 排序（升序）
来源：http://hz.316326.xyz/gtjzfqljjg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tanke756.top/gthpyzdftn.html


<!-- 参考信息 -->