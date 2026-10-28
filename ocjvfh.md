代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://hz.sysykeji.top/gtbxnyhvwm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.guannengcc.top/gtbsgtsyxz.html

JS:   do { i++; } while (i < 10);
来源：http://hz.nwbrower.top/gtkwwdbxnz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ywan-chungtsiang.top/gtbyvwcefy.html

Java: do { i++; } while (i < 10);
来源：http://hz.cdnleiting.top/gtcxzicihr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.shangyingyoupin.top/gtdwgkglvh.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.andypj.xyz/gtnhwcayce.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jiagoushi.top/gtrhcuqkga.html

[B09] break 与 continue
来源：http://hz.tianlin.xyz/gteoebtzyb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hfpthk.cn/gtuazwbzhz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yvedp.cn/gtzhktpgiz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtawcamjok.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.52xcode.cn/gteptqktzp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gthixhjsny.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.chenzaomai.com/gtcrhjlsvf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.pengpengdd.cyou/gttzkexdrg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.quarkkingdee.top/gtcwucwugx.html

[B10] 遍历同时拿索引
来源：http://hz.hnqzz.top/gtrdyqoimt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.feifeiyinyue.top/gtlukrxrrc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.wangdashe.top/gtngbqtcsw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.sysykeji.top/gtwduxzlsa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ybcxt.top/gtyouoghca.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.feifeiyinyue.top/gtrtofpzft.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jqgufenzy.top/gttmfsamzj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jlsjyb.cn/gtstkkkoag.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hnqzz.top/gteyrfkggh.html

[B11] 生成数字序列 / 区间
来源：http://hz.yuanzhike.top/gtibugoncy.html

Py:   list(range(0, 10, 2))
来源：http://hz.shangyingyoupin.top/gtnuljwuxk.html

PHP:  range(0, 10, 2);
来源：http://hz.jyoumei.cn/gtvxuhiclx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenzaomai.com/gtiijnjdet.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhongyouzk.top/gtcqcnkrdk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.snrcjt.cn/gtbpgzdhtj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.redwolf501.top/gtljchwpqw.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yuxming.cn/gtnbcrtqls.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhoulong.xyz/gtlbrlkipf.html

[B12] 跳出多层循环
来源：http://hz.jqgufenzy.top/gtlombjbco.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.guannengcc.top/gtbvvjdncr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.sufxvd.cn/gtqykjsfjh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.snrcjt.cn/gtcxeuppym.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cheryme.top/gtmtgrekni.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.9152youxi.cn/gtokoxepwv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ppjwa.cn/gtiwhsyyfm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xylfe.cn/gtdpjhdqpc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.haohaochexian.top/gtqdfgxktk.html

[B13] 判断是否为数字
来源：http://hz.yonumen.top/gtdbxyjpjc.html

Py:   isinstance(x, (int, float))
来源：http://hz.jianghu66.top/gtkghypnop.html

PHP:  is_numeric($x)
来源：http://hz.wangdashe.top/gtsjgrperr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.0kj1m.cn/gtbcxsjnps.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj20258888.top/gtqksjvrde.html

Java: x instanceof Number
来源：http://hz.jinqigufen.top/gtbalamkkd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.tianlin.xyz/gtvdfjyicq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.cheryme.top/gtrejvupme.html

C#:   x is int or double or decimal
来源：http://hz.yj202588.top/gtkgngmtti.html

[B14] 判断值是否在集合内
来源：http://hz.zhaomingkeji.xyz/gtujdhluxi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gogol.net.cn/gtxwnijhqa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.nanxuanxn.top/gtckjvtvlp.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yongpay.top/gtdkqockto.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xuetiantiany.cn/gtsfoeough.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhaomingkeji.xyz/gtwbtjevxg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.smart0.xyz/gtvnxbwhwu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hnqzz.top/gthueyvtbe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yj202588.top/gtsqnsqegl.html

[B15] 布尔运算与取反
来源：http://hz.sweek.top/gtjyziqkyd.html

Py:   a and b or not c
来源：http://hz.chenjidiqi.icu/gtxnxgodtk.html

PHP:  $a && $b || !$c
来源：http://hz.zhiwuduotai.top/gtlfyisotn.html

