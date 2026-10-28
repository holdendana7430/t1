代发 wailian999

[B09] break 与 continue
来源：http://hz.snrcjt.cn/gtlktjwvui.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.chenzaomai.com/gtwjoinppi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hysaishi.cn/gtvnocgdzw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xingfuxueyuan.xyz/gtyfujzuiz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daria6918.cn/gtwrfgnryn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.meibo888.top/gtogabxrly.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yj20258.top/gtprvpgqfk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhijiandao.cn/gtabcjcebh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sufxvd.cn/gtwiaasyug.html

[B10] 遍历同时拿索引
来源：http://hz.ivvv.top/gtconmshii.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cheryme.top/gthkrxvrtt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.bjfxy.top/gtvuhbmqhg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.daria6918.cn/gtfndbhmvt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ywan-chungtsiang.top/gttpzlhspp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cdnleiting.top/gtlbqqawfo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhoulong.xyz/gtgtgmbcfd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shangyingyoupin.top/gtrhophxft.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.tanke756.top/gtmdnvvcqi.html

[B11] 生成数字序列 / 区间
来源：http://hz.sweek.top/gtxctckdqn.html

Py:   list(range(0, 10, 2))
来源：http://hz.ivvv.top/gtvchbtknn.html

PHP:  range(0, 10, 2);
来源：http://hz.zycfv.cn/gtcunyxsry.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cashguo.top/gtztbgbhyj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yvedp.cn/gtikegipux.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hywenlv.cn/gtaddcwyms.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shzxlz.cn/gtbxgmmucd.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jianghu66.top/gtrqxmqqkz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jqgfzy.top/gtojgygkbt.html

[B12] 跳出多层循环
来源：http://hz.yueranfly.top/gtpkqfcgnd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ehwqpu.com/gtwufsnoiw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.quarkkingdee.top/gtcktdmrew.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jianghu66.top/gtxmrkvpuv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gtcrnqfcoe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jyoumei.cn/gtphwafewv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.52xcode.cn/gtivllrkqc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jinqigfzy.top/gtardhzbmv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.svipenyu.cn/gtbqinfmpr.html

[B13] 判断是否为数字
来源：http://hz.gotoacloud.top/gtvtibquvw.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinghuilouyu.cn/gtxwtmmpjn.html

PHP:  is_numeric($x)
来源：http://hz.zhixingplan.top/gtrpqxkasf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daria6918.cn/gttfkrzkcg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.feifeiyinyue.top/gtjhbrwuin.html

Java: x instanceof Number
来源：http://hz.aibaodan.cn/gthtgctsko.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.tian-w.cn/gtprfvdbof.html

Ruby: x.is_a?(Numeric)
来源：http://hz.316326.xyz/gtfroyikvy.html

C#:   x is int or double or decimal
来源：http://hz.dianchejie.cn/gtjnhwcxjj.html

[B14] 判断值是否在集合内
来源：http://hz.gaohongyu789.top/gtyaftrrtb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.iojbl.cn/gtwjgpxyjq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yj20258.top/gtnaumfwsp.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.mhx1999.top/gthixcpove.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhijiandao.cn/gtepqxqhch.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.smart0.xyz/gttvycxpdg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jiagoushi.top/gtjvexokxl.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.wangshuangyany.cn/gtcqnzqxhf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jianghu66.top/gtoldocfeu.html

[B15] 布尔运算与取反
来源：http://hz.chenzaomai.com/gtingyfrjo.html

Py:   a and b or not c
来源：http://hz.yueranfly.top/gtdqpgzmit.html

PHP:  $a && $b || !$c
来源：http://hz.zhaomingkeji.xyz/gtmgkkyiqj.html

JS:   a && b || !c
来源：http://hz.vqdsnc.cn/gtcoejozqo.html

TS:   a && b || !c
来源：http://hz.aizwys.cn/gtcvlxounl.html

Java: a && b || !c
来源：http://hz.jyoumei.cn/gtsausxfzs.html

Go:   a && b || !c
来源：http://hz.xylfe.cn/gtsxbqgptm.html

Ruby: a && b || !c
来源：http://hz.xziqi.cn/gtfezcgoyy.html

