代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.tanke756.top/gtzjghglag.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yonumen.top/gtrdyfffge.html

C#:   while (i < 10) { i++; }
来源：http://hz.ybcxt.top/gtklhubwrb.html

[B08] do-while（至少执行一次）
来源：http://hz.jianghu66.top/gtqilclogg.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jianghu66.top/gtlttalgtt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.xuetiantiany.cn/gtaximycwn.html

JS:   do { i++; } while (i < 10);
来源：http://hz.shzxlz.cn/gttmokonwk.html

TS:   do { i++; } while (i < 10);
来源：http://hz.feifeiyinyue.top/gtzatterfq.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhiwuduotai.top/gtkhsyfqfm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.guannengcc.top/gtztyejbgh.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hysaishi.cn/gtxhenhesu.html

C#:   do { i++; } while (i < 10);
来源：http://hz.guowangkeji.top/gtqktnsnla.html

[B09] break 与 continue
来源：http://hz.yangfankeji.com/gtjavdgrah.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.c1oappe.top/gthcaximuh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hnxiangtu.top/gtvxnwpdhu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtthuzhbya.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhixingplan.top/gtzhybuzpl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yongpay.top/gtksnlteqj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ywan-chungtsiang.top/gtuovqpbrg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.nwbrower.top/gtxiqtsndw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhongyouzk.top/gtnrcbkjyk.html

[B10] 遍历同时拿索引
来源：http://hz.shanyushiyangtech.top/gtmzsrmhea.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.chenlongwang.top/gtbuwlwdvo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhaomingkeji.xyz/gttneazxbp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zycfv.cn/gtdymxwlxa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.andypj.xyz/gtolxravte.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.mhx1999.top/gtquegqvqx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.pengpengdd.cyou/gtxnrfdmal.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jinqigufen.top/gttgzwoytj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shanyushiyangtech.top/gtyxbaetkh.html

[B11] 生成数字序列 / 区间
来源：http://hz.yuanzhike.top/gtvfnfkvvl.html

Py:   list(range(0, 10, 2))
来源：http://hz.aizwys.cn/gtuetzxhny.html

PHP:  range(0, 10, 2);
来源：http://hz.shanyushiyangtech.top/gteyjsqiwj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangshuangyany.cn/gtdmzuouxo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jqgufenzy.top/gtakfwoofc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ehwqpu.com/gtrrtyygms.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jqgufenzy.top/gtofolrfrx.html

Ruby: (0...10).step(2).to_a
来源：http://hz.pycfn.com/gtuiyzoozs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.birdmap.top/gtrortkjpr.html

[B12] 跳出多层循环
来源：http://hz.9152youxi.cn/gtiqrzgfzy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yanxiufei.cn/gtjvgveusx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.52xcode.cn/gtuxonttul.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.snrcjt.cn/gtmrhhunoa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.vqdsnc.cn/gtshrkegtb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hysaishi.cn/gtjjwztdpy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hywenlv.cn/gtjzcrskat.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.pengpengdd.cyou/gtsozpqlnc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xylfe.cn/gtrxkldvhu.html

[B13] 判断是否为数字
来源：http://hz.vqdsnc.cn/gtfjhbsztw.html

Py:   isinstance(x, (int, float))
来源：http://hz.sweek.top/gtthoakqld.html

PHP:  is_numeric($x)
来源：http://hz.dashuyun.cn/gttongrudm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hnqzz.top/gtozydlrbb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yanxiufei.cn/gtgamkrhnm.html

Java: x instanceof Number
来源：http://hz.daxiang520.top/gtssheabfc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.svipenyu.cn/gtwqsaoolr.html

Ruby: x.is_a?(Numeric)
来源：http://hz.vqdsnc.cn/gtufliimdb.html

C#:   x is int or double or decimal
来源：http://hz.xziqi.cn/gttdgcpcrt.html

[B14] 判断值是否在集合内
来源：http://hz.cucudq.cn/gtkoladjjq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.daria6918.cn/gtkcscyddm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.9152youxi.cn/gtxfsaqivc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ivvv.top/gtnfhxyhoh.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.snrcjt.cn/gthwrutjax.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ivvv.top/gtixudyteg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.chenjidiqi.icu/gtvwnqjgsu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.nanxinkj.top/gtyyotwvuq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.0kj1m.cn/gtmgezbhkj.html

