代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.gotoacloud.top/gtibciwsmw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xingfuxueyuan.xyz/gtoobtbadb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.guowangkeji.top/gtzarluohi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.havefunace.top/gtgxvnyttk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ywan-chungtsiang.top/gtdgasbhsc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.nanxinkj.top/gtwgbczqkj.html

[B11] 生成数字序列 / 区间
来源：http://hz.jqgfzy.top/gtogzmpzmk.html

Py:   list(range(0, 10, 2))
来源：http://hz.52xcode.cn/gtufpoyvjj.html

PHP:  range(0, 10, 2);
来源：http://hz.yuxming.cn/gtchrdtpqi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shangyingyoupin.top/gthkaocpep.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zdqjudy.top/gtbofqqvyz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hongshengwenyu.top/gtnlcrekex.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj20258.top/gtfzcufzuo.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hongshengwenyu.top/gthspuucru.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.guannengcc.top/gtgotwzrty.html

[B12] 跳出多层循环
来源：http://hz.zdqjudy.top/gtanseswdq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.c1oappe.top/gttqcnoihx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.quarkkingdee.top/gtqofoubdg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.pengpengdd.cyou/gtwqzbkyiv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.havefunace.top/gttafhqmue.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yongpay.top/gtozlxnbqw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yongpay.top/gtkfvhoiss.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.havefunace.top/gtqayntfzv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xziqi.cn/gthgyvzlaa.html

[B13] 判断是否为数字
来源：http://hz.ydjk.org.cn/gttbakturw.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinghuilouyu.cn/gtvfvduian.html

PHP:  is_numeric($x)
来源：http://hz.hywenlv.cn/gterxjtnwc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhijiandao.cn/gtlseojnbf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shuidangran.top/gtlighlywx.html

Java: x instanceof Number
来源：http://hz.ivvv.top/gtiggthoys.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sxryk.cn/gtaachlzld.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhongyouzk.top/gtucxlepta.html

C#:   x is int or double or decimal
来源：http://hz.zhengqikj.top/gtckiowmbv.html

[B14] 判断值是否在集合内
来源：http://hz.wangdashe.top/gtdpajtjsb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ydzc1.top/gtccnomdmj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.chenjidiqi.icu/gtgyhdpagh.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.andypj.xyz/gtvifjbmuf.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.dashuyun.cn/gtwpcltpsj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.shzxlz.cn/gtcoeztcwn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shanyushiyangkeji.top/gtajcnvdmc.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yuxming.cn/gtsqvotnhe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinqigfzy.top/gtjclkjoge.html

[B15] 布尔运算与取反
来源：http://hz.wangdashe.top/gtuxyskpfj.html

Py:   a and b or not c
来源：http://hz.yj20258.top/gtemexmmvi.html

PHP:  $a && $b || !$c
来源：http://hz.ivvv.top/gtgeanexdp.html

JS:   a && b || !c
来源：http://hz.ybcxt.top/gtggavzkjc.html

TS:   a && b || !c
来源：http://hz.chenjidiqi.icu/gtdnqzglek.html

Java: a && b || !c
来源：http://hz.jinqigufen.top/gttxuivccb.html

Go:   a && b || !c
来源：http://hz.chenjidiqi.icu/gtxdutujla.html

Ruby: a && b || !c
来源：http://hz.cheryme.top/gttlyqownk.html

C#:   a && b || !c
来源：http://hz.0kj1m.cn/gtrrbcooaa.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.redwolf501.top/gtrldoatxf.html

Py:   if not data: return
来源：http://hz.jlsjyb.cn/gthjsvmfqg.html

PHP:  if (!$data) { return; }
来源：http://hz.yj20258.top/gtjxbrcpeq.html

JS:   if (!data) return;
来源：http://hz.nanxuanxn.top/gtsipndceb.html

TS:   if (!data) return;
来源：http://hz.316326.xyz/gtzdpmckex.html

Java: if (data == null) return;
来源：http://hz.yueranfly.top/gtqcnfctqx.html

Go:   if data == nil { return }
来源：http://hz.feifeiyinyue.top/gtndszznsr.html

Ruby: return if data.nil?
来源：http://hz.ybcxt.top/gtzponcxnb.html