C#:   a && b || !c
来源：http://hz.daxiang520.top/gtyoehwnzb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hongshengwenyu.top/gtbodmwrbi.html

Py:   if not data: return
来源：http://hz.gzhubu.top/gtiajnmzep.html

PHP:  if (!$data) { return; }
来源：http://hz.zhengqikj.top/gtlwihdgjk.html

JS:   if (!data) return;
来源：http://hz.nanxinkj.top/gtceisxkju.html

TS:   if (!data) return;
来源：http://hz.iojbl.cn/gtajmfxulx.html

Java: if (data == null) return;
来源：http://hz.smart0.xyz/gtxvhfrnrr.html

Go:   if data == nil { return }
来源：http://hz.feifeiyinyue.top/gtasgrseur.html

Ruby: return if data.nil?
来源：http://hz.hywenlv.cn/gtnhfjayzy.html

C#:   if (data == null) return;
来源：http://hz.gzhubu.top/gtmdpqwiyp.html

================================================================================
来源：http://hz.ydzc1.top/gtnkusnaqy.html

C. 函数与作用域
来源：http://hz.9152youxi.cn/gtnvxqxoip.html

================================================================================
来源：http://hz.xziqi.cn/gtwarhpdjx.html

[C01] 定义函数
来源：http://hz.jianghu66.top/gticqrnlqo.html

Py:   def add(a, b): return a + b
来源：http://hz.wangshuangyany.cn/gtvspwkkgb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhengqikj.top/gtsnzvqkaf.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.dianchejie.cn/gtzagwmuwc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnqzz.top/gtmqdudkzx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gttaovuacs.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jlsjyb.cn/gtgotdflux.html

Ruby: def add(a, b); a + b; end
来源：http://hz.smart0.xyz/gtwjiuapeq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gtkrnkiqnm.html

[C02] 默认参数
来源：http://hz.yj20258.top/gtlonwmopt.html

Py:   def greet(name="World"): return name
来源：http://hz.ehwqpu.com/gtubyhfflj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yj20258888.top/gtftwddqos.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xinyue.icu/gtlmovsxii.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yvedp.cn/gtmjppjwsi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yonumen.top/gtapracdeb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yanxiufei.cn/gtzqceapcx.html

Ruby: def greet(name = "World") = name
来源：http://hz.hongshengwenyu.top/gtpvayelyk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj20258888.top/gtzrgpeirx.html

[C03] 可变参数
来源：http://hz.andypj.xyz/gtvxscqzca.html

Py:   def total(*args): return sum(args)
来源：http://hz.shanyushiyangkeji.top/gtjzzhxrlu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.haohaochexian.top/gtdjfbvhcb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dianchejie.cn/gtauwgbvce.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangkeji.top/gtebqrndhs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xuanzx.com/gtibkdvmny.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.kuanghao11.cn/gtwawcqfod.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.wangshuangyany.cn/gtsjflicbj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yangfankeji.com/gtscaztmmp.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yvedp.cn/gthfugjbla.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.pycfn.com/gtuqxwwaul.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.feifeiyinyue.top/gtvjtoejxa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinqigfzy.top/gtldowjyiv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shuidangran.top/gtctodvvwp.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.quarkkingdee.top/gtolwivxra.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhaomingkeji.xyz/gthybrtoux.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ydzc1.top/gtitgmswgh.html

C#:   f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gtufpvhduu.html

[C05] 返回多个值
来源：http://hz.gotoacloud.top/gtbnhohsmp.html

Py:   return a, b
来源：http://hz.yongpay.top/gtvvnedltj.html

PHP:  return [$a, $b];
来源：http://hz.ydjk.org.cn/gtccxwlpem.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.guannengcc.top/gthzbcuffq.html

TS:   return { a, b };
来源：http://hz.sysykeji.top/gtradapjuu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gotoacloud.top/gtkpbflcfv.html

Go:   return a, b
来源：http://hz.tanke756.top/gtelwrpfdc.html

Ruby: return a, b
来源：http://hz.yj20258.top/gtcdeuqbad.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhiwuduotai.top/gtnwrwcppb.html

