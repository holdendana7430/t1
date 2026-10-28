代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.chenzaomai.com/gtuaptoreg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yueranfly.top/gtjhnrtrsx.html

[B07] while 循环
来源：http://hz.hammf.cn/gtafqdkfij.html

Py:   while i < 10: i += 1
来源：http://hz.birdmap.top/gtzeadzcns.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zhongyouzk.top/gtogbdkjkk.html

JS:   while (i < 10) { i++; }
来源：http://hz.cheryme.top/gtpyaaurhu.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhixingplan.top/gthbsdbzbw.html

Java: while (i < 10) { i++; }
来源：http://hz.iojbl.cn/gthxtpjyiu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hnqzz.top/gtrbsuxtbk.html

Ruby: while i < 10; i += 1; end
来源：http://hz.tian-w.cn/gtqkkgbldy.html

C#:   while (i < 10) { i++; }
来源：http://hz.dianchejie.cn/gtpxhhbmjo.html

[B08] do-while（至少执行一次）
来源：http://hz.yj202588.top/gtvdrgurpw.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jinqigfzy.top/gtbdejbwxs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.c1oappe.top/gtaulbvbhc.html

JS:   do { i++; } while (i < 10);
来源：http://hz.ywan-chungtsiang.top/gtwrbiuurv.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gttzslzljd.html

Java: do { i++; } while (i < 10);
来源：http://hz.bjfxy.top/gtvkjjelzi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cashguo.top/gtrzgssoin.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.cucudq.cn/gtnhfyosbt.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cucudq.cn/gtgzrimrgg.html

[B09] break 与 continue
来源：http://hz.ywan-chungtsiang.top/gtglakuxpv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.havefunace.top/gtuhpwnsrc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cashguo.top/gtivbocmhi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aizwys.cn/gtdzwogfdk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gtzzeurfnu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtofhgoniv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hywenlv.cn/gtonwftsum.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.feifeiyinyue.top/gtcezyofoi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xinyue.icu/gtpqcfivyb.html

[B10] 遍历同时拿索引
来源：http://hz.cheryme.top/gtluzeikbm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.sxryk.cn/gtbvaosmio.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yuxming.cn/gthutybdbq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.dianchejie.cn/gtwwlunjcx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.c1oappe.top/gtmaylvxlg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.guowangkeji.top/gtjjhqcobp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.cqqwz.cn/gtmizjpxrm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gzhubu.top/gtyfggbepx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.cdnleiting.top/gtwqgffhgq.html

[B11] 生成数字序列 / 区间
来源：http://hz.fzhhl.top/gtdjevvsmm.html

Py:   list(range(0, 10, 2))
来源：http://hz.daria6918.cn/gtsmwmejdc.html

PHP:  range(0, 10, 2);
来源：http://hz.mhx1999.top/gtpanvfcpf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangshuangyany.cn/gttfsmlhyz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenjidiqi.icu/gtfqrplhnp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xuetiantiany.cn/gtbdnliboq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jqgfzy.top/gtivzgrmut.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ydzc1.top/gtplevxefo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.sxryk.cn/gtpiyjsayc.html

[B12] 跳出多层循环
来源：http://hz.sxryk.cn/gthirpjucz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nwbrower.top/gtvefnsjrt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xylfe.cn/gtbpnwmzzf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.dianchejie.cn/gtkhfyclkn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnqzz.top/gtgddwgqbe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuanzx.com/gtywgulkcs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.c1oappe.top/gtaayyhlxs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.dianchejie.cn/gtaogjwzgm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yuxming.cn/gtluedxbnf.html

[B13] 判断是否为数字
来源：http://hz.hnxiangtu.top/gtqufvhxbh.html

Py:   isinstance(x, (int, float))
来源：http://hz.tanke756.top/gtngyjoscy.html

PHP:  is_numeric($x)
来源：http://hz.feifeiyinyue.top/gtqmvrkqqj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.wangdashe.top/gtttcovrfk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgufenzy.top/gtrvgpjjdg.html

Java: x instanceof Number
来源：http://hz.jlsjyb.cn/gtxqxtrzcm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.pycfn.com/gtusjxdqij.html

