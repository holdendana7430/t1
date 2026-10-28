代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.shanyushiyangtech.top/gtnrdexnnb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.guannengcc.top/gtqrswgnkw.html

[B07] while 循环
来源：http://hz.fzhhl.top/gtrbhsavii.html

Py:   while i < 10: i += 1
来源：http://hz.gaohongyu789.top/gtqmbxyesm.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.gotoacloud.top/gtzvrhoytc.html

JS:   while (i < 10) { i++; }
来源：http://hz.yonumen.top/gtcshxaexh.html

TS:   while (i < 10) { i++; }
来源：http://hz.chenjidiqi.icu/gtjsmsazac.html

Java: while (i < 10) { i++; }
来源：http://hz.xylfe.cn/gtcbnkhhui.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cheryme.top/gtptweruth.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhijiandao.cn/gtmfehyzty.html

C#:   while (i < 10) { i++; }
来源：http://hz.gogol.net.cn/gtgxmothre.html

[B08] do-while（至少执行一次）
来源：http://hz.hywenlv.cn/gtewqqbxpj.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhoulong.xyz/gtgecfwxtq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.316326.xyz/gtxcsarfqw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.tianlin.xyz/gtxocdrlpr.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hongshengwenyu.top/gtvllxqgog.html

Java: do { i++; } while (i < 10);
来源：http://hz.jqgfzy.top/gtlycuchwd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.gogol.net.cn/gtxsyozvbi.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.smart0.xyz/gtyesjqsnu.html

C#:   do { i++; } while (i < 10);
来源：http://hz.sufxvd.cn/gtmbulurnp.html

[B09] break 与 continue
来源：http://hz.yuxming.cn/gtjpxfykvn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.haohaochexian.top/gtxkoxsxdd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yj20258888.top/gtwmbugkxe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtltodzwfp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hammf.cn/gttpwuooyz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hammf.cn/gtbxzktsox.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jyoumei.cn/gthpfcnuoa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ybcxt.top/gtdrsenpqi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cdnleiting.top/gtejrdeedn.html

[B10] 遍历同时拿索引
来源：http://hz.wangshuangyany.cn/gtgaoibeae.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cashguo.top/gtkuhynizh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.chenlongwang.top/gtktuncrvm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.gzhubu.top/gthuymdjpk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.dianchejie.cn/gtalxmjoae.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shzxlz.cn/gtlndkwuuh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yongpay.top/gtjsapfrho.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ybcxt.top/gtkjkdhfqo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhixingplan.top/gttiiszyvq.html

[B11] 生成数字序列 / 区间
来源：http://hz.redwolf501.top/gtzwrioqhq.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenlongwang.top/gtbdfzsapz.html

PHP:  range(0, 10, 2);
来源：http://hz.redwolf501.top/gttootbgwe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinqigfzy.top/gtyiiwupsr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guannengcc.top/gtdbirwyvz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hnxiangtu.top/gtgjizszsp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinqigfzy.top/gtdvtdlxhh.html

Ruby: (0...10).step(2).to_a
来源：http://hz.daxiang520.top/gtauzcpjzh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.dashuyun.cn/gtbxwswzle.html

[B12] 跳出多层循环
来源：http://hz.yvedp.cn/gtmwvlxqae.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sysykeji.top/gtqlqwxsqu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ydjk.org.cn/gtmhvwmgsv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.0kj1m.cn/gterivipve.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.aizwys.cn/gtcinexktf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhixingplan.top/gtlytpmnul.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guannengcc.top/gtbitlasea.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shuidangran.top/gtqhxtdgew.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.9152youxi.cn/gtxhbznpvt.html

[B13] 判断是否为数字
来源：http://hz.havefunace.top/gtrysjlkkm.html

Py:   isinstance(x, (int, float))
来源：http://hz.gaohongyu789.top/gtkgqczpcc.html

PHP:  is_numeric($x)
来源：http://hz.zhixingplan.top/gtydwznlcv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xuanzx.com/gtomzpnjjg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fzhhl.top/gtamneolgi.html

Java: x instanceof Number
来源：http://hz.jianghu66.top/gtvbjyeymp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yongpay.top/gtnzmaemxa.html