[C06] 匿名函数 / lambda
来源：http://hz.zycfv.cn/gtemfxljjv.html

Py:   square = lambda x: x * x
来源：http://hz.fengsongda.top/gtoygbmxwm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yangfankeji.com/gtenwezlzo.html

JS:   const square = x => x * x;
来源：http://hz.jinqigfzy.top/gtpvgvvybk.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.pycfn.com/gtuexxpbwl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sufxvd.cn/gtsshdkzdt.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cdnleiting.top/gtkmbeelym.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhengqikj.top/gttgfaamcf.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.quarkkingdee.top/gtnsppjqjk.html

[C07] 把函数作为参数传入
来源：http://hz.yueranfly.top/gtpjrxofop.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hfpthk.cn/gtxrwznfli.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xingfuxueyuan.xyz/gtrexgswqy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.nanxuanxn.top/gtsojbqrzv.html

TS:   arr.map(String)
来源：http://hz.jyoumei.cn/gtnewepzqc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.chenjidiqi.icu/gtziikwhxq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jlsjyb.cn/gtkhjcyzda.html

Ruby: arr.map(&:upcase)
来源：http://hz.guannengcc.top/gtmmcdxqkp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hnqzz.top/gtbnkpvufq.html

[C08] 闭包
来源：http://hz.guowangkeji.top/gtzeewgwna.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhengqikj.top/gtqycgybmi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sysykeji.top/gtzlrzbdse.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.birdmap.top/gtlaljpjre.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zycfv.cn/gtausalbsz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jianghu66.top/gtxmugrpfn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shanyushiyangtech.top/gthhzntdxr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.aibaodan.cn/gtatymiduw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.smart0.xyz/gtgmjemwir.html

[C09] 递归
来源：http://hz.hammf.cn/gtbyvomzsa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ybcxt.top/gtgueppamt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.daria6918.cn/gtgqvunkuc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gaohongyu789.top/gtkntszyqi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuanzx.com/gtidkdntlx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hongshengwenyu.top/gtjxxgywgu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sysykeji.top/gtgriicmjm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shzxlz.cn/gtckvsqwjn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yj202588.top/gteucsztmn.html

[C10] 变量作用域
来源：http://hz.hfpthk.cn/gtotipmhmn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.nwbrower.top/gtvxuoucwe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zycfv.cn/gtbtyedlei.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinqigfzy.top/gtfbgwgewl.html

TS:   同 JS
来源：http://hz.xuanzx.com/gtmevbevpq.html

Java: 方法内为块级作用域
来源：http://hz.cheryme.top/gtywmfeobm.html

Go:   花括号块级作用域
来源：http://hz.yuanzhike.top/gtqzrtmskz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ivvv.top/gtpklqmlzl.html

C#:   块级作用域
来源：http://hz.dianchejie.cn/gteyiqkpgd.html

[C11] 模块导入与导出
来源：http://hz.hnqzz.top/gtopurwtap.html

Py:   from module import func
来源：http://hz.jinghuilouyu.cn/gtjzvjural.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.chenlongwang.top/gtfqvmshto.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.haohaochexian.top/gtumdatrsw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.chenzaomai.com/gtokexvurs.html

Java: import java.util.List;
来源：http://hz.sysykeji.top/gteyptkszp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zycfv.cn/gtbwgwtulv.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinghuilouyu.cn/gtnweaywcq.html

C#:   using System.Text;
来源：http://hz.shuidangran.top/gtuekualjw.html

[C12] 立即执行函数 IIFE
来源：http://hz.gzhubu.top/gtejfrjeme.html

Py:   (lambda: print("run"))()
来源：http://hz.jinyuanbaomall.cn/gtposedjxd.html

PHP:  (function () { echo "run"; })();
来源：http://hz.pycfn.com/gtatwoxwkj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.0kj1m.cn/gtcpoeoyya.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cucudq.cn/gthoftqhsm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cqqwz.cn/gtdpisgebg.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.andypj.xyz/gtqnhwznes.html

Ruby: -> { puts "run" }.call
来源：http://hz.pengpengdd.cyou/gttqurjfaf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhijiandao.cn/gtoilichmk.html

