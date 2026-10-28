代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtniswhcom.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sweek.top/gtxkyuvecj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zycfv.cn/gtpbawrwbw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yongpay.top/gtyisgshkw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtlcmhovqp.html

[B10] 遍历同时拿索引
来源：http://hz.hammf.cn/gthtlaoecf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.hongshengwenyu.top/gtfeiojoyd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xuetiantiany.cn/gtpfwhtgmv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xziqi.cn/gtfvsewodd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.gzhubu.top/gtpsunywgi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yonumen.top/gtvzbbzcyz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xziqi.cn/gtnwcrjnfo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.andypj.xyz/gtoozjehdj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.daria6918.cn/gtaftxximl.html

[B11] 生成数字序列 / 区间
来源：http://hz.svipenyu.cn/gtrvkdokna.html

Py:   list(range(0, 10, 2))
来源：http://hz.shangyingyoupin.top/gtxdqbnktj.html

PHP:  range(0, 10, 2);
来源：http://hz.tianlin.xyz/gtdoplbpty.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.pengpengdd.cyou/gtkdtonfkx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gzhubu.top/gtyodqyrsp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cheryme.top/gtdebjcocd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yvedp.cn/gtkipavtoo.html

Ruby: (0...10).step(2).to_a
来源：http://hz.tanke756.top/gtsfspdyyu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xziqi.cn/gtrzkfjypy.html

[B12] 跳出多层循环
来源：http://hz.redwolf501.top/gtjvawwzpa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hammf.cn/gtyeyrcegi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.smart0.xyz/gtfcgiryot.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xinyue.icu/gtooupsetx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cucudq.cn/gtrukusekj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.birdmap.top/gtvdiemqmz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xylfe.cn/gtgogcokqi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hnqzz.top/gtbimytjwl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.bjfxy.top/gtxuwckuvc.html

[B13] 判断是否为数字
来源：http://hz.ppjwa.cn/gtutyetaca.html

Py:   isinstance(x, (int, float))
来源：http://hz.fengsongda.top/gtuabrhqyv.html

PHP:  is_numeric($x)
来源：http://hz.bjfxy.top/gtsugdldgx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtyflpigom.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tianlin.xyz/gtarvrxacv.html

Java: x instanceof Number
来源：http://hz.yj20258.top/gtfybxtjrd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.fzhhl.top/gtyavbtwrm.html

Ruby: x.is_a?(Numeric)
来源：http://hz.daxiang520.top/gthxjnoqbr.html

C#:   x is int or double or decimal
来源：http://hz.ybcxt.top/gtkzhwogxs.html

[B14] 判断值是否在集合内
来源：http://hz.fengsongda.top/gtjanqpren.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zycfv.cn/gtpvdvpjqy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.bjfxy.top/gtspmjvpzi.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinghuilouyu.cn/gtkgrbqzxv.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhiwuduotai.top/gtrymbspfv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.redwolf501.top/gtwqrbwqwr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cashguo.top/gtcxjqnqqv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ydjk.org.cn/gtdmrcuaci.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.redwolf501.top/gtwkfzyfrl.html

[B15] 布尔运算与取反
来源：http://hz.havefunace.top/gtfaeqpnkj.html

Py:   a and b or not c
来源：http://hz.xingfuxueyuan.xyz/gtykvwvzrh.html

PHP:  $a && $b || !$c
来源：http://hz.zhiwuduotai.top/gtwcbikdnk.html

JS:   a && b || !c
来源：http://hz.quarkkingdee.top/gtbwogqbtk.html

TS:   a && b || !c
来源：http://hz.yvedp.cn/gtaaboijwo.html

Java: a && b || !c
来源：http://hz.yj20258888.top/gtkcnlkves.html

Go:   a && b || !c
来源：http://hz.gotoacloud.top/gtfelnkevf.html

Ruby: a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtyhaauzlc.html

C#:   a && b || !c
来源：http://hz.yanxiufei.cn/gtmsqagggv.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ydzc1.top/gtzhaghbqk.html

Py:   if not data: return
来源：http://hz.aibaodan.cn/gtqqfyfgcz.html