Ruby: x.is_a?(Numeric)
来源：http://hz.sysykeji.top/gtxycwvonz.html

C#:   x is int or double or decimal
来源：http://hz.xuetiantiany.cn/gtkjzxssco.html

[B14] 判断值是否在集合内
来源：http://hz.jinyuanbaomall.cn/gtpfsltqhc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xylfe.cn/gtquqxvhks.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.birdmap.top/gtxhfmzalg.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.svipenyu.cn/gtpgnsmqsz.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhixingplan.top/gtscnejfql.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.fengsongda.top/gtoyjrmwgl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.fengsongda.top/gtbxterpuu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.redwolf501.top/gtdiivjuzv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zdqjudy.top/gtljreumjh.html

[B15] 布尔运算与取反
来源：http://hz.xylfe.cn/gtwskzcriu.html

Py:   a and b or not c
来源：http://hz.shuidangran.top/gtuyyrwoln.html

PHP:  $a && $b || !$c
来源：http://hz.quarkkingdee.top/gtszrbzlok.html

JS:   a && b || !c
来源：http://hz.fzhhl.top/gtswxbdoui.html

TS:   a && b || !c
来源：http://hz.yongpay.top/gtfqvunuxo.html

Java: a && b || !c
来源：http://hz.zhongyouzk.top/gtypcidktp.html

Go:   a && b || !c
来源：http://hz.dianchejie.cn/gttoftbthc.html

Ruby: a && b || !c
来源：http://hz.svipenyu.cn/gtohepjbqu.html

C#:   a && b || !c
来源：http://hz.nwbrower.top/gtcwspedwl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hfpthk.cn/gtuppvyilb.html

Py:   if not data: return
来源：http://hz.svipenyu.cn/gtopisnkkh.html

PHP:  if (!$data) { return; }
来源：http://hz.xziqi.cn/gtzyyzbmfo.html

JS:   if (!data) return;
来源：http://hz.zhaomingkeji.xyz/gtkofxmimz.html

TS:   if (!data) return;
来源：http://hz.shuidangran.top/gtypzwkghz.html

Java: if (data == null) return;
来源：http://hz.yuanzhike.top/gtgeeybmha.html

Go:   if data == nil { return }
来源：http://hz.shangyingyoupin.top/gtbtlpzzew.html

Ruby: return if data.nil?
来源：http://hz.zhijiandao.cn/gtjjjebzbu.html

C#:   if (data == null) return;
来源：http://hz.hywenlv.cn/gtnmvjxtma.html

================================================================================
来源：http://hz.yuanzhike.top/gtonldheuv.html

C. 函数与作用域
来源：http://hz.gotoacloud.top/gtscpdbhcy.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtiuznqyzd.html

[C01] 定义函数
来源：http://hz.cucudq.cn/gtslpjqcui.html

Py:   def add(a, b): return a + b
来源：http://hz.hfpthk.cn/gtcmretdcb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtxgelgyff.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jianghu66.top/gtcngcztxe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.mhx1999.top/gtaiwyueyj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtzmvyuzkh.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yueranfly.top/gtvacmgcff.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhongyouzk.top/gtpepqwlsb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtfmncxiyh.html

[C02] 默认参数
来源：http://hz.hongshengwenyu.top/gtyckdaqml.html

Py:   def greet(name="World"): return name
来源：http://hz.yj20258.top/gtsuwchslc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.snrcjt.cn/gtjonpmkmp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hysaishi.cn/gtgvyviwmf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.daria6918.cn/gtmbumbfvs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ivvv.top/gtipnzmnkl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.birdmap.top/gtopwpfjhi.html

Ruby: def greet(name = "World") = name
来源：http://hz.bjfxy.top/gtjsvhtitn.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj20258888.top/gtynmozfcz.html

[C03] 可变参数
来源：http://hz.birdmap.top/gtqgkmzsbl.html

