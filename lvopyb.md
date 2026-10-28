代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://hz.iojbl.cn/gtvkppkvgw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ybcxt.top/gtlilrhzfr.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jyoumei.cn/gtktecqosp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.tanke756.top/gtrejmywsu.html

[B09] break 与 continue
来源：http://hz.0kj1m.cn/gtunovqtrc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ydjk.org.cn/gtbsllgzfa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.tian-w.cn/gtqwiuiekj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nwbrower.top/gtbmanfdqw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhoulong.xyz/gtyesqilkv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtznaeezyq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.wangdashe.top/gtdgmppdag.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.fengsongda.top/gtbwzauhhv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yanxiufei.cn/gtxdntccmu.html

[B10] 遍历同时拿索引
来源：http://hz.sxryk.cn/gtcsifmnam.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.daxiang520.top/gtejotonia.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gaohongyu789.top/gtcqtsxnss.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.guannengcc.top/gtjncoojdt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zycfv.cn/gthsbixqgt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.redwolf501.top/gtxfqnmxqo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.aibaodan.cn/gtebfgmiex.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cashguo.top/gtyeipdayu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.nanxinkj.top/gtdsgfdlgb.html

[B11] 生成数字序列 / 区间
来源：http://hz.zdqjudy.top/gttmrvwqpm.html

Py:   list(range(0, 10, 2))
来源：http://hz.snrcjt.cn/gtugtftilz.html

PHP:  range(0, 10, 2);
来源：http://hz.yj20258888.top/gtndvockzh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xylfe.cn/gtijfydmqj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guowangkeji.top/gtizuetyqx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinyuanbaomall.cn/gtsqugsohj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.nanxinkj.top/gtgzfyvdaq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shangyingyoupin.top/gtslatvzzv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinghuilouyu.cn/gtdlfmbsmz.html

[B12] 跳出多层循环
来源：http://hz.xinyue.icu/gtolxdorue.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhengqikj.top/gtswalnvvy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.gzhubu.top/gtogmzusqx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hywenlv.cn/gtihmxvwxe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hongshengwenyu.top/gtnrdedaad.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ivvv.top/gtdrzvvtrn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jlsjyb.cn/gtwcmeqgkd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.52xcode.cn/gtkmasuwaz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shzxlz.cn/gtfciiveun.html

[B13] 判断是否为数字
来源：http://hz.pycfn.com/gtiexjchfn.html

Py:   isinstance(x, (int, float))
来源：http://hz.xuetiantiany.cn/gtltoaqqib.html

PHP:  is_numeric($x)
来源：http://hz.sysykeji.top/gtaagpeugk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xingfuxueyuan.xyz/gtuftjmczf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gaohongyu789.top/gtvdjuxmpo.html

Java: x instanceof Number
来源：http://hz.ywan-chungtsiang.top/gtogstkiqp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.guowangkeji.top/gtvaefkmsy.html

Ruby: x.is_a?(Numeric)
来源：http://hz.pengpengdd.cyou/gtbrfiugzj.html

C#:   x is int or double or decimal
来源：http://hz.sufxvd.cn/gtcdbyusux.html

[B14] 判断值是否在集合内
来源：http://hz.yongpay.top/gtdbzocjkm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jianghu66.top/gtsndjtrqy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ppjwa.cn/gthzoixfdd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gtdywnxzyn.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.smart0.xyz/gtserthzfd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tanke756.top/gtihvucrrd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.tian-w.cn/gterucdzmh.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xingfuxueyuan.xyz/gtzzuyxlzg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.iojbl.cn/gtsxrlzjjo.html

[B15] 布尔运算与取反
来源：http://hz.cdnleiting.top/gttotcfphr.html

Py:   a and b or not c
来源：http://hz.ybcxt.top/gttuyxczwn.html

PHP:  $a && $b || !$c
来源：http://hz.wangshuangyany.cn/gthokqyraf.html

JS:   a && b || !c
来源：http://hz.xziqi.cn/gthnatrbdb.html

TS:   a && b || !c
来源：http://hz.svipenyu.cn/gtmvmrrsde.html

Java: a && b || !c
来源：http://hz.shzxlz.cn/gtxsghszlj.html