PHP:  if (!$data) { return; }
来源：http://hz.ywan-chungtsiang.top/gttjxxasmg.html

JS:   if (!data) return;
来源：http://hz.xylfe.cn/gtoclutnlo.html

TS:   if (!data) return;
来源：http://hz.guannengcc.top/gtnlkeudac.html

Java: if (data == null) return;
来源：http://hz.daria6918.cn/gtrssybiad.html

Go:   if data == nil { return }
来源：http://hz.zhoulong.xyz/gtjjjfeuwq.html

Ruby: return if data.nil?
来源：http://hz.cashguo.top/gtigldigfc.html

C#:   if (data == null) return;
来源：http://hz.xziqi.cn/gtwjumubdk.html

================================================================================
来源：http://hz.yvedp.cn/gtwsflgaxe.html

C. 函数与作用域
来源：http://hz.zdqjudy.top/gthdlhvgql.html

================================================================================
来源：http://hz.meibo888.top/gtfzusprjy.html

[C01] 定义函数
来源：http://hz.yj202588.top/gtvnntwlme.html

Py:   def add(a, b): return a + b
来源：http://hz.sufxvd.cn/gtawiaitcv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ehwqpu.com/gttmjbsawk.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hywenlv.cn/gtddnkhqbu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigfzy.top/gtpqzafvml.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtvyhrhhca.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yvedp.cn/gthusukwin.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hammf.cn/gtgjwpqmgr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtataejbhs.html

[C02] 默认参数
来源：http://hz.wangdashe.top/gtcygkxxph.html

Py:   def greet(name="World"): return name
来源：http://hz.shanyushiyangtech.top/gtsponngxz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nwbrower.top/gtnjaamdic.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ydzc1.top/gtcddzxacj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hongshengwenyu.top/gtuekhfogr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xuetiantiany.cn/gtunddsdjf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sufxvd.cn/gtaikhrdyh.html

Ruby: def greet(name = "World") = name
来源：http://hz.9152youxi.cn/gtoordknsr.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhaomingkeji.xyz/gtwoavxvxc.html

[C03] 可变参数
来源：http://hz.c1oappe.top/gtzqyvjpsx.html

Py:   def total(*args): return sum(args)
来源：http://hz.316326.xyz/gtrodsxism.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xziqi.cn/gtiyalgiet.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nanxuanxn.top/gtentfyodq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgufenzy.top/gtvvcorhem.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.c1oappe.top/gtlgqmdhac.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.fengsongda.top/gtvdeijajj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shanyushiyangtech.top/gtbpkhyxzs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinqigfzy.top/gtgzojylgl.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xylfe.cn/gtclbukrbm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.pengpengdd.cyou/gtwvoedjzb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yangfankeji.com/gtfqaeqnro.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.iojbl.cn/gtwbqtufga.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.fzhhl.top/gtrjbbtwht.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhoulong.xyz/gttybpiago.html

Go:   // 无：用配置结构体参数
来源：http://hz.9152youxi.cn/gtnbgojjng.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtxsqbqyhq.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj20258888.top/gtkluwbdgc.html

[C05] 返回多个值
来源：http://hz.yangfankeji.com/gtkvokijxs.html

Py:   return a, b
来源：http://hz.jinqigfzy.top/gtipjyilbc.html

PHP:  return [$a, $b];
来源：http://hz.hywenlv.cn/gtxtdyfjmt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shzxlz.cn/gtnuzuremm.html

TS:   return { a, b };
来源：http://hz.nwbrower.top/gtakbgwyxj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.andypj.xyz/gtvwnassta.html

Go:   return a, b
来源：http://hz.haohaochexian.top/gtjhpkmeuj.html

Ruby: return a, b
来源：http://hz.cheryme.top/gteymjdtev.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.havefunace.top/gtdlbmsjth.html

[C06] 匿名函数 / lambda
来源：http://hz.dianchejie.cn/gtwyqchihd.html

Py:   square = lambda x: x * x
来源：http://hz.xinyue.icu/gtnhwrlrpc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.kuanghao11.cn/gtaaaubzqq.html