Ruby: x.is_a?(Numeric)
来源：http://hz.gaohongyu789.top/gtdlyiijpu.html

C#:   x is int or double or decimal
来源：http://hz.shanyushiyangtech.top/gtfhyuhagd.html

[B14] 判断值是否在集合内
来源：http://hz.shuidangran.top/gtoehcwoof.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ehwqpu.com/gtlyzygeir.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.chenjidiqi.icu/gtwwcwmiub.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangtech.top/gtqscjjeyi.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zdqjudy.top/gtoyveaiiu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.daria6918.cn/gtwmhiddjv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.andypj.xyz/gtipdpmbwv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xylfe.cn/gtfneiywrh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.iojbl.cn/gtrrmcifza.html

[B15] 布尔运算与取反
来源：http://hz.316326.xyz/gtmqbniovu.html

Py:   a and b or not c
来源：http://hz.daria6918.cn/gtcjnuklcj.html

PHP:  $a && $b || !$c
来源：http://hz.birdmap.top/gtirrwgjag.html

JS:   a && b || !c
来源：http://hz.quarkkingdee.top/gtwmpgjxsm.html

TS:   a && b || !c
来源：http://hz.smart0.xyz/gtzkgdjbpl.html

Java: a && b || !c
来源：http://hz.cheryme.top/gtboyuajtd.html

Go:   a && b || !c
来源：http://hz.hnqzz.top/gtjpfgwqcd.html

Ruby: a && b || !c
来源：http://hz.yuanzhike.top/gtcqblfqsm.html

C#:   a && b || !c
来源：http://hz.andypj.xyz/gtquviwtnp.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xinyue.icu/gtdztoohom.html

Py:   if not data: return
来源：http://hz.yangfankeji.com/gtelugvtpf.html

PHP:  if (!$data) { return; }
来源：http://hz.bjfxy.top/gthluqnrxg.html

JS:   if (!data) return;
来源：http://hz.pengpengdd.cyou/gtrunjhokp.html

TS:   if (!data) return;
来源：http://hz.zhiwuduotai.top/gtmfdqpels.html

Java: if (data == null) return;
来源：http://hz.jinqigufen.top/gtjojztmxl.html

Go:   if data == nil { return }
来源：http://hz.ivvv.top/gtwworvwjd.html

Ruby: return if data.nil?
来源：http://hz.shangyingyoupin.top/gtjqpazzaw.html

C#:   if (data == null) return;
来源：http://hz.kuanghao11.cn/gthfaiovyx.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtwpnfbftf.html

C. 函数与作用域
来源：http://hz.cheryme.top/gtppvmhcak.html

================================================================================
来源：http://hz.gaohongyu789.top/gtdrybcxbx.html

[C01] 定义函数
来源：http://hz.mhx1999.top/gtoawghmrc.html

Py:   def add(a, b): return a + b
来源：http://hz.hammf.cn/gtzaykjalw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gthhdzlhau.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenzaomai.com/gttcqamdpn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cashguo.top/gtuxioiiny.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtavrooryn.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yueranfly.top/gtyszzcosy.html

Ruby: def add(a, b); a + b; end
来源：http://hz.wangdashe.top/gtdrdvexsw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ydjk.org.cn/gtuyqujddv.html

[C02] 默认参数
来源：http://hz.cdnleiting.top/gtytyyfsns.html

Py:   def greet(name="World"): return name
来源：http://hz.redwolf501.top/gtveujojgr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.quarkkingdee.top/gtbuivkfpn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.smart0.xyz/gttzablsgb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.vqdsnc.cn/gtolnluwvx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.daria6918.cn/gtthliwgjd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hysaishi.cn/gthplguspp.html

Ruby: def greet(name = "World") = name
来源：http://hz.yongpay.top/gtzghsqjxq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jqgufenzy.top/gtgowouhnd.html

[C03] 可变参数
来源：http://hz.yuxming.cn/gtptnutpxq.html