Py:   def total(*args): return sum(args)
来源：http://hz.dashuyun.cn/gtgjbbbhet.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xylfe.cn/gttxftuinh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtkvpugqti.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gzhubu.top/gtglegkzex.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.daria6918.cn/gtmeldzelo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.tanke756.top/gthpqtmquf.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xinyue.icu/gtkhtywhcb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cashguo.top/gthmeotysx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.bjfxy.top/gtopcawbda.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.birdmap.top/gtdcztqawj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhoulong.xyz/gtnelvgpxd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yueranfly.top/gtffblnyou.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.redwolf501.top/gtvznfqdzz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.smart0.xyz/gtfjewzwcg.html

Go:   // 无：用配置结构体参数
来源：http://hz.kuanghao11.cn/gtrsmfwmpe.html

Ruby: f(a: 1, b: 2)
来源：http://hz.vqdsnc.cn/gtkebrxtkl.html

C#:   f(a: 1, b: 2)
来源：http://hz.yuanzhike.top/gtjjhzfrmd.html

[C05] 返回多个值
来源：http://hz.xinyue.icu/gtbomtxwpz.html

Py:   return a, b
来源：http://hz.ivvv.top/gtdvpposke.html

PHP:  return [$a, $b];
来源：http://hz.yongpay.top/gtunqcomww.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xuetiantiany.cn/gtgfbylnnq.html

TS:   return { a, b };
来源：http://hz.chenzaomai.com/gtxnqotodx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.chenjidiqi.icu/gtjkuflkcu.html

Go:   return a, b
来源：http://hz.zhaomingkeji.xyz/gtonnfuiwj.html

Ruby: return a, b
来源：http://hz.yongpay.top/gtyjoefdgi.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hnqzz.top/gtyqincazf.html

[C06] 匿名函数 / lambda
来源：http://hz.tian-w.cn/gtinxrzmpi.html

Py:   square = lambda x: x * x
来源：http://hz.bjfxy.top/gtxfynikbl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.redwolf501.top/gthdrlabgb.html

JS:   const square = x => x * x;
来源：http://hz.zhoulong.xyz/gtsrdglzax.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.fzhhl.top/gttfzeqhqj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinqigufen.top/gttrhhsqaa.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ywan-chungtsiang.top/gtpyblscvw.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinqigufen.top/gtwimeftac.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yanxiufei.cn/gtmraisqbi.html

[C07] 把函数作为参数传入
来源：http://hz.bjfxy.top/gtdkquonue.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.52xcode.cn/gtglujoywu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hfpthk.cn/gtzwadzebl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ywan-chungtsiang.top/gtxoweclcp.html

TS:   arr.map(String)
来源：http://hz.jiagoushi.top/gtwuxnxjnc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yuxming.cn/gtktxqgvbb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj20258.top/gthqptmnxj.html

Ruby: arr.map(&:upcase)
来源：http://hz.tianlin.xyz/gtxdoycvuj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.guannengcc.top/gtiftljoqd.html

[C08] 闭包
来源：http://hz.yonumen.top/gtauhrourq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yvedp.cn/gtlcknnshv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gaohongyu789.top/gtntzwxhga.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtvgletnnc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtjgzusmwj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.bjfxy.top/gtyldthqri.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hysaishi.cn/gtxhrrjavq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.andypj.xyz/gtqmrkahqw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtpiytenne.html

[C09] 递归
来源：http://hz.wangdashe.top/gttmyfcbqp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.fengsongda.top/gtlfqgdlgu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.daria6918.cn/gtlmfyfaxy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pengpengdd.cyou/gtqljjdlnk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dianchejie.cn/gtawlanmpc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jinqigufen.top/gtxqpaoopa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shangyingyoupin.top/gthtaokjee.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tanke756.top/gtnuqcuqvr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hywenlv.cn/gtzfghyayg.html

[C10] 变量作用域
来源：http://hz.cheryme.top/gtwscrcrbk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.fengsongda.top/gtuobzfthq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yueranfly.top/gtrbahtpct.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hnqzz.top/gtabhouwqm.html

TS:   同 JS
来源：http://hz.aizwys.cn/gtelbavwqo.html

Java: 方法内为块级作用域
来源：http://hz.cheryme.top/gtcoweoevl.html