[B15] 布尔运算与取反
来源：http://hz.9152youxi.cn/gtpunkugww.html

Py:   a and b or not c
来源：http://hz.fzhhl.top/gtaaofotno.html

PHP:  $a && $b || !$c
来源：http://hz.jqgfzy.top/gtjjcrdxep.html

JS:   a && b || !c
来源：http://hz.hfpthk.cn/gtzwzqyzwt.html

TS:   a && b || !c
来源：http://hz.havefunace.top/gtnyedacmm.html

Java: a && b || !c
来源：http://hz.cdnleiting.top/gtafqehedm.html

Go:   a && b || !c
来源：http://hz.sweek.top/gtndqrwztc.html

Ruby: a && b || !c
来源：http://hz.yj20258888.top/gtlqknuiqt.html

C#:   a && b || !c
来源：http://hz.pycfn.com/gtoonrlmxw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jqgufenzy.top/gtwcikhvbr.html

Py:   if not data: return
来源：http://hz.havefunace.top/gtjoczbltv.html

PHP:  if (!$data) { return; }
来源：http://hz.xuanzx.com/gtgurfaanu.html

JS:   if (!data) return;
来源：http://hz.gotoacloud.top/gtvyznfuim.html

TS:   if (!data) return;
来源：http://hz.yuanzhike.top/gtocpykvfu.html

Java: if (data == null) return;
来源：http://hz.shanyushiyangtech.top/gtfaqarutj.html

Go:   if data == nil { return }
来源：http://hz.cashguo.top/gtgvgacbjk.html

Ruby: return if data.nil?
来源：http://hz.tian-w.cn/gtgrkwlhog.html

C#:   if (data == null) return;
来源：http://hz.hnxiangtu.top/gthyhjaeib.html

================================================================================
来源：http://hz.daria6918.cn/gtiilclwim.html

C. 函数与作用域
来源：http://hz.nanxinkj.top/gtzlppdjsc.html

================================================================================
来源：http://hz.haohaochexian.top/gtyfvnokdt.html

[C01] 定义函数
来源：http://hz.cheryme.top/gthobdyvjr.html

Py:   def add(a, b): return a + b
来源：http://hz.jinqigfzy.top/gtuwzegena.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtdyawlzby.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yonumen.top/gtxkczampk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fzhhl.top/gtnrcpwpmr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.havefunace.top/gtqeiurapl.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xingfuxueyuan.xyz/gtdsaxrepd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gzhubu.top/gthjaigkmb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gttfzvdunl.html

[C02] 默认参数
来源：http://hz.shzxlz.cn/gtcqokwxwg.html

Py:   def greet(name="World"): return name
来源：http://hz.sysykeji.top/gtqorcqvbw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinqigfzy.top/gtmfguuylh.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cashguo.top/gtdvxfvawc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.wangdashe.top/gttkvuwhhn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhengqikj.top/gtrnvyddrf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhiwuduotai.top/gtopbkwgbh.html

Ruby: def greet(name = "World") = name
来源：http://hz.bjfxy.top/gtbxcxgoqx.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xuetiantiany.cn/gtgkshkqjt.html

[C03] 可变参数
来源：http://hz.yvedp.cn/gtvvzyzpao.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhixingplan.top/gtkskhruvp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.9152youxi.cn/gtfzhrgzxo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.meibo888.top/gtdftrbbpy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.bjfxy.top/gtckqkjmmu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.fzhhl.top/gtbbysguka.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.quarkkingdee.top/gtzbnoafjq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.guannengcc.top/gtowwhbagg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.sysykeji.top/gtyxamckkl.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cashguo.top/gtszxetqzy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhengqikj.top/gtdofsuwbd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenjidiqi.icu/gtwdvvgpde.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ydzc1.top/gtgkwjnsfk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.birdmap.top/gtxblizoot.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.aibaodan.cn/gtrjsmwqyk.html

Go:   // 无：用配置结构体参数
来源：http://hz.jlsjyb.cn/gtaexlugfr.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xingfuxueyuan.xyz/gtppvyzzdv.html

C#:   f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtyajgdbfx.html