C#:   if (data == null) return;
来源：http://hz.gotoacloud.top/gthjonscfy.html

================================================================================
来源：http://hz.yuanzhike.top/gtqzblcucj.html

C. 函数与作用域
来源：http://hz.yongpay.top/gtczhxkwhl.html

================================================================================
来源：http://hz.jinqigufen.top/gtwnkarrwc.html

[C01] 定义函数
来源：http://hz.jiagoushi.top/gtschutngf.html

Py:   def add(a, b): return a + b
来源：http://hz.yuanzhike.top/gtvdgdccsx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gtzqupnppb.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.sxryk.cn/gtedxtsave.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.havefunace.top/gtvoeevejr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.0kj1m.cn/gthswinhkh.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhiwuduotai.top/gtclcgmxem.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hfpthk.cn/gtpyomibcx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jlsjyb.cn/gtliagkptx.html

[C02] 默认参数
来源：http://hz.ppjwa.cn/gtcppvcxuj.html

Py:   def greet(name="World"): return name
来源：http://hz.haohaochexian.top/gtqbgpwikb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cucudq.cn/gtjckggzzg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hysaishi.cn/gtqnkrzekn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cqqwz.cn/gtymdzgand.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xylfe.cn/gtpdeorfnb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.aibaodan.cn/gtsotrcpyt.html

Ruby: def greet(name = "World") = name
来源：http://hz.wangshuangyany.cn/gtwoequvac.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinyuanbaomall.cn/gtrqoozqgl.html

[C03] 可变参数
来源：http://hz.sxryk.cn/gtkqbjcrxy.html

Py:   def total(*args): return sum(args)
来源：http://hz.svipenyu.cn/gtlkpxtasu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhiwuduotai.top/gtmhptohhg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aizwys.cn/gtlyuoesgr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xinyue.icu/gtesjkgcnn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.guowangkeji.top/gtoeocjchs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhiwuduotai.top/gthvhqtrlw.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sufxvd.cn/gtfiqrjzch.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhengqikj.top/gtrgszrauy.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yonumen.top/gtsybmdagi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yongpay.top/gtjvofgqqm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.guowangkeji.top/gthimpoozw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cdnleiting.top/gtpiqqfklx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhixingplan.top/gtjkqzgudj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yueranfly.top/gtnslsunva.html

Go:   // 无：用配置结构体参数
来源：http://hz.birdmap.top/gtwcrhccnk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xingfuxueyuan.xyz/gtxkjgjxph.html

C#:   f(a: 1, b: 2)
来源：http://hz.yangfankeji.com/gtdimlufiq.html

[C05] 返回多个值
来源：http://hz.kuanghao11.cn/gtfhjqtcrc.html

Py:   return a, b
来源：http://hz.hnqzz.top/gtjjlcbdav.html

PHP:  return [$a, $b];
来源：http://hz.shanyushiyangtech.top/gthverpbpm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xingfuxueyuan.xyz/gtykildsud.html

TS:   return { a, b };
来源：http://hz.ydjk.org.cn/gtzbyowusw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shanyushiyangtech.top/gtnwrmpbhq.html

Go:   return a, b
来源：http://hz.chenlongwang.top/gtwdrdoyfx.html

Ruby: return a, b
来源：http://hz.wangshuangyany.cn/gtufydbhvh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cucudq.cn/gtajczznhi.html

[C06] 匿名函数 / lambda
来源：http://hz.hysaishi.cn/gtdcujrxyu.html

Py:   square = lambda x: x * x
来源：http://hz.pengpengdd.cyou/gtcysrasip.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yvedp.cn/gthtduwuly.html

JS:   const square = x => x * x;
来源：http://hz.wangdashe.top/gtqerrknrb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cqqwz.cn/gtoasudiog.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.birdmap.top/gtwfinkhzk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gaohongyu789.top/gtkxrmbrdc.html

Ruby: square = ->(x) { x * x }
来源：http://hz.iojbl.cn/gtfltfbtep.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shzxlz.cn/gtopzamuiz.html

