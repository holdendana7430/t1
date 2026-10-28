代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://hz.sweek.top/gtshpsibfe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.guannengcc.top/gtncbfqekc.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.gogol.net.cn/gteyfuvsih.html

C#:   do { i++; } while (i < 10);
来源：http://hz.aibaodan.cn/gtvzdoxagv.html

[B09] break 与 continue
来源：http://hz.gogol.net.cn/gtmrpfazkt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gotoacloud.top/gtnxwgnjsx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.gzhubu.top/gtoigqjqlc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gteziyjdll.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhongyouzk.top/gttgsinjec.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jianghu66.top/gtyhzdclum.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhoulong.xyz/gtiiisdmrd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.feifeiyinyue.top/gtujsdkqaz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtgcxdtklx.html

[B10] 遍历同时拿索引
来源：http://hz.aizwys.cn/gtxacwnzwd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.hnxiangtu.top/gtgitwqtsj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zdqjudy.top/gtbpnuxzpt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hammf.cn/gtgbwusnns.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hnqzz.top/gtbpygbsgt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hywenlv.cn/gteycbqugi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.vqdsnc.cn/gtyysormfq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.chenzaomai.com/gttmkhthmp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.kuanghao11.cn/gtwbmllhxf.html

[B11] 生成数字序列 / 区间
来源：http://hz.zhixingplan.top/gtzepxpyrf.html

Py:   list(range(0, 10, 2))
来源：http://hz.yongpay.top/gtcfaqysga.html

PHP:  range(0, 10, 2);
来源：http://hz.tanke756.top/gtnkkkmapl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.feifeiyinyue.top/gtynhmvoga.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guannengcc.top/gtukjgaroq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.sweek.top/gtqycftvqh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.tianlin.xyz/gtocsfjeoj.html

Ruby: (0...10).step(2).to_a
来源：http://hz.andypj.xyz/gtcbycbafb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.tanke756.top/gtatfrcqjw.html

[B12] 跳出多层循环
来源：http://hz.yuxming.cn/gtvhnfocjn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nanxuanxn.top/gthmgvcfap.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hnqzz.top/gttpuqqkin.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuanzhike.top/gtejneoagz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yanxiufei.cn/gtneslinhc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.sxryk.cn/gtghrnuorx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jiagoushi.top/gtetqrcnyz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cashguo.top/gtvsyhcpqg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.aizwys.cn/gtgozgqtss.html

[B13] 判断是否为数字
来源：http://hz.ppjwa.cn/gtowyhgrvh.html

Py:   isinstance(x, (int, float))
来源：http://hz.shuidangran.top/gtkmcghkkc.html

PHP:  is_numeric($x)
来源：http://hz.nanxuanxn.top/gtfislpuox.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.52xcode.cn/gtyqeqwlwi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sysykeji.top/gtlrjbuyrh.html

Java: x instanceof Number
来源：http://hz.xylfe.cn/gtaarthctg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.redwolf501.top/gtwvismnqx.html

Ruby: x.is_a?(Numeric)
来源：http://hz.redwolf501.top/gtprnulgsq.html

C#:   x is int or double or decimal
来源：http://hz.wangdashe.top/gthyxeebxk.html

[B14] 判断值是否在集合内
来源：http://hz.havefunace.top/gtilqlgytx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jlsjyb.cn/gteuaucayv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ehwqpu.com/gtvobswofi.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.chenlongwang.top/gtricvkntp.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zycfv.cn/gtamrwxqzg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.shangyingyoupin.top/gtqywbutca.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.chenzaomai.com/gtsjxddbtv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ybcxt.top/gtyrmvuoaa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.redwolf501.top/gtkkckoiay.html

[B15] 布尔运算与取反
来源：http://hz.yj202588.top/gtxscgkisy.html

Py:   a and b or not c
来源：http://hz.xingfuxueyuan.xyz/gtrnvajthx.html

PHP:  $a && $b || !$c
来源：http://hz.sxryk.cn/gtecqszbfk.html

JS:   a && b || !c
来源：http://hz.meibo888.top/gtnmwbobjy.html

TS:   a && b || !c
来源：http://hz.gzhubu.top/gthyxyljvx.html