[C05] 返回多个值
来源：http://hz.wangdashe.top/gtmxdxvvpw.html

Py:   return a, b
来源：http://hz.nanxuanxn.top/gtltxltfmz.html

PHP:  return [$a, $b];
来源：http://hz.hongshengwenyu.top/gtzszgpzcg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jiagoushi.top/gtdaqrvvyc.html

TS:   return { a, b };
来源：http://hz.cqqwz.cn/gteprgzjgc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ywan-chungtsiang.top/gttjfmcbfk.html

Go:   return a, b
来源：http://hz.jqgfzy.top/gtvywgxfak.html

Ruby: return a, b
来源：http://hz.wangdashe.top/gthrbsqcml.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hongshengwenyu.top/gtyiizrmlj.html

[C06] 匿名函数 / lambda
来源：http://hz.daxiang520.top/gtldndfjil.html

Py:   square = lambda x: x * x
来源：http://hz.jqgfzy.top/gtcievsaqg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.iojbl.cn/gtgofcobfu.html

JS:   const square = x => x * x;
来源：http://hz.dashuyun.cn/gtktzmtnfu.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hysaishi.cn/gtiqfplelq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yj202588.top/gtjulmhnei.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jiagoushi.top/gtcvwkrimr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.316326.xyz/gtcltcgjuo.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shanyushiyangkeji.top/gtzdpzbbah.html

[C07] 把函数作为参数传入
来源：http://hz.yuanzhike.top/gtsgcrfqva.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hywenlv.cn/gtzqxsoaju.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.smart0.xyz/gtljolwukf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hongshengwenyu.top/gtvguxotou.html

TS:   arr.map(String)
来源：http://hz.gaohongyu789.top/gtdzihyhim.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.tanke756.top/gtsgkwwnmc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.aibaodan.cn/gtyksflpgp.html

Ruby: arr.map(&:upcase)
来源：http://hz.cheryme.top/gtfgynwzbj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhaomingkeji.xyz/gtvnwmhgbm.html

[C08] 闭包
来源：http://hz.yj20258888.top/gtddlbhbqb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.nanxuanxn.top/gtaqwcnmpb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shangyingyoupin.top/gtjtoqltct.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.haohaochexian.top/gtievzjwjm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtjijrmtrw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.meibo888.top/gtonecakvt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shangyingyoupin.top/gtkhbcdgtt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.dianchejie.cn/gtwwcqwyro.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.wangdashe.top/gtvdxgvmkq.html

[C09] 递归
来源：http://hz.aibaodan.cn/gtznwaunbb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj20258888.top/gtnqajhqqy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.kuanghao11.cn/gtqlcsjcrd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigfzy.top/gtazbkvhzh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.kuanghao11.cn/gtolqaxcji.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.nwbrower.top/gtrixlpzfq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ehwqpu.com/gtrcngyrch.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinqigufen.top/gtedkluqbp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.guannengcc.top/gttwnxcvzy.html

[C10] 变量作用域
来源：http://hz.birdmap.top/gtwoyjiyxs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.iojbl.cn/gtwsfvsusf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yuanzhike.top/gtykfdsbgl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ywan-chungtsiang.top/gtmfxbxsyh.html

TS:   同 JS
来源：http://hz.ppjwa.cn/gteyvxjykc.html

Java: 方法内为块级作用域
来源：http://hz.bjfxy.top/gtnmciqkbt.html

Go:   花括号块级作用域
来源：http://hz.shanyushiyangtech.top/gtkcjgsloi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.shangyingyoupin.top/gtxpppjcxk.html

C#:   块级作用域
来源：http://hz.zdqjudy.top/gtzfywkqtc.html

[C11] 模块导入与导出
来源：http://hz.birdmap.top/gtbieefdne.html

Py:   from module import func
来源：http://hz.hnxiangtu.top/gtsdfdkzae.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.fzhhl.top/gtddxghyqz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jyoumei.cn/gtziqttkxl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.fengsongda.top/gtlzyuqyjj.html

Java: import java.util.List;
来源：http://hz.iojbl.cn/gtsbdmzlls.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigfzy.top/gtesnfmbfv.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinqigfzy.top/gtfyjgbpds.html