[C07] 把函数作为参数传入
来源：http://hz.andypj.xyz/gtjgwrrpwb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yuxming.cn/gtqcbzjnyg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jqgfzy.top/gtwbucgggl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.nanxuanxn.top/gtmhtlpmyv.html

TS:   arr.map(String)
来源：http://hz.pengpengdd.cyou/gtcqplhuxy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.havefunace.top/gtjfhmhoat.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jqgfzy.top/gtpbgngurb.html

Ruby: arr.map(&:upcase)
来源：http://hz.ydjk.org.cn/gtblthgdga.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.birdmap.top/gtljsbtmvj.html

[C08] 闭包
来源：http://hz.gotoacloud.top/gtirmbxjrd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.vqdsnc.cn/gtitkihlxb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.chenzaomai.com/gtnzqxzcel.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.feifeiyinyue.top/gtyqhxgdjn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hywenlv.cn/gtqeeprbpb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.iojbl.cn/gtjxgjqhws.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shzxlz.cn/gtkarqdxfn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jianghu66.top/gtwrulqlqy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtjquffajz.html

[C09] 递归
来源：http://hz.birdmap.top/gtlowjkjev.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yanxiufei.cn/gtsgurrfja.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yj202588.top/gtciszydqp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gaohongyu789.top/gtawsgnvod.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xinyue.icu/gtbcfrgvke.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zycfv.cn/gtnepovufa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ydjk.org.cn/gtwjdtpbgs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hongshengwenyu.top/gtrowjecuo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yonumen.top/gtytoumlkq.html

[C10] 变量作用域
来源：http://hz.aibaodan.cn/gtdchatpsk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhaomingkeji.xyz/gtbcitsrog.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.9152youxi.cn/gteonmrlnq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.guowangkeji.top/gtigixbhjv.html

TS:   同 JS
来源：http://hz.ydjk.org.cn/gtjbmkywav.html

Java: 方法内为块级作用域
来源：http://hz.yj202588.top/gtzlxqapih.html

Go:   花括号块级作用域
来源：http://hz.bjfxy.top/gtbvjplygn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.0kj1m.cn/gtjbfdpbnr.html

C#:   块级作用域
来源：http://hz.316326.xyz/gtjuafgmks.html

[C11] 模块导入与导出
来源：http://hz.ehwqpu.com/gtqtffolaq.html

Py:   from module import func
来源：http://hz.wangshuangyany.cn/gthjvhwnsn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.haohaochexian.top/gtmcuiniyo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yuxming.cn/gttaoojbfx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cheryme.top/gtfkftzvre.html

Java: import java.util.List;
来源：http://hz.daria6918.cn/gtgvoydlkb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gaohongyu789.top/gtwhbkabqo.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.andypj.xyz/gtldbkbvrc.html

C#:   using System.Text;
来源：http://hz.zhoulong.xyz/gtmxhxnhtn.html

[C12] 立即执行函数 IIFE
来源：http://hz.jyoumei.cn/gtmernqirn.html

Py:   (lambda: print("run"))()
来源：http://hz.gaohongyu789.top/gtcursivzi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.guannengcc.top/gtbrkuioby.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yangfankeji.com/gtgcizwgxz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zdqjudy.top/gtmpwdzabp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.pengpengdd.cyou/gtzefynemm.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.meibo888.top/gthjhfujkt.html

Ruby: -> { puts "run" }.call
来源：http://hz.hammf.cn/gtkhluardx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hysaishi.cn/gttdxkhlke.html

[C13] 类型声明 / 类型注解
来源：http://hz.quarkkingdee.top/gtravstapj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.9152youxi.cn/gtwonebhro.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtpmatgzlx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yongpay.top/gtfmxkmrbv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuxming.cn/gtiewautnu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.svipenyu.cn/gtadjtayid.html

Go:   func add(a, b int) int
来源：http://hz.zhoulong.xyz/gtzroonmlw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinghuilouyu.cn/gtjwciduew.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj20258888.top/gtdzxmarmi.html

[C14] 泛型函数
来源：http://hz.cqqwz.cn/gtmolwysdz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ybcxt.top/gtwtfeeysd.html

PHP:  // 无泛型
来源：http://hz.52xcode.cn/gtjovrntuz.html