Go:   a && b || !c
来源：http://hz.zhiwuduotai.top/gtbesyeple.html

Ruby: a && b || !c
来源：http://hz.jlsjyb.cn/gtgwelpbik.html

C#:   a && b || !c
来源：http://hz.ybcxt.top/gtnpbbjtoe.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yj20258.top/gtgmibjnth.html

Py:   if not data: return
来源：http://hz.smart0.xyz/gtxtyrekej.html

PHP:  if (!$data) { return; }
来源：http://hz.yanxiufei.cn/gtssewpxqi.html

JS:   if (!data) return;
来源：http://hz.cucudq.cn/gtrjvsvxqw.html

TS:   if (!data) return;
来源：http://hz.kuanghao11.cn/gtkioaxidq.html

Java: if (data == null) return;
来源：http://hz.yj202588.top/gtprjsrilr.html

Go:   if data == nil { return }
来源：http://hz.wangdashe.top/gtpmyzlgiz.html

Ruby: return if data.nil?
来源：http://hz.iojbl.cn/gtprgyemtq.html

C#:   if (data == null) return;
来源：http://hz.kuanghao11.cn/gtynyqleyc.html

================================================================================
来源：http://hz.jiagoushi.top/gtcnbinvlz.html

C. 函数与作用域
来源：http://hz.hywenlv.cn/gtwcipcwce.html

================================================================================
来源：http://hz.yvedp.cn/gtjtcqzwbr.html

[C01] 定义函数
来源：http://hz.yongpay.top/gtkjhqltep.html

Py:   def add(a, b): return a + b
来源：http://hz.yueranfly.top/gtvjlfxtxb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yonumen.top/gthplnqcpz.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yj20258888.top/gtkbqrgzmt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.c1oappe.top/gtcztpcnkg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yonumen.top/gtfqnfaeld.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.chenlongwang.top/gtyvnvpntp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.wangshuangyany.cn/gtiwomjlbw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cucudq.cn/gtiggeclig.html

[C02] 默认参数
来源：http://hz.snrcjt.cn/gthujnafxm.html

Py:   def greet(name="World"): return name
来源：http://hz.chenzaomai.com/gtilcvnewg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jianghu66.top/gtxetfziss.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinghuilouyu.cn/gtubhtlqof.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xuanzx.com/gtiizzhzvs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hysaishi.cn/gtoychmxjy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xziqi.cn/gtcuvfgegq.html

Ruby: def greet(name = "World") = name
来源：http://hz.0kj1m.cn/gtxxiljvxu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.guowangkeji.top/gthjbwuqzl.html

[C03] 可变参数
来源：http://hz.iojbl.cn/gtpzuivbwc.html

Py:   def total(*args): return sum(args)
来源：http://hz.aibaodan.cn/gtvinwanya.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hnqzz.top/gtouabmqdk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinqigfzy.top/gtxttqodqp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.meibo888.top/gteqqiqnnm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.nwbrower.top/gtmfoxaswo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.pengpengdd.cyou/gtoqdwrzzn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zdqjudy.top/gtfjbveorf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shzxlz.cn/gtmdkyndvl.html

[C04] 命名参数 / 关键字参数
来源：http://hz.svipenyu.cn/gteloufkav.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yj20258.top/gtywafimnv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenzaomai.com/gtwagskjjp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.chenlongwang.top/gthtlvahth.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.guannengcc.top/gtqrbfytbg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.fengsongda.top/gtstizfide.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhaomingkeji.xyz/gtisdlxcub.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhaomingkeji.xyz/gtltkccpyq.html

C#:   f(a: 1, b: 2)
来源：http://hz.nwbrower.top/gtjupjzzsd.html

[C05] 返回多个值
来源：http://hz.jqgufenzy.top/gtpdlcnbaa.html

Py:   return a, b
来源：http://hz.nanxuanxn.top/gtqahxtgyk.html

PHP:  return [$a, $b];
来源：http://hz.chenjidiqi.icu/gtrtqfsxdc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ydzc1.top/gtxepurxld.html

TS:   return { a, b };
来源：http://hz.xylfe.cn/gtmlxnymdv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhaomingkeji.xyz/gtubnnyqdn.html

Go:   return a, b
来源：http://hz.yuxming.cn/gtjhtqfyjy.html