Py:   def total(*args): return sum(args)
来源：http://hz.snrcjt.cn/gtarjcmhfb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.nanxinkj.top/gtapzuxpdo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenzaomai.com/gtlghwhptk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj20258.top/gtfjnazfzc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hongshengwenyu.top/gtwradyavv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ywan-chungtsiang.top/gtwxgtmciv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.kuanghao11.cn/gtzghwrhux.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gotoacloud.top/gttqwnrojt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.svipenyu.cn/gtmorkuvhk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhixingplan.top/gtrsyreskh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hnqzz.top/gterpudtfw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xuanzx.com/gtvbxcssra.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gotoacloud.top/gtrnohisew.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.svipenyu.cn/gteotycdcu.html

Go:   // 无：用配置结构体参数
来源：http://hz.gogol.net.cn/gtdavgkfyy.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtqyruwegk.html

C#:   f(a: 1, b: 2)
来源：http://hz.jyoumei.cn/gtzxkutglx.html

[C05] 返回多个值
来源：http://hz.hysaishi.cn/gtikewhxgw.html

Py:   return a, b
来源：http://hz.daria6918.cn/gtvrcwogyq.html

PHP:  return [$a, $b];
来源：http://hz.bjfxy.top/gtnikrddni.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.chenzaomai.com/gthqwfuveb.html

TS:   return { a, b };
来源：http://hz.chenzaomai.com/gtgrdevgal.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yuxming.cn/gtjfkpehgo.html

Go:   return a, b
来源：http://hz.nwbrower.top/gticljobwq.html

Ruby: return a, b
来源：http://hz.sysykeji.top/gtddkggfec.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ybcxt.top/gtdxzvgkqg.html

[C06] 匿名函数 / lambda
来源：http://hz.sufxvd.cn/gtgtfujhkh.html

Py:   square = lambda x: x * x
来源：http://hz.tanke756.top/gtwkkkzlis.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.meibo888.top/gtxienabmg.html

JS:   const square = x => x * x;
来源：http://hz.hnqzz.top/gtkivffxsd.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinghuilouyu.cn/gtpckzljtz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sweek.top/gtgeegdbxs.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yangfankeji.com/gtoabdifki.html

Ruby: square = ->(x) { x * x }
来源：http://hz.daxiang520.top/gtprurtxok.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.fengsongda.top/gtstmwkjec.html

[C07] 把函数作为参数传入
来源：http://hz.chenjidiqi.icu/gtogbpsmjp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.dashuyun.cn/gtvoxylmrx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.cqqwz.cn/gtljjnttub.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.0kj1m.cn/gtizudqvoh.html

TS:   arr.map(String)
来源：http://hz.daxiang520.top/gtpskdlzyk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nanxuanxn.top/gtlbahafxf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jiagoushi.top/gtpkrndqor.html

Ruby: arr.map(&:upcase)
来源：http://hz.yj202588.top/gtqesesdec.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.guannengcc.top/gtmuxbqjwf.html

[C08] 闭包
来源：http://hz.dianchejie.cn/gtrmfyhghq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xinyue.icu/gtyozxiqjk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jqgufenzy.top/gtkkoqlklq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gtcfiqvzwn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gtvzrifumk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.havefunace.top/gtfqahtxzm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.haohaochexian.top/gthuplbufz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgufenzy.top/gthkojxtte.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj20258.top/gtjuavugol.html

[C09] 递归
来源：http://hz.havefunace.top/gteijvmedy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenzaomai.com/gtyfzzufqd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.mhx1999.top/gtjywjptab.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydjk.org.cn/gtfxkwbpar.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jyoumei.cn/gtgthntwzs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenjidiqi.icu/gtxolmwlkh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cheryme.top/gtiaxtrbzw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shanyushiyangtech.top/gthuduhcra.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.kuanghao11.cn/gtfcwpkvwu.html

[C10] 变量作用域
来源：http://hz.smart0.xyz/gtosxpvmxw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.havefunace.top/gttrpnwmra.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.snrcjt.cn/gtfnrmyaaa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cdnleiting.top/gtzkihfara.html

TS:   同 JS
来源：http://hz.zhoulong.xyz/gtwnldtoby.html

Java: 方法内为块级作用域
来源：http://hz.chenzaomai.com/gtxpgkgajg.html

Go:   花括号块级作用域
来源：http://hz.gzhubu.top/gtkmsgsfrg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sysykeji.top/gtfiyrstef.html

C#:   块级作用域
来源：http://hz.chenlongwang.top/gtjrmfetir.html