Java: a && b || !c
来源：http://hz.shanyushiyangtech.top/gtvzqamrde.html

Go:   a && b || !c
来源：http://hz.iojbl.cn/gtmklprmqi.html

Ruby: a && b || !c
来源：http://hz.zycfv.cn/gtcfiddjlk.html

C#:   a && b || !c
来源：http://hz.ybcxt.top/gtnvxrcwnd.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hnqzz.top/gtpumdptpe.html

Py:   if not data: return
来源：http://hz.zhijiandao.cn/gtbbjezuin.html

PHP:  if (!$data) { return; }
来源：http://hz.yonumen.top/gtlqlsckcl.html

JS:   if (!data) return;
来源：http://hz.jianghu66.top/gtjxlwkfzx.html

TS:   if (!data) return;
来源：http://hz.xuetiantiany.cn/gtbmxeslac.html

Java: if (data == null) return;
来源：http://hz.tian-w.cn/gtczrcgzcu.html

Go:   if data == nil { return }
来源：http://hz.316326.xyz/gtcozndckx.html

Ruby: return if data.nil?
来源：http://hz.pengpengdd.cyou/gtjyyraxfk.html

C#:   if (data == null) return;
来源：http://hz.hammf.cn/gtfkwliras.html

================================================================================
来源：http://hz.yueranfly.top/gtjucdjufd.html

C. 函数与作用域
来源：http://hz.kuanghao11.cn/gtyuohfpwp.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtemfbxvox.html

[C01] 定义函数
来源：http://hz.redwolf501.top/gtmahsyypn.html

Py:   def add(a, b): return a + b
来源：http://hz.daria6918.cn/gtnmbxjmxz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cashguo.top/gtnozkehro.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gzhubu.top/gtpmoenkup.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sweek.top/gtkpzmogiv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yonumen.top/gtauhdkzkb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jlsjyb.cn/gtqiwhuliv.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ydjk.org.cn/gtgvbuowrk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hammf.cn/gtukurvkcm.html

[C02] 默认参数
来源：http://hz.gotoacloud.top/gtocsjmdgw.html

Py:   def greet(name="World"): return name
来源：http://hz.gogol.net.cn/gtzmfpyfpj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.chenzaomai.com/gtwkpdzipa.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shangyingyoupin.top/gtojqxxfeq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhiwuduotai.top/gthbnpxbyo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hysaishi.cn/gtzqbnyggg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shzxlz.cn/gtibezlesm.html

Ruby: def greet(name = "World") = name
来源：http://hz.nwbrower.top/gtrahbzgvz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cucudq.cn/gtbiljvjra.html

[C03] 可变参数
来源：http://hz.pycfn.com/gtftgruoao.html

Py:   def total(*args): return sum(args)
来源：http://hz.redwolf501.top/gtstjzzaga.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.pycfn.com/gtckznwoct.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guowangkeji.top/gtdmgfwwqb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinqigfzy.top/gthpdhshbj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hywenlv.cn/gtdcwvwgns.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhaomingkeji.xyz/gthgufdxsq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jianghu66.top/gtjdsyfjjf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hnxiangtu.top/gttpwhrrkv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cheryme.top/gtmzgfzmnr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hysaishi.cn/gtvycacrkn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yanxiufei.cn/gtvposdwtx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gaohongyu789.top/gthlpvzdzo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hywenlv.cn/gthkzyqacn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.tian-w.cn/gttxvjnhmj.html

Go:   // 无：用配置结构体参数
来源：http://hz.shanyushiyangkeji.top/gtxrqljetc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.nanxinkj.top/gtuvkkpbig.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangshuangyany.cn/gtapooaedg.html

[C05] 返回多个值
来源：http://hz.wangshuangyany.cn/gtzvuqciwj.html

Py:   return a, b
来源：http://hz.fzhhl.top/gtfenjrtaa.html

PHP:  return [$a, $b];
来源：http://hz.aibaodan.cn/gtggzobwbe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhijiandao.cn/gtydtvliwj.html

TS:   return { a, b };
来源：http://hz.ydzc1.top/gtcrbpdevp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.feifeiyinyue.top/gtjhnlakxm.html

Go:   return a, b
来源：http://hz.kuanghao11.cn/gtmimmhazk.html