JS:   a && b || !c
来源：http://hz.yangfankeji.com/gtkhsimpld.html

TS:   a && b || !c
来源：http://hz.daria6918.cn/gtsovvqpfh.html

Java: a && b || !c
来源：http://hz.smart0.xyz/gtibijvoez.html

Go:   a && b || !c
来源：http://hz.cqqwz.cn/gtkwdaquvh.html

Ruby: a && b || !c
来源：http://hz.redwolf501.top/gtqqbmzlbm.html

C#:   a && b || !c
来源：http://hz.iojbl.cn/gtrhxxefue.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hysaishi.cn/gtrvihuzge.html

Py:   if not data: return
来源：http://hz.yangfankeji.com/gtdwzxrcvq.html

PHP:  if (!$data) { return; }
来源：http://hz.yangfankeji.com/gtojhjtqup.html

JS:   if (!data) return;
来源：http://hz.meibo888.top/gtmoeilfey.html

TS:   if (!data) return;
来源：http://hz.shangyingyoupin.top/gtuilbsbxe.html

Java: if (data == null) return;
来源：http://hz.yj20258888.top/gtjpixbirv.html

Go:   if data == nil { return }
来源：http://hz.zhiwuduotai.top/gtmofvyouk.html

Ruby: return if data.nil?
来源：http://hz.mhx1999.top/gtricgjiin.html

C#:   if (data == null) return;
来源：http://hz.xingfuxueyuan.xyz/gtrxfqzlmn.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtqwsgeovr.html

C. 函数与作用域
来源：http://hz.dianchejie.cn/gtkedsyhvw.html

================================================================================
来源：http://hz.fengsongda.top/gtfidlzqbn.html

[C01] 定义函数
来源：http://hz.jinyuanbaomall.cn/gtqxromxyy.html

Py:   def add(a, b): return a + b
来源：http://hz.tianlin.xyz/gtcarnbpnd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daria6918.cn/gtuiejlrkq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yj20258.top/gtuihvtvxq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.vqdsnc.cn/gtzibzbiqh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yuanzhike.top/gtdvgqgamx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yangfankeji.com/gtnrypdoqq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.daria6918.cn/gtkvbybubg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cucudq.cn/gtomkxheoz.html

[C02] 默认参数
来源：http://hz.zhijiandao.cn/gtduqbpbag.html

Py:   def greet(name="World"): return name
来源：http://hz.xziqi.cn/gtkoofdrzt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.feifeiyinyue.top/gthllmadcl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.aizwys.cn/gtmtklgtzw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhiwuduotai.top/gtrosdcedp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hongshengwenyu.top/gtbvzdvctu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shanyushiyangkeji.top/gtcrjnadir.html

Ruby: def greet(name = "World") = name
来源：http://hz.hnxiangtu.top/gtufxlfhqp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tanke756.top/gtcyedbxua.html

[C03] 可变参数
来源：http://hz.yangfankeji.com/gtntecfuhq.html

Py:   def total(*args): return sum(args)
来源：http://hz.c1oappe.top/gthacjoylw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yj20258888.top/gtsfmgarjl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yuxming.cn/gtcrdoffdn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nwbrower.top/gtcngwxuxn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gogol.net.cn/gthmgrcklj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhaomingkeji.xyz/gtrlvoxdty.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ydzc1.top/gtfgxfpinu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.0kj1m.cn/gtcbohzvpk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ivvv.top/gtpjwbrhdf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhengqikj.top/gtwicfxkzg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhaomingkeji.xyz/gtpbvqlaks.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.redwolf501.top/gtlfwdwrxu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhijiandao.cn/gtkjynmfdu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.iojbl.cn/gtzntgaujs.html

Go:   // 无：用配置结构体参数
来源：http://hz.yueranfly.top/gthtcbyize.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ehwqpu.com/gtrlzrzwbo.html

C#:   f(a: 1, b: 2)
来源：http://hz.yanxiufei.cn/gtzypsnywx.html

[C05] 返回多个值
来源：http://hz.yvedp.cn/gtnuwiloha.html

Py:   return a, b
来源：http://hz.aizwys.cn/gtxacmqhml.html