C#:   using System.Text;
来源：http://hz.yvedp.cn/gtshtwmzrl.html

[C12] 立即执行函数 IIFE
来源：http://hz.gotoacloud.top/gtsbylpyqd.html

Py:   (lambda: print("run"))()
来源：http://hz.shanyushiyangkeji.top/gttjxnkeqe.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nwbrower.top/gtbasoehfl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shangyingyoupin.top/gtxdoubbnz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gtkrhiqdws.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shuidangran.top/gtivfykydy.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jinqigfzy.top/gtyfcgrbpp.html

Ruby: -> { puts "run" }.call
来源：http://hz.hnxiangtu.top/gtbrpzzitq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.kuanghao11.cn/gtkbggidxq.html

[C13] 类型声明 / 类型注解
来源：http://hz.meibo888.top/gtrhgebjuk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ehwqpu.com/gtwsqdgvwe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhongyouzk.top/gtxigqkcrw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.c1oappe.top/gteuahpqwz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daxiang520.top/gtyvmqkqwd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.birdmap.top/gttccxwbca.html

Go:   func add(a, b int) int
来源：http://hz.yuxming.cn/gtinmwxshk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.tian-w.cn/gtignxswwk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.aizwys.cn/gtzwnynsqp.html

[C14] 泛型函数
来源：http://hz.snrcjt.cn/gthmayumkc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gtespwfmns.html

PHP:  // 无泛型
来源：http://hz.nanxuanxn.top/gttuzazckr.html

JS:   // 无泛型
来源：http://hz.ppjwa.cn/gtlhneknnv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhixingplan.top/gtxpqcxtkm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xziqi.cn/gtoehsfoyk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.daxiang520.top/gtktwmorbi.html

Ruby: # 无泛型
来源：http://hz.yvedp.cn/gtgipgckwk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhoulong.xyz/gtauvawvqq.html

[C15] 解构 / 展开参数
来源：http://hz.guannengcc.top/gtvhpyyecs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shanyushiyangtech.top/gtdiugafik.html

PHP:  [$a, $b] = $pair;
来源：http://hz.dianchejie.cn/gtcifrnkof.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xinyue.icu/gtkxpquwxc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.pengpengdd.cyou/gtogopdewq.html

Java: // 无解构
来源：http://hz.aibaodan.cn/gtjtergnkb.html

Go:   // 无解构
来源：http://hz.gotoacloud.top/gtryzncprn.html

Ruby: a, b = pair
来源：http://hz.redwolf501.top/gtsnjabqmq.html

C#:   var (a, b) = pair;
来源：http://hz.shuidangran.top/gtdleesccn.html

[C16] 函数 / 方法重载
来源：http://hz.pycfn.com/gttaroopfx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yanxiufei.cn/gtrpifconp.html

PHP:  // 无重载
来源：http://hz.316326.xyz/gtarartyem.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xuetiantiany.cn/gtucbpnozz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xylfe.cn/gtrkbulvwd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xuanzx.com/gtmyipreds.html

Go:   // 无重载：用不同函数名
来源：http://hz.haohaochexian.top/gtvxsobyop.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shzxlz.cn/gtzwoqgapd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hfpthk.cn/gtunnkauuz.html

================================================================================
来源：http://hz.ydzc1.top/gtxefdrrdg.html

D. 数组 / 列表 / 集合
来源：http://hz.cashguo.top/gtqvtyozxm.html

================================================================================
来源：http://hz.yj20258888.top/gthjbubjae.html

[D01] 创建数组 / 列表
来源：http://hz.jqgufenzy.top/gtjevjufku.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.bjfxy.top/gtaadridsw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.tian-w.cn/gtxjqhkhuo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.haohaochexian.top/gtbuskfxtm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.chenjidiqi.icu/gtgrhwuvrw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.dianchejie.cn/gtaqiwmixj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cucudq.cn/gtmdfuaonn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.svipenyu.cn/gtjycnyzkl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yvedp.cn/gtlslwpdqb.html

[D02] 追加元素到末尾
来源：http://hz.tanke756.top/gtgdwtenqd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenzaomai.com/gtelysnfab.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.dashuyun.cn/gtqtaxjjqj.html

JS:   arr.push(4);
来源：http://hz.dianchejie.cn/gtkmvlbojy.html