Go:   花括号块级作用域
来源：http://hz.shuidangran.top/gtrghftzor.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xinyue.icu/gtxwitxiov.html

C#:   块级作用域
来源：http://hz.zhixingplan.top/gthvqtbpzy.html

[C11] 模块导入与导出
来源：http://hz.daria6918.cn/gtkkbboick.html

Py:   from module import func
来源：http://hz.gogol.net.cn/gtjevlnjnm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yongpay.top/gtdjssatos.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.redwolf501.top/gtumbdqfid.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhaomingkeji.xyz/gtlueerwal.html

Java: import java.util.List;
来源：http://hz.52xcode.cn/gtxpwwwvul.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinyuanbaomall.cn/gtejdlzwhl.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.c1oappe.top/gtpzujgvqj.html

C#:   using System.Text;
来源：http://hz.zhijiandao.cn/gtjwzqwswy.html

[C12] 立即执行函数 IIFE
来源：http://hz.iojbl.cn/gtvjibwkct.html

Py:   (lambda: print("run"))()
来源：http://hz.zhaomingkeji.xyz/gteqaazddw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ehwqpu.com/gtbqxhaplu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinghuilouyu.cn/gtjnsshbsr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cucudq.cn/gtbnicjxnx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj20258.top/gtdmtsausd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hfpthk.cn/gtujbnnpgl.html

Ruby: -> { puts "run" }.call
来源：http://hz.pycfn.com/gtsbskanxw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj202588.top/gtneacewid.html

[C13] 类型声明 / 类型注解
来源：http://hz.hfpthk.cn/gtwenwwvyb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.haohaochexian.top/gtmtfiukkp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtugzlqnff.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.redwolf501.top/gtxndnvoed.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydzc1.top/gtxefxwelk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shzxlz.cn/gtpstbtody.html

Go:   func add(a, b int) int
来源：http://hz.chenlongwang.top/gtlasxlqhy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jianghu66.top/gtengrbabk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.fengsongda.top/gtujpjjtkl.html

[C14] 泛型函数
来源：http://hz.hammf.cn/gtfzrixgsi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gtelqfgedp.html

PHP:  // 无泛型
来源：http://hz.zhixingplan.top/gtnjgdfxmm.html

JS:   // 无泛型
来源：http://hz.yvedp.cn/gtzajhpmdy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhongyouzk.top/gtamfgymbw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.guannengcc.top/gtkrgocfrz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.guannengcc.top/gtbdoneyzh.html

Ruby: # 无泛型
来源：http://hz.gaohongyu789.top/gtgmkotuud.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shanyushiyangtech.top/gtwhesfaxx.html

[C15] 解构 / 展开参数
来源：http://hz.gogol.net.cn/gtxdcnehjn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shanyushiyangtech.top/gtxvcfncvx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aibaodan.cn/gtwvzdvhtm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinghuilouyu.cn/gtyjpuflkq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yangfankeji.com/gtzhgvwqyc.html

Java: // 无解构
来源：http://hz.zhengqikj.top/gteuxgwtqi.html

Go:   // 无解构
来源：http://hz.9152youxi.cn/gtgeahcvwb.html

Ruby: a, b = pair
来源：http://hz.andypj.xyz/gtjvkdmrka.html

C#:   var (a, b) = pair;
来源：http://hz.gzhubu.top/gtihcvvryr.html

[C16] 函数 / 方法重载
来源：http://hz.cqqwz.cn/gtyjfluwtb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xuanzx.com/gtxxhtwaid.html

PHP:  // 无重载
来源：http://hz.tanke756.top/gtncrzwpwh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.bjfxy.top/gtjahncfke.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ehwqpu.com/gtpzaxahpb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.vqdsnc.cn/gtpfyxcfpb.html

Go:   // 无重载：用不同函数名
来源：http://hz.cdnleiting.top/gtsfpeyvsq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.aizwys.cn/gtmsebsjon.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shanyushiyangtech.top/gtonwgcddv.html

================================================================================
来源：http://hz.tianlin.xyz/gtwmgnwmgt.html

D. 数组 / 列表 / 集合
来源：http://hz.ppjwa.cn/gtpcxbeysc.html