JS:   const square = x => x * x;
来源：http://hz.yonumen.top/gtpcbhwqpf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhoulong.xyz/gtvwxofujk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.svipenyu.cn/gtzwkpauul.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cheryme.top/gtbursxvyx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.haohaochexian.top/gtlxhrxmjb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj202588.top/gtzxnipviw.html

[C07] 把函数作为参数传入
来源：http://hz.meibo888.top/gtelpyglhk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yongpay.top/gtlhfgiogc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ybcxt.top/gtyovvknan.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhoulong.xyz/gtjvmihghl.html

TS:   arr.map(String)
来源：http://hz.smart0.xyz/gtlahbqzvz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hnqzz.top/gtgpfggoix.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xziqi.cn/gtoqilbpjy.html

Ruby: arr.map(&:upcase)
来源：http://hz.sysykeji.top/gtpfxsqfkb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.cqqwz.cn/gtjdqbxwvv.html

[C08] 闭包
来源：http://hz.aizwys.cn/gthdiwcusj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.fengsongda.top/gtgsyomydm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sufxvd.cn/gtnftzsrwo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtalqbbpss.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtvpwrlioq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sysykeji.top/gtnwqenghf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hnqzz.top/gtlcmlpbis.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hysaishi.cn/gtgaqjvbul.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhijiandao.cn/gtrdjjkjqd.html

[C09] 递归
来源：http://hz.yongpay.top/gtfmndeloa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shangyingyoupin.top/gtmuucvgkq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.guowangkeji.top/gtzbbxcqqy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dianchejie.cn/gtivrxwzcn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.birdmap.top/gtmigrvvma.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shanyushiyangtech.top/gthneaulvh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zycfv.cn/gtanffatxa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinqigfzy.top/gtbjgibbrw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shuidangran.top/gtsxczvicm.html

[C10] 变量作用域
来源：http://hz.dashuyun.cn/gtvpaxtiym.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.daxiang520.top/gtgkcmsehn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxuanxn.top/gthyjxvwxm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yj202588.top/gtzlrrfguw.html

TS:   同 JS
来源：http://hz.shuidangran.top/gtgsmcxfga.html

Java: 方法内为块级作用域
来源：http://hz.yangfankeji.com/gtnfzzwepb.html

Go:   花括号块级作用域
来源：http://hz.yueranfly.top/gtovotwlul.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhaomingkeji.xyz/gtmgydrcpf.html

C#:   块级作用域
来源：http://hz.xuanzx.com/gtieubvnoo.html

[C11] 模块导入与导出
来源：http://hz.vqdsnc.cn/gtxqekluwd.html

Py:   from module import func
来源：http://hz.nanxuanxn.top/gtzqdvazmc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hnqzz.top/gtojqpwtev.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hnqzz.top/gtecxbidvk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ydzc1.top/gtabyzsgxq.html

Java: import java.util.List;
来源：http://hz.meibo888.top/gthyvcgzsm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hongshengwenyu.top/gtrmltlvch.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yonumen.top/gtkwrtrbjz.html

C#:   using System.Text;
来源：http://hz.jiagoushi.top/gtxxksjzvz.html

[C12] 立即执行函数 IIFE
来源：http://hz.yuxming.cn/gtmcgobiqu.html

Py:   (lambda: print("run"))()
来源：http://hz.ywan-chungtsiang.top/gtqkebvyky.html

PHP:  (function () { echo "run"; })();
来源：http://hz.redwolf501.top/gtblqtcnhp.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yanxiufei.cn/gtdhwgwnzs.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yuanzhike.top/gtvjuetndt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ehwqpu.com/gtdxzbyyez.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sxryk.cn/gtnyalexsa.html

Ruby: -> { puts "run" }.call
来源：http://hz.dianchejie.cn/gtnyodcvlt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinqigufen.top/gtukgvmuxv.html

[C13] 类型声明 / 类型注解
来源：http://hz.jqgufenzy.top/gtyegaiegf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shzxlz.cn/gteihnyrvt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shangyingyoupin.top/gtpckgbjgk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.guowangkeji.top/gtvlhfrnfh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.bjfxy.top/gtvncdpven.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.nanxinkj.top/gtjjsjxhws.html

Go:   func add(a, b int) int
来源：http://hz.ehwqpu.com/gtbybplkps.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ppjwa.cn/gtuvoufzbt.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hnxiangtu.top/gthsqqljwr.html