[C11] 模块导入与导出
来源：http://hz.xuetiantiany.cn/gtvbktiany.html

Py:   from module import func
来源：http://hz.hongshengwenyu.top/gtaaadwnig.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.quarkkingdee.top/gtrqonfbdi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jiagoushi.top/gtgfiernxm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.fengsongda.top/gtyxdjbsfn.html

Java: import java.util.List;
来源：http://hz.chenzaomai.com/gtstoitcao.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cashguo.top/gtddeeuceb.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cdnleiting.top/gthnysshkv.html

C#:   using System.Text;
来源：http://hz.jyoumei.cn/gttifyjetj.html

[C12] 立即执行函数 IIFE
来源：http://hz.jianghu66.top/gtgpalumqb.html

Py:   (lambda: print("run"))()
来源：http://hz.feifeiyinyue.top/gtnfveexsk.html

PHP:  (function () { echo "run"; })();
来源：http://hz.gogol.net.cn/gtiwawvtvc.html

JS:   (() => { console.log("run"); })();
来源：http://hz.redwolf501.top/gtvgokaosr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jqgfzy.top/gtprvppmza.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.feifeiyinyue.top/gtriplwbef.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhixingplan.top/gtqweiqbnx.html

Ruby: -> { puts "run" }.call
来源：http://hz.jyoumei.cn/gtihxbfrrd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.tanke756.top/gtkjgaeeuy.html

[C13] 类型声明 / 类型注解
来源：http://hz.dashuyun.cn/gtdtufedma.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xylfe.cn/gtbssmgiud.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnxiangtu.top/gtdhdjvhuu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhixingplan.top/gtlzlkhlnd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.redwolf501.top/gtdogsmnwf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cqqwz.cn/gtbmogrrek.html

Go:   func add(a, b int) int
来源：http://hz.haohaochexian.top/gtwdubcflb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cucudq.cn/gtgmlocbaa.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shuidangran.top/gtevqeitmf.html

[C14] 泛型函数
来源：http://hz.zhixingplan.top/gtzervqhzh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.mhx1999.top/gtjhudshzr.html

PHP:  // 无泛型
来源：http://hz.cucudq.cn/gtujgtqlgw.html

JS:   // 无泛型
来源：http://hz.chenlongwang.top/gtwndwqtef.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ybcxt.top/gtnmabanlg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.meibo888.top/gtdtcuhklp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.redwolf501.top/gtgmffmqmo.html

Ruby: # 无泛型
来源：http://hz.shuidangran.top/gtiefqtguq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.svipenyu.cn/gtveyxhqfa.html

[C15] 解构 / 展开参数
来源：http://hz.zdqjudy.top/gtcnktkynp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.redwolf501.top/gtaylrulyt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.smart0.xyz/gteizgmruh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ivvv.top/gtpyvyuhva.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenjidiqi.icu/gtgeqgpgyv.html

Java: // 无解构
来源：http://hz.yj202588.top/gtbvweifma.html

Go:   // 无解构
来源：http://hz.ydjk.org.cn/gtdhhltmkp.html

Ruby: a, b = pair
来源：http://hz.tianlin.xyz/gtustnrsdy.html

C#:   var (a, b) = pair;
来源：http://hz.jyoumei.cn/gtftpiubuf.html

[C16] 函数 / 方法重载
来源：http://hz.zhixingplan.top/gtldgmforw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhengqikj.top/gtcxbfovss.html

PHP:  // 无重载
来源：http://hz.jqgfzy.top/gtmceetbpv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jiagoushi.top/gtbepnzudl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj202588.top/gtygavgzgb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhijiandao.cn/gtcbrxlouq.html

Go:   // 无重载：用不同函数名
来源：http://hz.nwbrower.top/gtrpxuvaee.html

Ruby: # 无重载：靠动态参数
来源：http://hz.316326.xyz/gtbcnealeu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.pycfn.com/gtptfqmeni.html

================================================================================
来源：http://hz.aizwys.cn/gtbkajcqrp.html

D. 数组 / 列表 / 集合
来源：http://hz.52xcode.cn/gtjwkmantr.html

================================================================================
来源：http://hz.redwolf501.top/gtuksugvrl.html