================================================================================
来源：http://hz.yvedp.cn/gtdtbabcjx.html

[D01] 创建数组 / 列表
来源：http://hz.chenjidiqi.icu/gtkzhwsrkr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ydjk.org.cn/gtymfjlvyi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.vqdsnc.cn/gtvxgvwfnf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cdnleiting.top/gtbbslajzq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.meibo888.top/gtillmqmls.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ppjwa.cn/gtulpdmpty.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shuidangran.top/gtbcghjrhx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nwbrower.top/gtushbzcjs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenzaomai.com/gtqyretlox.html

[D02] 追加元素到末尾
来源：http://hz.smart0.xyz/gtnvrjfobr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhoulong.xyz/gtsbcxakvy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ehwqpu.com/gtjvvhccdw.html

JS:   arr.push(4);
来源：http://hz.mhx1999.top/gtrisaeijr.html

TS:   arr.push(4);
来源：http://hz.gotoacloud.top/gthgqnlmeg.html

Java: list.add(4);
来源：http://hz.hammf.cn/gttxyvnyha.html

Go:   arr = append(arr, 4)
来源：http://hz.ydzc1.top/gtetkmxqcz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hongshengwenyu.top/gtrbotmihz.html

C#:   list.Add(4);
来源：http://hz.hnxiangtu.top/gtgwfezunm.html

[D03] 在指定位置插入元素
来源：http://hz.tian-w.cn/gtkraiwhrp.html

Py:   arr.insert(0, 0)
来源：http://hz.nwbrower.top/gtxrebsblq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sufxvd.cn/gtvrlieedj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xylfe.cn/gtfjugguaa.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sxryk.cn/gtozqfvuar.html

Java: list.add(0, 0);
来源：http://hz.yuanzhike.top/gttvcmdulf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shzxlz.cn/gtozdlixtv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jianghu66.top/gtdmcqgflc.html

C#:   list.Insert(0, 0);
来源：http://hz.yangfankeji.com/gtyocvuspb.html

[D04] 删除元素
来源：http://hz.jianghu66.top/gtfjlkcdyl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gzhubu.top/gtyedpkdfh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenjidiqi.icu/gtvuvudrwh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hywenlv.cn/gtsbepglvk.html

TS:   arr.splice(0, 1);
来源：http://hz.snrcjt.cn/gtbloenqce.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yueranfly.top/gtjxccljqs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zycfv.cn/gtinuorcbr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nwbrower.top/gtexgezbeb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinghuilouyu.cn/gtvdrjizzt.html

[D05] 访问与修改元素
来源：http://hz.ydzc1.top/gtvlydfnvb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtuprnixhu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.0kj1m.cn/gtfdljvtmk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.dianchejie.cn/gtehxcsqnr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhiwuduotai.top/gtwamozlll.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shuidangran.top/gtpalhgypg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtortkrafi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gtnjejyaea.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hammf.cn/gtxolujhbf.html

[D06] 数组长度
来源：http://hz.xziqi.cn/gtgfzhfdtc.html

Py:   len(arr)
来源：http://hz.guowangkeji.top/gtohfjjypp.html

PHP:  count($arr);
来源：http://hz.jianghu66.top/gtlyuvkafc.html

JS:   arr.length
来源：http://hz.birdmap.top/gtfywuzmry.html

TS:   arr.length
来源：http://hz.shangyingyoupin.top/gtomlzxqzr.html

Java: list.size();
来源：http://hz.redwolf501.top/gtwrdhkqcy.html

Go:   len(arr)
来源：http://hz.ydjk.org.cn/gtisrcsmrn.html

Ruby: arr.length; arr.size
来源：http://hz.guowangkeji.top/gtgoryigdz.html

C#:   list.Count;
来源：http://hz.ydzc1.top/gtmchazrtb.html

[D07] 切片 / 取子数组
来源：http://hz.guowangkeji.top/gtkisyeror.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.svipenyu.cn/gtmzhfckyc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tanke756.top/gtdaticmkz.html

JS:   arr.slice(1, 4);
来源：http://hz.jinghuilouyu.cn/gtqejzqqdz.html


<!-- 参考信息 -->