[C14] 泛型函数
来源：http://hz.cashguo.top/gtvbflwjjz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ppjwa.cn/gtzbkpmqld.html

PHP:  // 无泛型
来源：http://hz.sweek.top/gtpqflhssm.html

JS:   // 无泛型
来源：http://hz.ybcxt.top/gtuvobyodj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.quarkkingdee.top/gtrfxdrfxu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jianghu66.top/gtrdzfzznq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hfpthk.cn/gtfdfeocup.html

Ruby: # 无泛型
来源：http://hz.xziqi.cn/gthccnkuav.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yueranfly.top/gtiggdqjyf.html

[C15] 解构 / 展开参数
来源：http://hz.dashuyun.cn/gtkafbqktk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgfzy.top/gtcmzhgfbp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhiwuduotai.top/gtcpbsnwbe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.wangshuangyany.cn/gtkvguilwx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhiwuduotai.top/gtveuabchs.html

Java: // 无解构
来源：http://hz.daria6918.cn/gttbdymlls.html

Go:   // 无解构
来源：http://hz.jqgufenzy.top/gtlibujhmj.html

Ruby: a, b = pair
来源：http://hz.9152youxi.cn/gtrfcmwfhp.html

C#:   var (a, b) = pair;
来源：http://hz.sysykeji.top/gtczmayuge.html

[C16] 函数 / 方法重载
来源：http://hz.jinghuilouyu.cn/gtqfkimglw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sxryk.cn/gtyjhwvwxr.html

PHP:  // 无重载
来源：http://hz.havefunace.top/gtxhkzgeui.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jianghu66.top/gttewgybzd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ybcxt.top/gtbiigzhmw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.kuanghao11.cn/gtcmzavuxi.html

Go:   // 无重载：用不同函数名
来源：http://hz.jyoumei.cn/gtszbfmivj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.andypj.xyz/gtvdjbiyhn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ywan-chungtsiang.top/gtgutfxpwz.html

================================================================================
来源：http://hz.snrcjt.cn/gtpmujxpmk.html

D. 数组 / 列表 / 集合
来源：http://hz.cashguo.top/gtdlkebtpu.html

================================================================================
来源：http://hz.tian-w.cn/gtgbjzerik.html

[D01] 创建数组 / 列表
来源：http://hz.jiagoushi.top/gtgdgyhgtb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.fzhhl.top/gtaanzunik.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ydzc1.top/gtnesziflj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aibaodan.cn/gtkmykpluh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ivvv.top/gtxuoqungv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.tian-w.cn/gtczyktxuh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.dashuyun.cn/gtsulzdrla.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangshuangyany.cn/gttaakbqqu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.tanke756.top/gthfpwdbtd.html

[D02] 追加元素到末尾
来源：http://hz.pengpengdd.cyou/gtabouhdgf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shanyushiyangtech.top/gtpbivwbfz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xingfuxueyuan.xyz/gtxodgmhxy.html

JS:   arr.push(4);
来源：http://hz.cqqwz.cn/gtngrmnphu.html

TS:   arr.push(4);
来源：http://hz.yueranfly.top/gtkyojnqxd.html

Java: list.add(4);
来源：http://hz.daxiang520.top/gtbzdoizdy.html

Go:   arr = append(arr, 4)
来源：http://hz.0kj1m.cn/gtyjynzzxq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.guowangkeji.top/gtipqdhsyy.html

C#:   list.Add(4);
来源：http://hz.daxiang520.top/gtunztlitm.html

[D03] 在指定位置插入元素
来源：http://hz.nanxuanxn.top/gtvwjeaisc.html

Py:   arr.insert(0, 0)
来源：http://hz.zhiwuduotai.top/gtuhcdiaub.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.daria6918.cn/gtjtkxrplz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hammf.cn/gtlrslwpoe.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cashguo.top/gtlrakcurr.html

Java: list.add(0, 0);
来源：http://hz.sxryk.cn/gtpooofwww.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ivvv.top/gtjgoxljoh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.316326.xyz/gtkesydurz.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxinkj.top/gtxuvufbmx.html