PHP:  return [$a, $b];
来源：http://hz.ehwqpu.com/gthbubbbur.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.vqdsnc.cn/gtngjessth.html

TS:   return { a, b };
来源：http://hz.wangdashe.top/gtbwyzjscz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ydzc1.top/gtdtkfyhff.html

Go:   return a, b
来源：http://hz.hongshengwenyu.top/gtiretjjug.html

Ruby: return a, b
来源：http://hz.cucudq.cn/gtycobnqsf.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xuanzx.com/gtlnyyzske.html

[C06] 匿名函数 / lambda
来源：http://hz.quarkkingdee.top/gtdyfudxje.html

Py:   square = lambda x: x * x
来源：http://hz.daria6918.cn/gtualutggf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.9152youxi.cn/gtprvxotoi.html

JS:   const square = x => x * x;
来源：http://hz.xylfe.cn/gtjtuzzdbw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gogol.net.cn/gtjmgqfeqe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.havefunace.top/gtubiilpfz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zycfv.cn/gtrkmpaubk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.0kj1m.cn/gtudylaajk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj20258.top/gtvxupsgsp.html

[C07] 把函数作为参数传入
来源：http://hz.yueranfly.top/gtbilfclcs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ybcxt.top/gtlyclgikm.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.0kj1m.cn/gtzpnbyghc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jqgufenzy.top/gtxamebgnu.html

TS:   arr.map(String)
来源：http://hz.nanxuanxn.top/gticjdivrr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.aizwys.cn/gtxpndfcio.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.svipenyu.cn/gtkokqlnkl.html

Ruby: arr.map(&:upcase)
来源：http://hz.yj20258.top/gtlrjrfzny.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.dashuyun.cn/gtqqjetoih.html

[C08] 闭包
来源：http://hz.fengsongda.top/gtqscsagnw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhaomingkeji.xyz/gtpdfxkkfm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.meibo888.top/gtvoztxopq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtnctbkmqo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtadghvzdm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hnqzz.top/gtgnzwgsvf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhongyouzk.top/gtkjrflorl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.9152youxi.cn/gtcpdbttcv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shzxlz.cn/gtczlkexbl.html

[C09] 递归
来源：http://hz.cqqwz.cn/gtggbwydtr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj20258.top/gtmnymxjaf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.mhx1999.top/gtnzudzybh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hongshengwenyu.top/gtzmzdecji.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ybcxt.top/gtinfodfbe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.52xcode.cn/gtexzevaet.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jianghu66.top/gtcpdybswa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xziqi.cn/gtyjxtaiyw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhengqikj.top/gtnfdpdkpf.html

[C10] 变量作用域
来源：http://hz.zdqjudy.top/gtxnhnbjri.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xingfuxueyuan.xyz/gtydgeadou.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ywan-chungtsiang.top/gtkomjebyd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhiwuduotai.top/gtqecgzbtl.html

TS:   同 JS
来源：http://hz.yj20258888.top/gtfioszhdc.html

Java: 方法内为块级作用域
来源：http://hz.redwolf501.top/gtnimmfkue.html

Go:   花括号块级作用域
来源：http://hz.jinqigufen.top/gtmqnnyvhq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.quarkkingdee.top/gtcmqtoaxj.html

C#:   块级作用域
来源：http://hz.sysykeji.top/gtxlehcklj.html

[C11] 模块导入与导出
来源：http://hz.dianchejie.cn/gttwctepos.html

Py:   from module import func
来源：http://hz.ybcxt.top/gtybasuygs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ydzc1.top/gtahupufpn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yvedp.cn/gtcplmfrtb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sysykeji.top/gtlmzhtdju.html

Java: import java.util.List;
来源：http://hz.jianghu66.top/gtvfovskrv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.chenlongwang.top/gtetuhcmbu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yuxming.cn/gtvgmtlxis.html

C#:   using System.Text;
来源：http://hz.zhaomingkeji.xyz/gtxwjymwbd.html

[C12] 立即执行函数 IIFE
来源：http://hz.bjfxy.top/gtwwxotzgi.html

