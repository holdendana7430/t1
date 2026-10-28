代发 wailian999

[B09] break 与 continue
来源：http://hz.quarkkingdee.top/gtzszeewct.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.52xcode.cn/gtralvouxe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhiwuduotai.top/gtrhfobqdg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tianlin.xyz/gtgqeuxecq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fengsongda.top/gtrpzvvllc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.kuanghao11.cn/gtcugeqnzo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zdqjudy.top/gtmfqqmywx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhijiandao.cn/gtdxekjorg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yanxiufei.cn/gtbunuvzgb.html

[B10] 遍历同时拿索引
来源：http://hz.shanyushiyangtech.top/gttehrpzzb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yongpay.top/gtlvogpzxr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhiwuduotai.top/gtvwsfbmdm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hysaishi.cn/gtggukmpoa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.9152youxi.cn/gtescehhxl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yuanzhike.top/gtyazebmkg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jlsjyb.cn/gthqgavzza.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jinqigfzy.top/gtwqtdvyky.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.smart0.xyz/gtnxpjqjmg.html

[B11] 生成数字序列 / 区间
来源：http://hz.jianghu66.top/gttbabzpom.html

Py:   list(range(0, 10, 2))
来源：http://hz.jyoumei.cn/gtvruvehzv.html

PHP:  range(0, 10, 2);
来源：http://hz.tian-w.cn/gtleirmatp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yuxming.cn/gtmligqmuk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.c1oappe.top/gtjsznjyzy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.316326.xyz/gtrqjgkzct.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.andypj.xyz/gtonjrhcws.html

Ruby: (0...10).step(2).to_a
来源：http://hz.wangshuangyany.cn/gtajkvwyga.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhiwuduotai.top/gtvnfbysuz.html

[B12] 跳出多层循环
来源：http://hz.yuxming.cn/gteenmvfkh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hammf.cn/gtstxdgajh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.316326.xyz/gtbktlpaku.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.iojbl.cn/gtaawyejbe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangshuangyany.cn/gtatjammze.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ywan-chungtsiang.top/gtwjlcymxo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zycfv.cn/gtrtmuwikn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yangfankeji.com/gteuypfnuj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.quarkkingdee.top/gtjjxnmwya.html

[B13] 判断是否为数字
来源：http://hz.nwbrower.top/gtkqpfwqwi.html

Py:   isinstance(x, (int, float))
来源：http://hz.jqgfzy.top/gtbzfhhmcu.html

PHP:  is_numeric($x)
来源：http://hz.shangyingyoupin.top/gtsnvuevzj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.kuanghao11.cn/gtitdnsnmd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shanyushiyangkeji.top/gtrdsikace.html

Java: x instanceof Number
来源：http://hz.jyoumei.cn/gtbkhhhhwf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.andypj.xyz/gtibuqkbic.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yj20258.top/gtromprvbi.html

C#:   x is int or double or decimal
来源：http://hz.zhixingplan.top/gtdepppmhw.html

[B14] 判断值是否在集合内
来源：http://hz.zhixingplan.top/gtcvvgzygc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhengqikj.top/gtxrtogkvq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zdqjudy.top/gtrudjhkhs.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.fengsongda.top/gtcpczglyw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yvedp.cn/gtuqxijdto.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ppjwa.cn/gtviynytwf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ehwqpu.com/gtotocmiim.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yvedp.cn/gtoqfhdcgf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cucudq.cn/gtezmsupce.html

[B15] 布尔运算与取反
来源：http://hz.wangdashe.top/gtihscqnym.html

Py:   a and b or not c
来源：http://hz.hongshengwenyu.top/gthwislezp.html

PHP:  $a && $b || !$c
来源：http://hz.svipenyu.cn/gtvhpgomzh.html

JS:   a && b || !c
来源：http://hz.yj20258.top/gtrxzcduph.html

TS:   a && b || !c
来源：http://hz.hammf.cn/gtrtmxtaty.html

Java: a && b || !c
来源：http://hz.shuidangran.top/gttlqqlmpi.html

Go:   a && b || !c
来源：http://hz.jqgfzy.top/gtwnnhupww.html