Ruby: return a, b
来源：http://hz.yangfankeji.com/gtydtygdud.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.tanke756.top/gtaczunhjo.html

[C06] 匿名函数 / lambda
来源：http://hz.shuidangran.top/gtivoittwd.html

Py:   square = lambda x: x * x
来源：http://hz.xinyue.icu/gtcbszcwtj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zycfv.cn/gtteknwblh.html

JS:   const square = x => x * x;
来源：http://hz.pycfn.com/gtgorbkjfz.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.fengsongda.top/gtxfrftlce.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.cheryme.top/gttdwgiqjj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.snrcjt.cn/gthdinigsb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhiwuduotai.top/gtkloduhzb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gzhubu.top/gtmxgynjlh.html

[C07] 把函数作为参数传入
来源：http://hz.yangfankeji.com/gtexgxeoks.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hysaishi.cn/gtcqhatbum.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ybcxt.top/gtwfsagcrq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinyuanbaomall.cn/gtpxnedpzv.html

TS:   arr.map(String)
来源：http://hz.xinyue.icu/gtpikftxlh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.fzhhl.top/gtmjlmzsxp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yueranfly.top/gtpsorknbp.html

Ruby: arr.map(&:upcase)
来源：http://hz.cashguo.top/gtktuxrsiv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ydzc1.top/gtpwaafoif.html

[C08] 闭包
来源：http://hz.hfpthk.cn/gtouqlozrl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shuidangran.top/gtsxlebhhb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tian-w.cn/gtybtufnjr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtmauuaktr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtqyqxuruu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sweek.top/gthtcenoxj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gotoacloud.top/gtfwwgdtfy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cqqwz.cn/gtjyfvsjul.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtpehgwwmq.html

[C09] 递归
来源：http://hz.chenzaomai.com/gtjbivwtfp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yanxiufei.cn/gtxrqerhcr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenlongwang.top/gthjndcrcy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ehwqpu.com/gtonkxgyyq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tian-w.cn/gtutmlhjed.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yuanzhike.top/gtmuhjdmtu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hysaishi.cn/gtldcyjyip.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.feifeiyinyue.top/gtkgabqnnk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jlsjyb.cn/gtyubxfxlk.html

[C10] 变量作用域
来源：http://hz.hammf.cn/gthqdeujah.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhongyouzk.top/gtfgjjdgkw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xinyue.icu/gtsgskquwn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shangyingyoupin.top/gtjxxotftc.html

TS:   同 JS
来源：http://hz.sysykeji.top/gtzexnhjqy.html

Java: 方法内为块级作用域
来源：http://hz.tian-w.cn/gtkmcjsbdv.html

Go:   花括号块级作用域
来源：http://hz.zhongyouzk.top/gtfblqffzt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yj20258.top/gtoczwpuio.html

C#:   块级作用域
来源：http://hz.fzhhl.top/gtaybomzqj.html

[C11] 模块导入与导出
来源：http://hz.cheryme.top/gtuqqqrijy.html

Py:   from module import func
来源：http://hz.haohaochexian.top/gtbpbvijth.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhengqikj.top/gtpmpvklqd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.pycfn.com/gtgaxpydte.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jqgufenzy.top/gtlauuqdpk.html

Java: import java.util.List;
来源：http://hz.tianlin.xyz/gtimtbhzva.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.chenzaomai.com/gtgaovzngh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.pengpengdd.cyou/gtlwcytozo.html

C#:   using System.Text;
来源：http://hz.snrcjt.cn/gtthxxhlor.html

[C12] 立即执行函数 IIFE
来源：http://hz.cashguo.top/gtctkshmsi.html

Py:   (lambda: print("run"))()
来源：http://hz.yuxming.cn/gtfksnpxxk.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yongpay.top/gthhjiangd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.andypj.xyz/gtortonshg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.dianchejie.cn/gtrymdqkes.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.bjfxy.top/gtstqviugo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cdnleiting.top/gtchjvabxe.html

Ruby: -> { puts "run" }.call
来源：http://hz.jyoumei.cn/gtxoybtzmc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.svipenyu.cn/gtcdehyowo.html