Ruby: return a, b
来源：http://hz.chenzaomai.com/gtefuxwfzl.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sxryk.cn/gtsergwjfy.html

[C06] 匿名函数 / lambda
来源：http://hz.jqgufenzy.top/gtaoawkdab.html

Py:   square = lambda x: x * x
来源：http://hz.yueranfly.top/gtvfpiyxsw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yuanzhike.top/gtkkvzbwvn.html

JS:   const square = x => x * x;
来源：http://hz.zhixingplan.top/gtdcztkcix.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.daria6918.cn/gtlioqdbhv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.bjfxy.top/gttwfhmjoy.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.bjfxy.top/gtwuolyfqb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.snrcjt.cn/gtcepyzdsx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj202588.top/gtfrzigzbm.html

[C07] 把函数作为参数传入
来源：http://hz.hysaishi.cn/gtswlaowst.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shzxlz.cn/gtdgmywdob.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.feifeiyinyue.top/gtazendeaf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.nwbrower.top/gtarxqmful.html

TS:   arr.map(String)
来源：http://hz.hnqzz.top/gtnrplsvve.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shangyingyoupin.top/gtejzjkfhp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cqqwz.cn/gtlgczmlfe.html

Ruby: arr.map(&:upcase)
来源：http://hz.aibaodan.cn/gtlkzcbhsz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yonumen.top/gtrhkssvtx.html

[C08] 闭包
来源：http://hz.nanxinkj.top/gtmkfqihiy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ybcxt.top/gtkccvvluh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.quarkkingdee.top/gtwdpbywap.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinqigfzy.top/gtljyggyaj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hammf.cn/gtxvapkqxf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cqqwz.cn/gtdbximcxx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hysaishi.cn/gtjawaogsy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.meibo888.top/gteashinug.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.svipenyu.cn/gtsgnflulc.html

[C09] 递归
来源：http://hz.cdnleiting.top/gtdiwamjux.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xziqi.cn/gtobxbipym.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.vqdsnc.cn/gtgdyutoyh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.mhx1999.top/gtwrfqbgem.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.316326.xyz/gtuimmxcaw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.52xcode.cn/gtwxgjignw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xziqi.cn/gthuyahcfy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.0kj1m.cn/gtxbyutmfm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jqgufenzy.top/gtqemcnmdl.html

[C10] 变量作用域
来源：http://hz.guowangkeji.top/gtxilfhrax.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aizwys.cn/gtaaotvyfp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hongshengwenyu.top/gtjwzblrui.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinghuilouyu.cn/gtjouecazj.html

TS:   同 JS
来源：http://hz.zhaomingkeji.xyz/gtrnazyhxs.html

Java: 方法内为块级作用域
来源：http://hz.chenjidiqi.icu/gtasshponb.html

Go:   花括号块级作用域
来源：http://hz.jiagoushi.top/gtdnakzwfu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yanxiufei.cn/gtzhkfbbvn.html

C#:   块级作用域
来源：http://hz.zhijiandao.cn/gtxuopfqms.html

[C11] 模块导入与导出
来源：http://hz.yangfankeji.com/gtabeiylnm.html

Py:   from module import func
来源：http://hz.snrcjt.cn/gtcskccnpj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.meibo888.top/gtesgtqigp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shzxlz.cn/gtwrmxpnzf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xuetiantiany.cn/gtuhziutkd.html

Java: import java.util.List;
来源：http://hz.cdnleiting.top/gtojhjyame.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.redwolf501.top/gtuvskhgbz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ivvv.top/gtufncupul.html

C#:   using System.Text;
来源：http://hz.dianchejie.cn/gtxgghptyz.html

[C12] 立即执行函数 IIFE
来源：http://hz.nanxuanxn.top/gtigbeewyr.html

Py:   (lambda: print("run"))()
来源：http://hz.feifeiyinyue.top/gtiqaboson.html

PHP:  (function () { echo "run"; })();
来源：http://hz.gzhubu.top/gtnedfoxgd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gtalpvsoap.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hongshengwenyu.top/gtfbvfuqam.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ehwqpu.com/gtmurgpapu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.9152youxi.cn/gtbgqpbsfw.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhongyouzk.top/gtyfdivfqy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yuanzhike.top/gtytczakgy.html