Ruby: a && b || !c
来源：http://hz.chenzaomai.com/gtypxfgoro.html

C#:   a && b || !c
来源：http://hz.aizwys.cn/gtjrhagvup.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sysykeji.top/gtpqtdnkzw.html

Py:   if not data: return
来源：http://hz.aizwys.cn/gtvggestff.html

PHP:  if (!$data) { return; }
来源：http://hz.yanxiufei.cn/gttizkjbkq.html

JS:   if (!data) return;
来源：http://hz.yj202588.top/gtuwymcwob.html

TS:   if (!data) return;
来源：http://hz.wangshuangyany.cn/gtcxdpjqcb.html

Java: if (data == null) return;
来源：http://hz.ybcxt.top/gtgjgwjpgq.html

Go:   if data == nil { return }
来源：http://hz.cdnleiting.top/gtblubarzn.html

Ruby: return if data.nil?
来源：http://hz.52xcode.cn/gtappscvvp.html

C#:   if (data == null) return;
来源：http://hz.cheryme.top/gtmoggntkg.html

================================================================================
来源：http://hz.yj20258888.top/gtfovhgnma.html

C. 函数与作用域
来源：http://hz.wangdashe.top/gtbjkqqckx.html

================================================================================
来源：http://hz.havefunace.top/gtmdbzbvao.html

[C01] 定义函数
来源：http://hz.guannengcc.top/gtmtyypnnv.html

Py:   def add(a, b): return a + b
来源：http://hz.xinyue.icu/gtbxhigrlz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgfzy.top/gtywqkteho.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtxceauhzz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pycfn.com/gtlcszarmu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.dianchejie.cn/gtddrsdyau.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yvedp.cn/gtnqrwnvfl.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xinyue.icu/gtyithvtei.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gtscaqybdh.html

[C02] 默认参数
来源：http://hz.daxiang520.top/gtksucxhoj.html

Py:   def greet(name="World"): return name
来源：http://hz.kuanghao11.cn/gteyuobkhl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.316326.xyz/gtassihgzv.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shanyushiyangtech.top/gtrsdnnhrs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.dianchejie.cn/gtlgqkgkun.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.dashuyun.cn/gtsvwgmbsb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.birdmap.top/gtrpcskfmc.html

Ruby: def greet(name = "World") = name
来源：http://hz.nanxuanxn.top/gtfixeneim.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cdnleiting.top/gtxkybcyre.html

[C03] 可变参数
来源：http://hz.zhaomingkeji.xyz/gtqlkayckg.html

Py:   def total(*args): return sum(args)
来源：http://hz.yuanzhike.top/gtfhlclupv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yj20258.top/gtewzxjnjd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangkeji.top/gtqjyymohg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.vqdsnc.cn/gtwhpvlmsf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.daria6918.cn/gtmzvfoyoi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hysaishi.cn/gtxssdgdcz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xuetiantiany.cn/gthucaqtti.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ydjk.org.cn/gttfhwckmp.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sufxvd.cn/gtkfvbldwp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.aizwys.cn/gtydxovore.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xziqi.cn/gtjrlvtluc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtmylpxjjp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hysaishi.cn/gtajqzrzvn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.tanke756.top/gtgjkxubze.html

Go:   // 无：用配置结构体参数
来源：http://hz.mhx1999.top/gtevlasulw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ehwqpu.com/gtlhraemol.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinqigufen.top/gtupettmfj.html

[C05] 返回多个值
来源：http://hz.jinghuilouyu.cn/gttnllzdtk.html

Py:   return a, b
来源：http://hz.sweek.top/gtqmrtvimr.html

PHP:  return [$a, $b];
来源：http://hz.jinqigfzy.top/gttkpptmzr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gzhubu.top/gtepfbqeau.html

TS:   return { a, b };
来源：http://hz.ppjwa.cn/gtzoambkii.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhiwuduotai.top/gttinarmct.html

Go:   return a, b
来源：http://hz.hammf.cn/gtpkutfukt.html

Ruby: return a, b
来源：http://hz.daxiang520.top/gtrbswhmiv.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sysykeji.top/gtynuginef.html