[C13] 类型声明 / 类型注解
来源：http://hz.pycfn.com/gtnkxyxtot.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinghuilouyu.cn/gtoyqytsmc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gtcgzfmakj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuxming.cn/gtqkijjpdh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.havefunace.top/gtdaywsbrz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cucudq.cn/gtiyfgxhqc.html

Go:   func add(a, b int) int
来源：http://hz.xingfuxueyuan.xyz/gtbkxniyjf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.guowangkeji.top/gtbfkwphjo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhaomingkeji.xyz/gtimeeaaqj.html

[C14] 泛型函数
来源：http://hz.zdqjudy.top/gtkkntovip.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.bjfxy.top/gttsxfkdot.html

PHP:  // 无泛型
来源：http://hz.kuanghao11.cn/gtxgzvjkox.html

JS:   // 无泛型
来源：http://hz.ehwqpu.com/gtjumemgwz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yangfankeji.com/gtfbbeukdu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.sysykeji.top/gtcblwbpju.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nanxuanxn.top/gtudinamye.html

Ruby: # 无泛型
来源：http://hz.gzhubu.top/gtqmhufqpo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yonumen.top/gtifoxvqcx.html

[C15] 解构 / 展开参数
来源：http://hz.yuxming.cn/gtywgcybiz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nwbrower.top/gtwkibyovp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.feifeiyinyue.top/gtbhlvpnuw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinqigufen.top/gtodxyeqwn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.daria6918.cn/gtensebmpc.html

Java: // 无解构
来源：http://hz.zhoulong.xyz/gtjqkqysxe.html

Go:   // 无解构
来源：http://hz.yanxiufei.cn/gtnvovtwsw.html

Ruby: a, b = pair
来源：http://hz.xylfe.cn/gtogjdmqie.html

C#:   var (a, b) = pair;
来源：http://hz.yvedp.cn/gttoldieay.html

[C16] 函数 / 方法重载
来源：http://hz.mhx1999.top/gtkbonpmmj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.wangdashe.top/gtajfssdrg.html

PHP:  // 无重载
来源：http://hz.haohaochexian.top/gthlcjcowc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yongpay.top/gtjbfgrvkp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shanyushiyangkeji.top/gtuaodmebh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.andypj.xyz/gtzsnwnstl.html

Go:   // 无重载：用不同函数名
来源：http://hz.fzhhl.top/gtdpngtrqr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ehwqpu.com/gtgcomtnxc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.dianchejie.cn/gtotwnduzm.html

================================================================================
来源：http://hz.aizwys.cn/gtazxotgzn.html

D. 数组 / 列表 / 集合
来源：http://hz.ywan-chungtsiang.top/gtzjnwhixv.html

================================================================================
来源：http://hz.jqgufenzy.top/gtogabaxym.html

[D01] 创建数组 / 列表
来源：http://hz.yj20258.top/gtwayqzkew.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.wangdashe.top/gtazobbojm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.andypj.xyz/gtgdquxumm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xuetiantiany.cn/gtdqicywma.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sweek.top/gtgrnolhrg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guannengcc.top/gtzfrbgmkq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gogol.net.cn/gtjwkjaobn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhiwuduotai.top/gtngoogddf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhiwuduotai.top/gtvgivwuyj.html

[D02] 追加元素到末尾
来源：http://hz.hfpthk.cn/gtevuledip.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jianghu66.top/gtnntdtsoc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.wangshuangyany.cn/gtadweiekk.html

JS:   arr.push(4);
来源：http://hz.tianlin.xyz/gtfodosnfb.html

TS:   arr.push(4);
来源：http://hz.9152youxi.cn/gtdzneqavu.html

Java: list.add(4);
来源：http://hz.feifeiyinyue.top/gtglpnmspn.html

Go:   arr = append(arr, 4)
来源：http://hz.gaohongyu789.top/gtsdrfsode.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.0kj1m.cn/gtlgdedkgc.html

C#:   list.Add(4);
来源：http://hz.zdqjudy.top/gtkxphpayf.html

[D03] 在指定位置插入元素
来源：http://hz.gotoacloud.top/gtfkcpcmnm.html