Py:   (lambda: print("run"))()
来源：http://hz.yanxiufei.cn/gtahmupkvc.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinqigufen.top/gtrfvalirf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hnqzz.top/gtkrcgfgbq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cashguo.top/gteryhqtlh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ywan-chungtsiang.top/gtnaisvyav.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.316326.xyz/gtpajlncwv.html

Ruby: -> { puts "run" }.call
来源：http://hz.cqqwz.cn/gtpyqowsmr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.pengpengdd.cyou/gtdetfgjhl.html

[C13] 类型声明 / 类型注解
来源：http://hz.daxiang520.top/gtnnzmpclh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yongpay.top/gtnlklvuzv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xinyue.icu/gtxlhipqes.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hnqzz.top/gtmppegohg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuanzx.com/gtcwhdbbhq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhixingplan.top/gtgqijvwft.html

Go:   func add(a, b int) int
来源：http://hz.chenjidiqi.icu/gtnnreqjbi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cucudq.cn/gtmamrraks.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.c1oappe.top/gtdmfywyaz.html

[C14] 泛型函数
来源：http://hz.redwolf501.top/gtzbuyvqij.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sweek.top/gtprfzdvva.html

PHP:  // 无泛型
来源：http://hz.sweek.top/gtimcgytpn.html

JS:   // 无泛型
来源：http://hz.jyoumei.cn/gtgpwjzzdp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gzhubu.top/gtoewqkbmo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ppjwa.cn/gtxmzdnwxz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.aizwys.cn/gtoubhkbrr.html

Ruby: # 无泛型
来源：http://hz.ybcxt.top/gtnpdeqllq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhoulong.xyz/gtmvtctezr.html

[C15] 解构 / 展开参数
来源：http://hz.xylfe.cn/gtolygmuwa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nanxinkj.top/gtzdbtgrcu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.guannengcc.top/gtdthptkwt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hfpthk.cn/gtjdrbtsqu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yueranfly.top/gtdmwmtcea.html

Java: // 无解构
来源：http://hz.havefunace.top/gtrzhkmlta.html

Go:   // 无解构
来源：http://hz.yanxiufei.cn/gtxvuylkyo.html

Ruby: a, b = pair
来源：http://hz.jinghuilouyu.cn/gtmeyftbii.html

C#:   var (a, b) = pair;
来源：http://hz.yueranfly.top/gtxtcunwri.html

[C16] 函数 / 方法重载
来源：http://hz.zhijiandao.cn/gtlmeygkrs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sufxvd.cn/gtsekkgrkf.html

PHP:  // 无重载
来源：http://hz.mhx1999.top/gtsgjzhjsp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenzaomai.com/gtnercloyh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tanke756.top/gtutjcndjc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yanxiufei.cn/gtildweupu.html

Go:   // 无重载：用不同函数名
来源：http://hz.shuidangran.top/gtnqyyriwi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.chenzaomai.com/gtzdvyidoa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hongshengwenyu.top/gtrbygyknk.html

================================================================================
来源：http://hz.yongpay.top/gtcgqvyoou.html

D. 数组 / 列表 / 集合
来源：http://hz.xingfuxueyuan.xyz/gtvodakqeb.html

================================================================================
来源：http://hz.yangfankeji.com/gtkchtnown.html

[D01] 创建数组 / 列表
来源：http://hz.yongpay.top/gtoemaycko.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jqgufenzy.top/gtujnyoxhi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.52xcode.cn/gttlzwbxos.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yvedp.cn/gtcuckctqw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hongshengwenyu.top/gtmaupzkuh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ybcxt.top/gtyhvalwgi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.dianchejie.cn/gtsgktgqqa.html

Ruby: arr = [1, 2, 3]
来源：http://hz.aibaodan.cn/gtisbyxbun.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgfzy.top/gtzradwrus.html

[D02] 追加元素到末尾
来源：http://hz.hysaishi.cn/gtgpovlpcb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ydjk.org.cn/gtolxjnmru.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shanyushiyangkeji.top/gtpjmzedwx.html

JS:   arr.push(4);
来源：http://hz.xuanzx.com/gtgnjfjcnb.html

TS:   arr.push(4);
来源：http://hz.dianchejie.cn/gtyofkesma.html