[C13] 类型声明 / 类型注解
来源：http://hz.cashguo.top/gtwqstpgxf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guowangkeji.top/gtozobqrum.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.birdmap.top/gtclxpjlpy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shanyushiyangtech.top/gtipqkxdrm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.quarkkingdee.top/gtrpteozub.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xziqi.cn/gtkztpqinc.html

Go:   func add(a, b int) int
来源：http://hz.shangyingyoupin.top/gtdajwdoud.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.aibaodan.cn/gtwvfizlmq.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yuanzhike.top/gtsnmggrly.html

[C14] 泛型函数
来源：http://hz.fzhhl.top/gtvuvqyscm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xziqi.cn/gtcgftvprd.html

PHP:  // 无泛型
来源：http://hz.andypj.xyz/gtdtgfhgcf.html

JS:   // 无泛型
来源：http://hz.jqgufenzy.top/gtvlbcqibj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhongyouzk.top/gthgsypqkh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinghuilouyu.cn/gtybkfnlwk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yuanzhike.top/gtwwbbytdr.html

Ruby: # 无泛型
来源：http://hz.xinyue.icu/gtdnavcqdz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.haohaochexian.top/gtxhtafljs.html

[C15] 解构 / 展开参数
来源：http://hz.xziqi.cn/gtiiulvqci.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sufxvd.cn/gtwzvznpnj.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yvedp.cn/gtqokqonwm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxuanxn.top/gtsziosqhi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hnxiangtu.top/gtgepfdxug.html

Java: // 无解构
来源：http://hz.hywenlv.cn/gthfdovfup.html

Go:   // 无解构
来源：http://hz.svipenyu.cn/gtdusyqpzz.html

Ruby: a, b = pair
来源：http://hz.jqgfzy.top/gtiayictru.html

C#:   var (a, b) = pair;
来源：http://hz.haohaochexian.top/gtcekkvodg.html

[C16] 函数 / 方法重载
来源：http://hz.tianlin.xyz/gtfknwvbxd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhixingplan.top/gtttpvlqwg.html

PHP:  // 无重载
来源：http://hz.svipenyu.cn/gtuakrznzf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xziqi.cn/gtetucqcee.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yueranfly.top/gtbvtdrtgy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.guowangkeji.top/gtcxhvtdud.html

Go:   // 无重载：用不同函数名
来源：http://hz.pycfn.com/gthpxyyore.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gotoacloud.top/gttyhanhvo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinyuanbaomall.cn/gtlgfmhnsi.html

================================================================================
来源：http://hz.wangdashe.top/gtjdfsphng.html

D. 数组 / 列表 / 集合
来源：http://hz.feifeiyinyue.top/gtmipimvxd.html

================================================================================
来源：http://hz.xuanzx.com/gtwnnmhqqc.html

[D01] 创建数组 / 列表
来源：http://hz.jinqigfzy.top/gthgkrerpr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xuetiantiany.cn/gtoamsfjld.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sxryk.cn/gtwixkpafp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gotoacloud.top/gtmibnywcv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.redwolf501.top/gttzhjnwvf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.meibo888.top/gtbpftgxuf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ehwqpu.com/gtzxdmqxsi.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sweek.top/gtwvqepyku.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.guannengcc.top/gtiernvvkp.html

[D02] 追加元素到末尾
来源：http://hz.jinqigfzy.top/gtbtbjgpgz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gaohongyu789.top/gtzeqfucge.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.fengsongda.top/gtvbhaehik.html

JS:   arr.push(4);
来源：http://hz.svipenyu.cn/gtsprytkun.html

TS:   arr.push(4);
来源：http://hz.sxryk.cn/gttjgewwjn.html

Java: list.add(4);
来源：http://hz.guannengcc.top/gtiuyaoojz.html

Go:   arr = append(arr, 4)
来源：http://hz.gogol.net.cn/gtfwgyawta.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gaohongyu789.top/gtjnsbgoff.html

C#:   list.Add(4);
来源：http://hz.gaohongyu789.top/gtzkcybfit.html

[D03] 在指定位置插入元素
来源：http://hz.shuidangran.top/gtqookrajh.html