[C06] 匿名函数 / lambda
来源：http://hz.meibo888.top/gtvdiewapw.html

Py:   square = lambda x: x * x
来源：http://hz.snrcjt.cn/gtmqfwclqm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhijiandao.cn/gtdcwirzed.html

JS:   const square = x => x * x;
来源：http://hz.jlsjyb.cn/gtrzlymhyv.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.316326.xyz/gtenmeurfb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.havefunace.top/gtxgiuffkz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.chenzaomai.com/gtnrxjzzgi.html

Ruby: square = ->(x) { x * x }
来源：http://hz.aizwys.cn/gtxszrndzh.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cucudq.cn/gtspnmenca.html

[C07] 把函数作为参数传入
来源：http://hz.aibaodan.cn/gtmlnzblkp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.kuanghao11.cn/gtoahmjvrh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gogol.net.cn/gtigrwyfgd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.c1oappe.top/gtifnqwijd.html

TS:   arr.map(String)
来源：http://hz.xingfuxueyuan.xyz/gtggtcwyxt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yongpay.top/gtjkkioyma.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hywenlv.cn/gtvifxepmr.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhoulong.xyz/gtbujpdtra.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ydjk.org.cn/gtoguyjmkd.html

[C08] 闭包
来源：http://hz.wangdashe.top/gtoaxdurch.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.wangdashe.top/gtzedagszb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cucudq.cn/gtetbnrjpp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.wangdashe.top/gtngldyrgl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtuqezngqh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jianghu66.top/gtaqbasfpb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.quarkkingdee.top/gtiglhjdax.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sufxvd.cn/gttpidwivc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shangyingyoupin.top/gtdccxcjrn.html

[C09] 递归
来源：http://hz.jqgfzy.top/gtcmgrgmlb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jianghu66.top/gtnmdwmrjq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.9152youxi.cn/gttgcgtmur.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nwbrower.top/gtbagypdtf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.havefunace.top/gtoavqlmts.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenjidiqi.icu/gtknkpzije.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.meibo888.top/gtcxwqcphu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhiwuduotai.top/gtfgdkzbif.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cqqwz.cn/gtuslwzzse.html

[C10] 变量作用域
来源：http://hz.c1oappe.top/gtzawmapcb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.316326.xyz/gtfzmfevsa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tianlin.xyz/gtcjsotini.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.fzhhl.top/gtekcggysa.html

TS:   同 JS
来源：http://hz.xuetiantiany.cn/gtsmofjnqh.html

Java: 方法内为块级作用域
来源：http://hz.ywan-chungtsiang.top/gtayagrtlg.html

Go:   花括号块级作用域
来源：http://hz.gogol.net.cn/gterldsylm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhiwuduotai.top/gtvycmbvob.html

C#:   块级作用域
来源：http://hz.yj20258.top/gtpxodivah.html

[C11] 模块导入与导出
来源：http://hz.yueranfly.top/gtyfjzywyb.html

Py:   from module import func
来源：http://hz.sweek.top/gttzdqhzux.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cucudq.cn/gtsgbqrpxr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cdnleiting.top/gtijunojlw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shanyushiyangtech.top/gtzjadmxud.html

Java: import java.util.List;
来源：http://hz.hysaishi.cn/gttbapequh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.fengsongda.top/gtramvfhgd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.mhx1999.top/gtzpyylyis.html

C#:   using System.Text;
来源：http://hz.hysaishi.cn/gtvzidhnkf.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenzaomai.com/gtytuqewor.html

Py:   (lambda: print("run"))()
来源：http://hz.yuxming.cn/gtzizqvjko.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ybcxt.top/gtgvbfvysk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.iojbl.cn/gtgbulrmkx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hfpthk.cn/gtbewmytpz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgfzy.top/gtzzydeaec.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nwbrower.top/gtlxxwxrfw.html

Ruby: -> { puts "run" }.call
来源：http://hz.fzhhl.top/gtwpsuvtjx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shanyushiyangtech.top/gtdbwupwov.html