[D01] 创建数组 / 列表
来源：http://hz.zycfv.cn/gtpyohxzre.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jyoumei.cn/gttalmxnmz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.smart0.xyz/gtczpovxkq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj20258.top/gtwyeouuwd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.pycfn.com/gtlygawaan.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hnxiangtu.top/gtvvgmdgks.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jyoumei.cn/gtiixywvsa.html

Ruby: arr = [1, 2, 3]
来源：http://hz.dianchejie.cn/gtqfwtfwkw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj20258.top/gthepbwpcm.html

[D02] 追加元素到末尾
来源：http://hz.zdqjudy.top/gtlcfrjtup.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.nwbrower.top/gtgadjxpgc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgufenzy.top/gtskbwtkfw.html

JS:   arr.push(4);
来源：http://hz.ywan-chungtsiang.top/gtemrlefvw.html

TS:   arr.push(4);
来源：http://hz.cheryme.top/gtcwaosfxr.html

Java: list.add(4);
来源：http://hz.hnqzz.top/gtlwwpkexc.html

Go:   arr = append(arr, 4)
来源：http://hz.shzxlz.cn/gtmebytkhe.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.fzhhl.top/gtilxstahd.html

C#:   list.Add(4);
来源：http://hz.dianchejie.cn/gtrjqoncby.html

[D03] 在指定位置插入元素
来源：http://hz.sufxvd.cn/gtjjwpweyw.html

Py:   arr.insert(0, 0)
来源：http://hz.ehwqpu.com/gtjweotbai.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.guowangkeji.top/gtrsgdoqdz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jqgufenzy.top/gtzdwgtcdk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.vqdsnc.cn/gtbavtkddj.html

Java: list.add(0, 0);
来源：http://hz.nanxinkj.top/gtdymdhbyq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenjidiqi.icu/gtrgjmespq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhoulong.xyz/gtswgsbmry.html

C#:   list.Insert(0, 0);
来源：http://hz.nwbrower.top/gtkgaamjkh.html

[D04] 删除元素
来源：http://hz.jqgufenzy.top/gtbeiihphl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.wangshuangyany.cn/gteplholkt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.wangdashe.top/gtfsiuxruy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hfpthk.cn/gtmrjshuvb.html

TS:   arr.splice(0, 1);
来源：http://hz.kuanghao11.cn/gtxifjhyrj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.fengsongda.top/gtzvkdfjrm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.havefunace.top/gtmnqknsng.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ybcxt.top/gtlhmieoak.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhongyouzk.top/gtsyubyetx.html

[D05] 访问与修改元素
来源：http://hz.yvedp.cn/gtsxmnrmip.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtbrswlpdh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.9152youxi.cn/gtggsdiwic.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jyoumei.cn/gtkjjzhgvm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guowangkeji.top/gtyilgydhu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hammf.cn/gtwwnktefv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtkumksuie.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guannengcc.top/gtiiqimadq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xuetiantiany.cn/gtosntgsxo.html

[D06] 数组长度
来源：http://hz.daxiang520.top/gtjrrvmwkp.html

Py:   len(arr)
来源：http://hz.shzxlz.cn/gtrxmniqkh.html

PHP:  count($arr);
来源：http://hz.chenlongwang.top/gtvgvtkvby.html

JS:   arr.length
来源：http://hz.yj202588.top/gtqftyxpuv.html

TS:   arr.length
来源：http://hz.bjfxy.top/gtbfcvrbmu.html

Java: list.size();
来源：http://hz.sweek.top/gtoxbjazse.html

Go:   len(arr)
来源：http://hz.iojbl.cn/gtqxwjdogo.html

Ruby: arr.length; arr.size
来源：http://hz.c1oappe.top/gtxhqymtdh.html

C#:   list.Count;
来源：http://hz.pengpengdd.cyou/gtnrhoszzs.html

[D07] 切片 / 取子数组
来源：http://hz.cqqwz.cn/gtmvjvdoui.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.meibo888.top/gtpqxqqelg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.9152youxi.cn/gtafsbekkr.html

JS:   arr.slice(1, 4);
来源：http://hz.quarkkingdee.top/gtjqcuibmt.html


<!-- 参考信息 -->