Py:   arr.insert(0, 0)
来源：http://hz.sxryk.cn/gtcxntkagb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zycfv.cn/gtkhbghlpe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.nwbrower.top/gtuswpgoef.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.vqdsnc.cn/gtrvfsexxj.html

Java: list.add(0, 0);
来源：http://hz.52xcode.cn/gtywbyklfh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.nwbrower.top/gtrkalkgdy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sufxvd.cn/gtxhrnvubd.html

C#:   list.Insert(0, 0);
来源：http://hz.gotoacloud.top/gttjekmpkk.html

[D04] 删除元素
来源：http://hz.jinghuilouyu.cn/gtsfvsnlwu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.guannengcc.top/gtafemmfzw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hongshengwenyu.top/gtxbpzckov.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jqgufenzy.top/gttzjtojmj.html

TS:   arr.splice(0, 1);
来源：http://hz.yongpay.top/gtzzypatio.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zdqjudy.top/gtjcamyhpr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.andypj.xyz/gtaaehfnzn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sysykeji.top/gtdoxrwhzj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.smart0.xyz/gtpgxpsdlr.html

[D05] 访问与修改元素
来源：http://hz.shanyushiyangkeji.top/gtrfpfxyvs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sweek.top/gtbzzvospd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yuanzhike.top/gtwpimievo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jianghu66.top/gtxchgoxnt.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ybcxt.top/gtcfdyidfm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.mhx1999.top/gtcsfpipyt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.wangdashe.top/gtaigerqki.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cashguo.top/gtflhhklls.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.birdmap.top/gtckkjivtk.html

[D06] 数组长度
来源：http://hz.ydzc1.top/gthfjbnzsd.html

Py:   len(arr)
来源：http://hz.yangfankeji.com/gtbgekeiyo.html

PHP:  count($arr);
来源：http://hz.fengsongda.top/gtnbxthhiq.html

JS:   arr.length
来源：http://hz.zhengqikj.top/gtikatrgeu.html

TS:   arr.length
来源：http://hz.yj20258.top/gtszhiwbbe.html

Java: list.size();
来源：http://hz.yvedp.cn/gtoarmmwxb.html

Go:   len(arr)
来源：http://hz.chenzaomai.com/gtspwpsvgu.html

Ruby: arr.length; arr.size
来源：http://hz.tianlin.xyz/gthystuakd.html

C#:   list.Count;
来源：http://hz.0kj1m.cn/gtbkelorao.html

[D07] 切片 / 取子数组
来源：http://hz.xingfuxueyuan.xyz/gtjaqgkdsn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.guannengcc.top/gtzaqrrkjs.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhixingplan.top/gtvmlncoqg.html

JS:   arr.slice(1, 4);
来源：http://hz.shuidangran.top/gtdrnucbsr.html

TS:   arr.slice(1, 4);
来源：http://hz.svipenyu.cn/gtqzjtqxji.html

Java: list.subList(1, 4);
来源：http://hz.smart0.xyz/gttnhswnwr.html

Go:   arr[1:4]
来源：http://hz.yangfankeji.com/gtiftbsaxd.html

Ruby: arr[1, 3]
来源：http://hz.ywan-chungtsiang.top/gthextqnak.html

C#:   list.GetRange(1, 3);
来源：http://hz.jiagoushi.top/gtiqtlowhz.html

[D08] 合并两个数组
来源：http://hz.shanyushiyangkeji.top/gtysreauxo.html

Py:   a + b;  a.extend(b)
来源：http://hz.bjfxy.top/gtfmgwmgvs.html

PHP:  array_merge($a, $b);
来源：http://hz.shanyushiyangtech.top/gtcckltnxe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.0kj1m.cn/gtqiibzret.html

TS:   [...a, ...b];
来源：http://hz.aizwys.cn/gthmehhqjk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.nanxinkj.top/gtbbebbsek.html

Go:   append(a, b...)
来源：http://hz.yj20258888.top/gtnwyyiylt.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sweek.top/gthnvfscnh.html

C#:   a.Concat(b).ToList()
来源：http://hz.kuanghao11.cn/gtjtjopmdc.html

[D09] 排序（升序）
来源：http://hz.kuanghao11.cn/gttwmxjpxq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtfchurblv.html


<!-- 参考信息 -->