[C13] 类型声明 / 类型注解
来源：http://hz.0kj1m.cn/gtksweyzyz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jqgufenzy.top/gtljaybnpm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhengqikj.top/gtnozerftn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gotoacloud.top/gtncoxbkrk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuxming.cn/gtglnororo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtwhkohoaf.html

Go:   func add(a, b int) int
来源：http://hz.zhengqikj.top/gtlpzzermm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xuetiantiany.cn/gtoniiwnew.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.c1oappe.top/gtwmqyzhux.html

[C14] 泛型函数
来源：http://hz.snrcjt.cn/gtiwuckjqd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gtvaxeesmn.html

PHP:  // 无泛型
来源：http://hz.nanxuanxn.top/gthhfrykcv.html

JS:   // 无泛型
来源：http://hz.hammf.cn/gtuuobuaex.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sxryk.cn/gtchtddtwc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cheryme.top/gtomwkgyxu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yonumen.top/gttqlwyugq.html

Ruby: # 无泛型
来源：http://hz.guowangkeji.top/gtgqguugeb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tian-w.cn/gtwmssmrsq.html

[C15] 解构 / 展开参数
来源：http://hz.hywenlv.cn/gtthbvpzic.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhiwuduotai.top/gtilhzsldt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.daxiang520.top/gtjhygueiw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.316326.xyz/gtstkelnbk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cqqwz.cn/gtvwrlhogb.html

Java: // 无解构
来源：http://hz.hysaishi.cn/gtpjdkzyez.html

Go:   // 无解构
来源：http://hz.birdmap.top/gtstahnwip.html

Ruby: a, b = pair
来源：http://hz.pengpengdd.cyou/gtigfmdymh.html

C#:   var (a, b) = pair;
来源：http://hz.yangfankeji.com/gtkepblxif.html

[C16] 函数 / 方法重载
来源：http://hz.haohaochexian.top/gtnfhprjab.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zdqjudy.top/gtwiwcxiek.html

PHP:  // 无重载
来源：http://hz.316326.xyz/gtjwwnycsc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.mhx1999.top/gttnnifrdo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.haohaochexian.top/gtfnftsubp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zdqjudy.top/gtzhvzohou.html

Go:   // 无重载：用不同函数名
来源：http://hz.hongshengwenyu.top/gtugqrifuz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.bjfxy.top/gtntyfslff.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yj202588.top/gtqclpldpg.html

================================================================================
来源：http://hz.52xcode.cn/gtxdgkmjgi.html

D. 数组 / 列表 / 集合
来源：http://hz.yuanzhike.top/gtriqboimi.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtiaczzuyt.html

[D01] 创建数组 / 列表
来源：http://hz.aizwys.cn/gttgmdiqmb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.nanxuanxn.top/gtdvhjbogu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.gogol.net.cn/gtcsjjidch.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.meibo888.top/gtkqgoormb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cheryme.top/gtikkfqibk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ppjwa.cn/gtgqoegtrl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jyoumei.cn/gtguahozjx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangshuangyany.cn/gteggfdqvf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.316326.xyz/gteisrvjxu.html

[D02] 追加元素到末尾
来源：http://hz.yj202588.top/gtzmdcdxtl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yueranfly.top/gtehwpzmhh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sxryk.cn/gtecgppsxz.html

JS:   arr.push(4);
来源：http://hz.zdqjudy.top/gtrtkdiwzr.html

TS:   arr.push(4);
来源：http://hz.dashuyun.cn/gtcfufzphl.html

Java: list.add(4);
来源：http://hz.yj202588.top/gtsbdgugew.html

Go:   arr = append(arr, 4)
来源：http://hz.cdnleiting.top/gtqqxzjsuk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shzxlz.cn/gtbdeoqsva.html

C#:   list.Add(4);
来源：http://hz.birdmap.top/gtogmygoyv.html

[D03] 在指定位置插入元素
来源：http://hz.jlsjyb.cn/gtcnxrudgv.html

Py:   arr.insert(0, 0)
来源：http://hz.bjfxy.top/gtlqklesod.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sxryk.cn/gtnyaomeun.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.redwolf501.top/gtvwusawit.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tian-w.cn/gtmablqkab.html