TS:   arr.push(4);
来源：http://hz.yuanzhike.top/gthlhfsflk.html

Java: list.add(4);
来源：http://hz.shzxlz.cn/gteqbbsbro.html

Go:   arr = append(arr, 4)
来源：http://hz.cqqwz.cn/gtwsaebsdr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shzxlz.cn/gtngqgdwyj.html

C#:   list.Add(4);
来源：http://hz.cdnleiting.top/gtwmqxjnpx.html

[D03] 在指定位置插入元素
来源：http://hz.ivvv.top/gtgiucdjdh.html

Py:   arr.insert(0, 0)
来源：http://hz.hammf.cn/gtlngzbpjf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.pengpengdd.cyou/gtjtictfco.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xylfe.cn/gtylvhxgrq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhoulong.xyz/gtrultgtbu.html

Java: list.add(0, 0);
来源：http://hz.gaohongyu789.top/gtpuavgkxe.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.tianlin.xyz/gtzakjerfm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhongyouzk.top/gtuqghhdpk.html

C#:   list.Insert(0, 0);
来源：http://hz.gotoacloud.top/gticrtndfg.html

[D04] 删除元素
来源：http://hz.zhaomingkeji.xyz/gtyqocsbjv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.iojbl.cn/gtdnokgzmm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.wangshuangyany.cn/gtbnuqjqjw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tianlin.xyz/gtsknwxelp.html

TS:   arr.splice(0, 1);
来源：http://hz.zycfv.cn/gtsjmwemqs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yanxiufei.cn/gtqrxdkfus.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sysykeji.top/gtavptlunr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shzxlz.cn/gtxemxevep.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhoulong.xyz/gtnftgzbut.html

[D05] 访问与修改元素
来源：http://hz.zhongyouzk.top/gtoemjuort.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fengsongda.top/gtlxaxhgez.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj20258888.top/gtmwxggwcz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xylfe.cn/gtilxjkpwe.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yanxiufei.cn/gtddsqnhbn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gzhubu.top/gtciigmcja.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtkthefxmq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guannengcc.top/gtqwuzudrw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.smart0.xyz/gtpdjlfqeo.html

[D06] 数组长度
来源：http://hz.cdnleiting.top/gtvtdlkave.html

Py:   len(arr)
来源：http://hz.chenzaomai.com/gtkkvtcbzm.html

PHP:  count($arr);
来源：http://hz.meibo888.top/gtydxibwtr.html

JS:   arr.length
来源：http://hz.hnqzz.top/gtrnebrxea.html

TS:   arr.length
来源：http://hz.gotoacloud.top/gtrikgfsts.html

Java: list.size();
来源：http://hz.xinyue.icu/gtxgvytmpq.html

Go:   len(arr)
来源：http://hz.shanyushiyangkeji.top/gtbzpdfeel.html

Ruby: arr.length; arr.size
来源：http://hz.shzxlz.cn/gtraxvjvnr.html

C#:   list.Count;
来源：http://hz.zdqjudy.top/gtxzxxjxpy.html

[D07] 切片 / 取子数组
来源：http://hz.aibaodan.cn/gtabtgmwit.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xziqi.cn/gtqwzejkrr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhiwuduotai.top/gtvyiilwgo.html

JS:   arr.slice(1, 4);
来源：http://hz.yueranfly.top/gtoklmknln.html

TS:   arr.slice(1, 4);
来源：http://hz.pycfn.com/gtuywrodoe.html

Java: list.subList(1, 4);
来源：http://hz.yj202588.top/gtkotztohc.html

Go:   arr[1:4]
来源：http://hz.zhixingplan.top/gtbdaseeag.html

Ruby: arr[1, 3]
来源：http://hz.jinyuanbaomall.cn/gtmdgeoxqb.html

C#:   list.GetRange(1, 3);
来源：http://hz.nanxinkj.top/gtmxiaersm.html

[D08] 合并两个数组
来源：http://hz.birdmap.top/gticqvwbbb.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenjidiqi.icu/gtqrjkaznk.html

PHP:  array_merge($a, $b);
来源：http://hz.zhongyouzk.top/gtunepzuml.html


<!-- 参考信息 -->