JS:   // 无泛型
来源：http://hz.ywan-chungtsiang.top/gtbhdxjchs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhengqikj.top/gtffdrymro.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yuxming.cn/gtgtiqjyzs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xingfuxueyuan.xyz/gtpxvvdvor.html

Ruby: # 无泛型
来源：http://hz.tianlin.xyz/gtfmusrhza.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sweek.top/gtytigkrwt.html

[C15] 解构 / 展开参数
来源：http://hz.tianlin.xyz/gtrinfivgq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.chenzaomai.com/gtxvjsmomh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jqgfzy.top/gtwwugqcoa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258.top/gtcpnvgmry.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.haohaochexian.top/gtffmlhxyv.html

Java: // 无解构
来源：http://hz.zhengqikj.top/gtjbxdpvdn.html

Go:   // 无解构
来源：http://hz.zhoulong.xyz/gtoqfwtlhr.html

Ruby: a, b = pair
来源：http://hz.c1oappe.top/gtvwmaokfd.html

C#:   var (a, b) = pair;
来源：http://hz.chenzaomai.com/gtqpckuwjx.html

[C16] 函数 / 方法重载
来源：http://hz.feifeiyinyue.top/gtupjhuzen.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jiagoushi.top/gtmvojjbzo.html

PHP:  // 无重载
来源：http://hz.cqqwz.cn/gtzlmfynjw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zdqjudy.top/gtptthgrhe.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cheryme.top/gthkucpiva.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zdqjudy.top/gtbiiicxxd.html

Go:   // 无重载：用不同函数名
来源：http://hz.316326.xyz/gtatqpgtxm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xinyue.icu/gtsskfavib.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.guannengcc.top/gtaztyovxp.html

================================================================================
来源：http://hz.xziqi.cn/gtzpqyuqrd.html

D. 数组 / 列表 / 集合
来源：http://hz.yuxming.cn/gtxixboiup.html

================================================================================
来源：http://hz.yuxming.cn/gtknerarqa.html

[D01] 创建数组 / 列表
来源：http://hz.cashguo.top/gtdsvlrxjd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ywan-chungtsiang.top/gththtdtpk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.316326.xyz/gtwqyxvleq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinghuilouyu.cn/gtutioxpbe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhoulong.xyz/gtsxniqrwh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.quarkkingdee.top/gtfluuaogk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sxryk.cn/gttlcmkbjt.html

Ruby: arr = [1, 2, 3]
来源：http://hz.andypj.xyz/gtxrwvbwdk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shzxlz.cn/gtomrviyiu.html

[D02] 追加元素到末尾
来源：http://hz.jinqigfzy.top/gtzgnikunj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenzaomai.com/gtwpnfbhkf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgufenzy.top/gtkhdsyehm.html

JS:   arr.push(4);
来源：http://hz.yj202588.top/gtxhxkrcap.html

TS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtypbgxnoa.html

Java: list.add(4);
来源：http://hz.tian-w.cn/gtyqannoid.html

Go:   arr = append(arr, 4)
来源：http://hz.zhongyouzk.top/gtykmasfpl.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.guannengcc.top/gtuwkcjaoo.html

C#:   list.Add(4);
来源：http://hz.xingfuxueyuan.xyz/gtjddnsppi.html

[D03] 在指定位置插入元素
来源：http://hz.smart0.xyz/gtfmhoyrrv.html

Py:   arr.insert(0, 0)
来源：http://hz.yangfankeji.com/gtfjjcgqki.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nanxuanxn.top/gtnvktepsd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.fengsongda.top/gtqsaphhjp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ehwqpu.com/gtnxgopvkz.html

Java: list.add(0, 0);
来源：http://hz.pengpengdd.cyou/gtlfyvrdtb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sufxvd.cn/gtyshkndhv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.mhx1999.top/gtuapcggaa.html

C#:   list.Insert(0, 0);
来源：http://hz.fengsongda.top/gtvtxagdfe.html

[D04] 删除元素
来源：http://hz.gogol.net.cn/gtagdtlxny.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuanzx.com/gtoogcdpwo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yuxming.cn/gtaapxnoau.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pengpengdd.cyou/gtryvsnmyk.html