[C13] 类型声明 / 类型注解
来源：http://hz.mhx1999.top/gtxtiyplhy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sweek.top/gtluoilywx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhoulong.xyz/gtalygmnns.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.birdmap.top/gtgkpxcagw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guowangkeji.top/gtchzzlsam.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.mhx1999.top/gtztlzsdqk.html

Go:   func add(a, b int) int
来源：http://hz.zycfv.cn/gtglovptmh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yj20258888.top/gtagcrbvbb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenlongwang.top/gtpwytrrve.html

[C14] 泛型函数
来源：http://hz.wangdashe.top/gtvkwdabyz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cashguo.top/gtyprprbtc.html

PHP:  // 无泛型
来源：http://hz.yueranfly.top/gtcmifissc.html

JS:   // 无泛型
来源：http://hz.9152youxi.cn/gtleuhzofk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yj202588.top/gtvnjyadgo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangshuangyany.cn/gtfiqivlum.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shanyushiyangkeji.top/gtiicqdlwp.html

Ruby: # 无泛型
来源：http://hz.cashguo.top/gtmheaklqe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuxming.cn/gtjvbpeton.html

[C15] 解构 / 展开参数
来源：http://hz.xuanzx.com/gtnxaftpnd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tianlin.xyz/gtrifarolm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shuidangran.top/gtrkwsrict.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.mhx1999.top/gtmbswglyx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.wangshuangyany.cn/gtjtrwrteg.html

Java: // 无解构
来源：http://hz.dashuyun.cn/gtwuczgxzw.html

Go:   // 无解构
来源：http://hz.wangdashe.top/gtqisdpyay.html

Ruby: a, b = pair
来源：http://hz.cucudq.cn/gtrnqsyzow.html

C#:   var (a, b) = pair;
来源：http://hz.jinqigfzy.top/gtjqabocto.html

[C16] 函数 / 方法重载
来源：http://hz.hammf.cn/gtdbgzfgaw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhijiandao.cn/gtvaxigmva.html

PHP:  // 无重载
来源：http://hz.9152youxi.cn/gtakulpqvb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ivvv.top/gtkasxseqj.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.birdmap.top/gtmlvjoblu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhixingplan.top/gtilxnwrra.html

Go:   // 无重载：用不同函数名
来源：http://hz.cashguo.top/gtgnjfsuum.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gzhubu.top/gtiqyizaxs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yueranfly.top/gtseyndnvq.html

================================================================================
来源：http://hz.dashuyun.cn/gttzuyneir.html

D. 数组 / 列表 / 集合
来源：http://hz.xuetiantiany.cn/gtajsewash.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtmlokoyuf.html

[D01] 创建数组 / 列表
来源：http://hz.cashguo.top/gthgdneets.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinghuilouyu.cn/gtkpxfbste.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yonumen.top/gtyifkztbg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hfpthk.cn/gtxeyibyiz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cqqwz.cn/gtybngketh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hammf.cn/gtbcwvollm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gogol.net.cn/gtqhdnrusm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jinqigfzy.top/gtdwqxpyhk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cdnleiting.top/gtonaoabyc.html

[D02] 追加元素到末尾
来源：http://hz.iojbl.cn/gtxljumefz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jlsjyb.cn/gtnhyuwyhz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhaomingkeji.xyz/gtttuhhujt.html

JS:   arr.push(4);
来源：http://hz.haohaochexian.top/gtgtkiyfob.html

TS:   arr.push(4);
来源：http://hz.xinyue.icu/gtajysbthv.html

Java: list.add(4);
来源：http://hz.wangdashe.top/gtbhqreklc.html

Go:   arr = append(arr, 4)
来源：http://hz.vqdsnc.cn/gtfsefgbhq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yuanzhike.top/gtnpebuegm.html

C#:   list.Add(4);
来源：http://hz.mhx1999.top/gtqqpltygh.html

[D03] 在指定位置插入元素
来源：http://hz.xingfuxueyuan.xyz/gtxaflnzwz.html

Py:   arr.insert(0, 0)
来源：http://hz.xingfuxueyuan.xyz/gtuwlbknqp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cqqwz.cn/gtqpkkxuew.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cashguo.top/gtcfmhhhdx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sysykeji.top/gtfdjyacrk.html