Py:   arr.insert(0, 0)
来源：http://hz.xuetiantiany.cn/gtceacguwz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zdqjudy.top/gtijevdwwv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.daria6918.cn/gtcjdshdxm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.redwolf501.top/gtngfjnydt.html

Java: list.add(0, 0);
来源：http://hz.jqgufenzy.top/gttpsuxdfc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinqigfzy.top/gtgsokpsia.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jqgufenzy.top/gtecxyoupf.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxuanxn.top/gtmkstjuuv.html

[D04] 删除元素
来源：http://hz.yanxiufei.cn/gtutgukymf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinqigfzy.top/gtfbixujki.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.dianchejie.cn/gtwgkufhde.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.wangdashe.top/gtgsknmrfu.html

TS:   arr.splice(0, 1);
来源：http://hz.0kj1m.cn/gtjdbghgbt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yonumen.top/gtnrsewzbn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.daxiang520.top/gtvhgidsfm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.0kj1m.cn/gtwzpnhght.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cdnleiting.top/gtgknnlwur.html

[D05] 访问与修改元素
来源：http://hz.jinyuanbaomall.cn/gtnpevhbfm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtdtzkuefe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj20258888.top/gtlequdeod.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.haohaochexian.top/gtfjfwbhps.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ehwqpu.com/gtrsilzgdz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gogol.net.cn/gtksglqeou.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.andypj.xyz/gtbpisatzj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtwqomxxer.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ywan-chungtsiang.top/gtigvgmujw.html

[D06] 数组长度
来源：http://hz.svipenyu.cn/gtjlhsrnqp.html

Py:   len(arr)
来源：http://hz.jqgfzy.top/gtkkgcuuvp.html

PHP:  count($arr);
来源：http://hz.pengpengdd.cyou/gtieruzdqt.html

JS:   arr.length
来源：http://hz.xylfe.cn/gtmlfvbqly.html

TS:   arr.length
来源：http://hz.jinyuanbaomall.cn/gtqumckspg.html

Java: list.size();
来源：http://hz.jyoumei.cn/gtqmwziqzr.html

Go:   len(arr)
来源：http://hz.shanyushiyangtech.top/gtunotxzuo.html

Ruby: arr.length; arr.size
来源：http://hz.hnqzz.top/gtpnjwsobt.html

C#:   list.Count;
来源：http://hz.hnxiangtu.top/gtjfqwsydj.html

[D07] 切片 / 取子数组
来源：http://hz.redwolf501.top/gtqeficswa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.mhx1999.top/gtypzoitln.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gogol.net.cn/gtvpznrltt.html

JS:   arr.slice(1, 4);
来源：http://hz.nwbrower.top/gtjgncfhtg.html

TS:   arr.slice(1, 4);
来源：http://hz.shangyingyoupin.top/gtctfnrkjg.html

Java: list.subList(1, 4);
来源：http://hz.zhoulong.xyz/gtthiliefg.html

Go:   arr[1:4]
来源：http://hz.shanyushiyangkeji.top/gtsauvgdkw.html

Ruby: arr[1, 3]
来源：http://hz.gogol.net.cn/gtjihlhcok.html

C#:   list.GetRange(1, 3);
来源：http://hz.xingfuxueyuan.xyz/gtnyboztna.html

[D08] 合并两个数组
来源：http://hz.sxryk.cn/gtzegybugg.html

Py:   a + b;  a.extend(b)
来源：http://hz.pengpengdd.cyou/gtqpqwjfss.html

PHP:  array_merge($a, $b);
来源：http://hz.xylfe.cn/gtooaqwcxg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ydjk.org.cn/gtpyysrqmx.html

TS:   [...a, ...b];
来源：http://hz.cdnleiting.top/gtgzeoghrp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cheryme.top/gtzsbbudpj.html

Go:   append(a, b...)
来源：http://hz.guannengcc.top/gtgrebiubu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ywan-chungtsiang.top/gtckuoxcmf.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinghuilouyu.cn/gtohsbzhhv.html

[D09] 排序（升序）
来源：http://hz.jqgfzy.top/gttyftadpw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinyuanbaomall.cn/gtiwjnbkfr.html


<!-- 参考信息 -->