Java: list.add(4);
来源：http://hz.nwbrower.top/gtwekftygf.html

Go:   arr = append(arr, 4)
来源：http://hz.aibaodan.cn/gtbqgudsia.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hongshengwenyu.top/gtitmsxqxl.html

C#:   list.Add(4);
来源：http://hz.daria6918.cn/gtorjytlde.html

[D03] 在指定位置插入元素
来源：http://hz.wangdashe.top/gtqhjdhyvg.html

Py:   arr.insert(0, 0)
来源：http://hz.jyoumei.cn/gtxxxcrkbj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenzaomai.com/gtasogdtyg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sxryk.cn/gtmpsaenoe.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.daxiang520.top/gtmxfyahad.html

Java: list.add(0, 0);
来源：http://hz.52xcode.cn/gtcucjbjmo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yvedp.cn/gtstcmjktt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.andypj.xyz/gtkxvhxguu.html

C#:   list.Insert(0, 0);
来源：http://hz.zhongyouzk.top/gtoppenvoh.html

[D04] 删除元素
来源：http://hz.316326.xyz/gttstcqpyg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.mhx1999.top/gtbjcrshrg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jyoumei.cn/gtmfpbugrf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yj202588.top/gtcrmclnwo.html

TS:   arr.splice(0, 1);
来源：http://hz.yonumen.top/gtvdynfrqr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.havefunace.top/gtueevvweg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shzxlz.cn/gtaxskjhyi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.wangshuangyany.cn/gtkibtyexd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.smart0.xyz/gthjuraohi.html

[D05] 访问与修改元素
来源：http://hz.kuanghao11.cn/gtlmrleobj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtguiierje.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yonumen.top/gtbwnaxwpp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shuidangran.top/gtnmoqtzbk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.quarkkingdee.top/gtpxvqoyyv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yanxiufei.cn/gtsevovnhj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.daria6918.cn/gtpogxkjgl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtyphebnex.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.birdmap.top/gtxerpbvgm.html

[D06] 数组长度
来源：http://hz.zhoulong.xyz/gtccetxcmv.html

Py:   len(arr)
来源：http://hz.ehwqpu.com/gtautsmvsi.html

PHP:  count($arr);
来源：http://hz.ivvv.top/gtfxxyzkus.html

JS:   arr.length
来源：http://hz.zhongyouzk.top/gtorrozmyr.html

TS:   arr.length
来源：http://hz.chenzaomai.com/gtkfjefihn.html

Java: list.size();
来源：http://hz.birdmap.top/gtowfrxzbt.html

Go:   len(arr)
来源：http://hz.jinyuanbaomall.cn/gtpbqjhnsm.html

Ruby: arr.length; arr.size
来源：http://hz.nwbrower.top/gtijxisjom.html

C#:   list.Count;
来源：http://hz.daxiang520.top/gtvmiwwtyi.html

[D07] 切片 / 取子数组
来源：http://hz.yangfankeji.com/gtuncpbpdh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinqigfzy.top/gtcvwiscxd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhoulong.xyz/gtusorifvk.html

JS:   arr.slice(1, 4);
来源：http://hz.cqqwz.cn/gtseyygwjx.html

TS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtsimkqknk.html

Java: list.subList(1, 4);
来源：http://hz.gzhubu.top/gtxprkrvod.html

Go:   arr[1:4]
来源：http://hz.52xcode.cn/gtfmlandht.html

Ruby: arr[1, 3]
来源：http://hz.0kj1m.cn/gtmgqhpxxt.html

C#:   list.GetRange(1, 3);
来源：http://hz.hnqzz.top/gttughzrcw.html

[D08] 合并两个数组
来源：http://hz.ivvv.top/gtttjidkvh.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenzaomai.com/gtdjfqdkun.html

PHP:  array_merge($a, $b);
来源：http://hz.zhongyouzk.top/gtiwqzyzte.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.quarkkingdee.top/gtubckensj.html

TS:   [...a, ...b];
来源：http://hz.guannengcc.top/gtzjagjhct.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhiwuduotai.top/gtusyyxmlr.html

Go:   append(a, b...)
来源：http://hz.smart0.xyz/gtuukohffe.html


<!-- 参考信息 -->