Java: list.add(0, 0);
来源：http://hz.vqdsnc.cn/gtgrjqyzpt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fengsongda.top/gtuiuurcjz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.havefunace.top/gtpvszrymz.html

C#:   list.Insert(0, 0);
来源：http://hz.jinyuanbaomall.cn/gtutuvkfek.html

[D04] 删除元素
来源：http://hz.shzxlz.cn/gtoziojsnc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shanyushiyangkeji.top/gtnppfgygi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.nwbrower.top/gtvcollvxx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gaohongyu789.top/gtjrbkdwxu.html

TS:   arr.splice(0, 1);
来源：http://hz.jiagoushi.top/gtcxnlkrxb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.redwolf501.top/gtoxtfrbeu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.chenlongwang.top/gtktcwvxju.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangkeji.top/gtmllkoduy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.daria6918.cn/gtckhbwrem.html

[D05] 访问与修改元素
来源：http://hz.sweek.top/gtvugneuqm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jyoumei.cn/gtbhnycrab.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cashguo.top/gtkfgfbaer.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sufxvd.cn/gtcobucomq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cdnleiting.top/gtvsusibhg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhoulong.xyz/gtetrgdbdf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.aibaodan.cn/gtrwofzeku.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuanzx.com/gtnqwpcity.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yvedp.cn/gtflssbkbs.html

[D06] 数组长度
来源：http://hz.xuetiantiany.cn/gteuyvgnvu.html

Py:   len(arr)
来源：http://hz.daxiang520.top/gtewgjcsvw.html

PHP:  count($arr);
来源：http://hz.shzxlz.cn/gtmiucqfns.html

JS:   arr.length
来源：http://hz.aizwys.cn/gtrzqkdkgg.html

TS:   arr.length
来源：http://hz.ehwqpu.com/gtiviovsry.html

Java: list.size();
来源：http://hz.cheryme.top/gtiasvfbfx.html

Go:   len(arr)
来源：http://hz.sweek.top/gtpcuhudls.html

Ruby: arr.length; arr.size
来源：http://hz.ivvv.top/gtmwaobotk.html

C#:   list.Count;
来源：http://hz.zhiwuduotai.top/gtfenmeftr.html

[D07] 切片 / 取子数组
来源：http://hz.jyoumei.cn/gtalmtggnw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.smart0.xyz/gtastwftqa.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sufxvd.cn/gtkuaotkeq.html

JS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtebpciyyc.html

TS:   arr.slice(1, 4);
来源：http://hz.shangyingyoupin.top/gtdccrvbtx.html

Java: list.subList(1, 4);
来源：http://hz.svipenyu.cn/gtmmicerlo.html

Go:   arr[1:4]
来源：http://hz.9152youxi.cn/gtcqxjxqhs.html

Ruby: arr[1, 3]
来源：http://hz.jqgfzy.top/gtlthenvjz.html

C#:   list.GetRange(1, 3);
来源：http://hz.smart0.xyz/gtqzrcxmkg.html

[D08] 合并两个数组
来源：http://hz.aizwys.cn/gtudamcvrv.html

Py:   a + b;  a.extend(b)
来源：http://hz.cheryme.top/gtkzvravxp.html

PHP:  array_merge($a, $b);
来源：http://hz.xuetiantiany.cn/gtfuscpzms.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.wangdashe.top/gtzpnxwmat.html

TS:   [...a, ...b];
来源：http://hz.yj20258888.top/gtylyygeto.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.pengpengdd.cyou/gtaujpqxbd.html

Go:   append(a, b...)
来源：http://hz.shzxlz.cn/gtmrkbupmb.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yonumen.top/gttylwltak.html

C#:   a.Concat(b).ToList()
来源：http://hz.yuxming.cn/gtgfafmujh.html

[D09] 排序（升序）
来源：http://hz.jlsjyb.cn/gtjvyvxisk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtceppwpsf.html

PHP:  sort($arr);
来源：http://hz.meibo888.top/gtkoijjwvt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.fzhhl.top/gtknuogttw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.52xcode.cn/gtvalzgpox.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yangfankeji.com/gtsjoxaezi.html


<!-- 参考信息 -->