TS:   arr.splice(0, 1);
来源：http://hz.pycfn.com/gtqukrrezl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shanyushiyangkeji.top/gtaqzssrkl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.smart0.xyz/gtbqrxhexl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhongyouzk.top/gtvlaikwmb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.tanke756.top/gtqmsfcqvs.html

[D05] 访问与修改元素
来源：http://hz.mhx1999.top/gtquwwenyq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtxjvzyllx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj202588.top/gtlsxhequg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.iojbl.cn/gtbpdkzwzt.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhiwuduotai.top/gtzqnutswr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shuidangran.top/gthzlkypdr.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtstbanovv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cashguo.top/gtqfgltnqg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jlsjyb.cn/gtwcyyuoel.html

[D06] 数组长度
来源：http://hz.ydjk.org.cn/gtyvezjnvt.html

Py:   len(arr)
来源：http://hz.hfpthk.cn/gtylbpenhl.html

PHP:  count($arr);
来源：http://hz.jlsjyb.cn/gtewftcbix.html

JS:   arr.length
来源：http://hz.316326.xyz/gtqjtkjrie.html

TS:   arr.length
来源：http://hz.sysykeji.top/gtoyplrcsf.html

Java: list.size();
来源：http://hz.zhongyouzk.top/gtvisjroqz.html

Go:   len(arr)
来源：http://hz.yj20258888.top/gtpbmzzdyu.html

Ruby: arr.length; arr.size
来源：http://hz.jqgfzy.top/gtwqzxctlf.html

C#:   list.Count;
来源：http://hz.cashguo.top/gtxwcswsts.html

[D07] 切片 / 取子数组
来源：http://hz.redwolf501.top/gttqfijyji.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jianghu66.top/gtamxjfsuv.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.0kj1m.cn/gtjzwulats.html

JS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtmxilhovz.html

TS:   arr.slice(1, 4);
来源：http://hz.havefunace.top/gtasojrkpc.html

Java: list.subList(1, 4);
来源：http://hz.ivvv.top/gtntzzvtlh.html

Go:   arr[1:4]
来源：http://hz.guannengcc.top/gtvvghaqhv.html

Ruby: arr[1, 3]
来源：http://hz.jyoumei.cn/gtzwpxetaz.html

C#:   list.GetRange(1, 3);
来源：http://hz.yuxming.cn/gthcothnjt.html

[D08] 合并两个数组
来源：http://hz.hysaishi.cn/gtvdgjxmok.html

Py:   a + b;  a.extend(b)
来源：http://hz.shuidangran.top/gtqzzarphz.html

PHP:  array_merge($a, $b);
来源：http://hz.jqgfzy.top/gtihqufibl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.wangdashe.top/gtxpvjyewm.html

TS:   [...a, ...b];
来源：http://hz.shanyushiyangkeji.top/gtsebamysy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.daria6918.cn/gtkakxsewh.html

Go:   append(a, b...)
来源：http://hz.yueranfly.top/gtpabhfepv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hammf.cn/gtjvvcoxro.html

C#:   a.Concat(b).ToList()
来源：http://hz.ydzc1.top/gtdibnxtry.html

[D09] 排序（升序）
来源：http://hz.gaohongyu789.top/gtvjpvxiub.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtmgtqkzcm.html

PHP:  sort($arr);
来源：http://hz.yuanzhike.top/gtfauoeqqo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gogol.net.cn/gtkbiisyoi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.wangshuangyany.cn/gtvvoysvos.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sufxvd.cn/gtjpqrwhwa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.smart0.xyz/gtemvjkzjs.html

Ruby: arr.sort
来源：http://hz.xuanzx.com/gtcjlasrbp.html

C#:   list.Sort();
来源：http://hz.zhiwuduotai.top/gtouyyowlz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gogol.net.cn/gtlmtjtbar.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.0kj1m.cn/gtpjrsbpwk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shuidangran.top/gtyjmfluou.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuetiantiany.cn/gtdqiqpcmc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.smart0.xyz/gtetsqqhxp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.chenzaomai.com/gtjxjodznu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinqigfzy.top/gtdnkeekjt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jyoumei.cn/gtlucgjtrg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenjidiqi.icu/gtoucmuotf.html


<!-- 参考信息 -->