[D04] 删除元素
来源：http://hz.xuetiantiany.cn/gtxvdocudi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.aibaodan.cn/gtvugtywsv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinqigfzy.top/gtofpebmuc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.andypj.xyz/gtdmtznqrz.html

TS:   arr.splice(0, 1);
来源：http://hz.nanxinkj.top/gtyfbnehvc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hammf.cn/gtzpejadhb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hnxiangtu.top/gtuoakavfo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cqqwz.cn/gtrshdnain.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cucudq.cn/gtjvtbqbqk.html

[D05] 访问与修改元素
来源：http://hz.sweek.top/gtejtqogdx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sweek.top/gtlulqhfvc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.pycfn.com/gtsxecjzov.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.316326.xyz/gtisaiakcm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.haohaochexian.top/gtuuvmiktf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinyuanbaomall.cn/gtvctpzytd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hnqzz.top/gtoqevinyl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tianlin.xyz/gtfyvtylfm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yvedp.cn/gthqisbiel.html

[D06] 数组长度
来源：http://hz.c1oappe.top/gtufqtpfvm.html

Py:   len(arr)
来源：http://hz.hfpthk.cn/gtqsmtgasz.html

PHP:  count($arr);
来源：http://hz.svipenyu.cn/gtisegfrun.html

JS:   arr.length
来源：http://hz.aizwys.cn/gtmyxberht.html

TS:   arr.length
来源：http://hz.aibaodan.cn/gtpryqmhzs.html

Java: list.size();
来源：http://hz.jlsjyb.cn/gtlvhdgewo.html

Go:   len(arr)
来源：http://hz.ybcxt.top/gtfpsntyhw.html

Ruby: arr.length; arr.size
来源：http://hz.vqdsnc.cn/gtznqkizdh.html

C#:   list.Count;
来源：http://hz.gotoacloud.top/gtxqbgqrta.html

[D07] 切片 / 取子数组
来源：http://hz.hfpthk.cn/gtrmszebti.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xylfe.cn/gtjxiwfwlw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tian-w.cn/gtuauwmzgh.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxuanxn.top/gtvxdmrrmh.html

TS:   arr.slice(1, 4);
来源：http://hz.nwbrower.top/gtbuwwunac.html

Java: list.subList(1, 4);
来源：http://hz.tanke756.top/gtbqaafsno.html

Go:   arr[1:4]
来源：http://hz.aibaodan.cn/gtqkpkumex.html

Ruby: arr[1, 3]
来源：http://hz.xingfuxueyuan.xyz/gtvtsxyrao.html

C#:   list.GetRange(1, 3);
来源：http://hz.0kj1m.cn/gtdccesafp.html

[D08] 合并两个数组
来源：http://hz.xinyue.icu/gtavfrvdio.html

Py:   a + b;  a.extend(b)
来源：http://hz.haohaochexian.top/gtnysmopxv.html

PHP:  array_merge($a, $b);
来源：http://hz.jqgufenzy.top/gtbgcimzhg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.nwbrower.top/gtwxuldcgm.html

TS:   [...a, ...b];
来源：http://hz.yonumen.top/gtcghgoefp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sxryk.cn/gtvusejryu.html

Go:   append(a, b...)
来源：http://hz.chenjidiqi.icu/gthbqtdssq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gotoacloud.top/gtsbzwurwc.html

C#:   a.Concat(b).ToList()
来源：http://hz.gogol.net.cn/gtomeuumoa.html

[D09] 排序（升序）
来源：http://hz.cucudq.cn/gtmnchvkle.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.c1oappe.top/gtjavotfzy.html

PHP:  sort($arr);
来源：http://hz.xylfe.cn/gtvrczhsbr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hongshengwenyu.top/gttuwnewsw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hfpthk.cn/gtjatmkctd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.316326.xyz/gtsrhylsnh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhijiandao.cn/gtcykjhrei.html

Ruby: arr.sort
来源：http://hz.tanke756.top/gtxqduwujl.html

C#:   list.Sort();
来源：http://hz.fzhhl.top/gtdugtrbqv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shuidangran.top/gtyfxeaekk.html


<!-- 参考信息 -->