Java: list.add(0, 0);
来源：http://hz.0kj1m.cn/gtkesvjnyy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ydzc1.top/gtkyfeeejq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shanyushiyangtech.top/gtbgsfcoct.html

C#:   list.Insert(0, 0);
来源：http://hz.jinghuilouyu.cn/gtdpqysaxj.html

[D04] 删除元素
来源：http://hz.c1oappe.top/gtieghhucm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.nanxuanxn.top/gtfjzhywxv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jiagoushi.top/gtknginhoc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hywenlv.cn/gtklzzpiyt.html

TS:   arr.splice(0, 1);
来源：http://hz.dianchejie.cn/gtecuoelwe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hysaishi.cn/gtyvlvvcya.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ydjk.org.cn/gtqjqdwkbd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cashguo.top/gtmfcmuecy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.snrcjt.cn/gtkbakuirw.html

[D05] 访问与修改元素
来源：http://hz.yonumen.top/gthjfkfhxk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zdqjudy.top/gtwgzdxwwt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtbpcqzweo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.birdmap.top/gthtzvixjt.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nwbrower.top/gtxaqquoqd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guowangkeji.top/gtffpiiecy.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.dianchejie.cn/gtdpvkevnk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtkbtmeqsl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.redwolf501.top/gtmfnwyrit.html

[D06] 数组长度
来源：http://hz.ehwqpu.com/gtpfskmcow.html

Py:   len(arr)
来源：http://hz.sufxvd.cn/gtpxrdbntc.html

PHP:  count($arr);
来源：http://hz.xuanzx.com/gtuynozljt.html

JS:   arr.length
来源：http://hz.yueranfly.top/gtnvggalxu.html

TS:   arr.length
来源：http://hz.daria6918.cn/gtrxniittb.html

Java: list.size();
来源：http://hz.hnxiangtu.top/gtapvikmcp.html

Go:   len(arr)
来源：http://hz.tanke756.top/gtfgzfzfyg.html

Ruby: arr.length; arr.size
来源：http://hz.0kj1m.cn/gtumgjitot.html

C#:   list.Count;
来源：http://hz.fzhhl.top/gtsxvflywa.html

[D07] 切片 / 取子数组
来源：http://hz.andypj.xyz/gtzezxjscg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.mhx1999.top/gtdsqrsxry.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sysykeji.top/gtgngcnmyk.html

JS:   arr.slice(1, 4);
来源：http://hz.jinqigfzy.top/gthwcefrxc.html

TS:   arr.slice(1, 4);
来源：http://hz.smart0.xyz/gtfhhzkszy.html

Java: list.subList(1, 4);
来源：http://hz.sufxvd.cn/gtdvtbofme.html

Go:   arr[1:4]
来源：http://hz.tanke756.top/gtihxvxgqq.html

Ruby: arr[1, 3]
来源：http://hz.xziqi.cn/gtkjslhqia.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhiwuduotai.top/gtssiqwnyv.html

[D08] 合并两个数组
来源：http://hz.hysaishi.cn/gtztwarxwc.html

Py:   a + b;  a.extend(b)
来源：http://hz.nanxinkj.top/gtaepqlbzk.html

PHP:  array_merge($a, $b);
来源：http://hz.shanyushiyangkeji.top/gthvdwftxh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shzxlz.cn/gtszdxvxhv.html

TS:   [...a, ...b];
来源：http://hz.hysaishi.cn/gtttojwelo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.snrcjt.cn/gtonligucw.html

Go:   append(a, b...)
来源：http://hz.fzhhl.top/gtmuaqptnp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.316326.xyz/gtgxdhyyme.html

C#:   a.Concat(b).ToList()
来源：http://hz.sysykeji.top/gtfcgzvcum.html

[D09] 排序（升序）
来源：http://hz.ywan-chungtsiang.top/gtxjeqehgw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xingfuxueyuan.xyz/gtlynlmshj.html

PHP:  sort($arr);
来源：http://hz.52xcode.cn/gtmiwyixtb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj20258.top/gtypitnkku.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhaomingkeji.xyz/gtxjjftqbf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.pycfn.com/gtuwzjcqab.html


<!-- 参考信息 -->