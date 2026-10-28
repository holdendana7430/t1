代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtoyavpcpg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.snrcjt.cn/gtxvyftcyp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zycfv.cn/gtvovhqias.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yongpay.top/gtunomoouv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shzxlz.cn/gtkropaldf.html

[B10] 遍历同时拿索引
来源：http://hz.bjfxy.top/gtgjovkzwx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.nanxuanxn.top/gtjtgcpmyl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.fzhhl.top/gtuzjtgtts.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xylfe.cn/gtefkmrycf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xinyue.icu/gtqzplutmk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.9152youxi.cn/gttiiwqvfz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.ydzc1.top/gtbcjnoaib.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jinyuanbaomall.cn/gtjiqyvast.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zycfv.cn/gtufhowujz.html

[B11] 生成数字序列 / 区间
来源：http://hz.zdqjudy.top/gtdahzishz.html

Py:   list(range(0, 10, 2))
来源：http://hz.yvedp.cn/gtfmozxpad.html

PHP:  range(0, 10, 2);
来源：http://hz.nanxuanxn.top/gtsjnltbsq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tanke756.top/gtyeoyvxvk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jiagoushi.top/gtwuwqyjag.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jianghu66.top/gtuiunkxhj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.0kj1m.cn/gtsosgkukd.html

Ruby: (0...10).step(2).to_a
来源：http://hz.quarkkingdee.top/gtwdsfbtva.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shanyushiyangkeji.top/gtmmzslxxf.html

[B12] 跳出多层循环
来源：http://hz.zycfv.cn/gtqvwdqmbj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gogol.net.cn/gtbmoiuucz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hysaishi.cn/gtgdwqqjhl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.iojbl.cn/gtanpkxswn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.vqdsnc.cn/gtxtjflgqw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnxiangtu.top/gtrbrohgel.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.dashuyun.cn/gtilazqjkr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yuanzhike.top/gtfrwshref.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhongyouzk.top/gtivytohla.html

[B13] 判断是否为数字
来源：http://hz.shzxlz.cn/gtmqlyqvyh.html

Py:   isinstance(x, (int, float))
来源：http://hz.aibaodan.cn/gtsnmatcjo.html

PHP:  is_numeric($x)
来源：http://hz.xziqi.cn/gtcwrqdrgl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinqigufen.top/gtlguaorcd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ywan-chungtsiang.top/gtjkbfopzy.html

Java: x instanceof Number
来源：http://hz.sufxvd.cn/gtzpsxtnvk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinghuilouyu.cn/gtfdcivvcb.html

Ruby: x.is_a?(Numeric)
来源：http://hz.fzhhl.top/gtusokeofm.html

C#:   x is int or double or decimal
来源：http://hz.cdnleiting.top/gtyiazstgo.html

[B14] 判断值是否在集合内
来源：http://hz.gzhubu.top/gtyrxqqibt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhengqikj.top/gtodzhoawy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.haohaochexian.top/gttntltxkp.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ehwqpu.com/gtabtrnyjv.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yanxiufei.cn/gtuviruuck.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.birdmap.top/gtocklhrjp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nanxinkj.top/gthketaicq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.fengsongda.top/gtwvmdxfdr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.smart0.xyz/gtqtrlqkia.html

[B15] 布尔运算与取反
来源：http://hz.dashuyun.cn/gtiukgymwk.html

Py:   a and b or not c
来源：http://hz.smart0.xyz/gtgikvpiqd.html

PHP:  $a && $b || !$c
来源：http://hz.birdmap.top/gtzkjhjzsy.html

JS:   a && b || !c
来源：http://hz.hfpthk.cn/gtvnmqrhwg.html

TS:   a && b || !c
来源：http://hz.shuidangran.top/gtwmdkycxo.html

Java: a && b || !c
来源：http://hz.svipenyu.cn/gtvpfzabve.html

Go:   a && b || !c
来源：http://hz.jinqigfzy.top/gtflkhxmwt.html

Ruby: a && b || !c
来源：http://hz.dashuyun.cn/gtxblfavle.html

C#:   a && b || !c
来源：http://hz.zdqjudy.top/gtmvhumvwg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jinqigufen.top/gtvaethjcn.html

Py:   if not data: return
来源：http://hz.shanyushiyangtech.top/gtxxbtgjqb.html

PHP:  if (!$data) { return; }
来源：http://hz.bjfxy.top/gtlqwltdvm.html

JS:   if (!data) return;
来源：http://hz.c1oappe.top/gtthjprbzp.html

TS:   if (!data) return;
来源：http://hz.yuxming.cn/gthfkovnho.html

Java: if (data == null) return;
来源：http://hz.smart0.xyz/gtgejwdcmt.html

Go:   if data == nil { return }
来源：http://hz.c1oappe.top/gtamuvkdpn.html

Ruby: return if data.nil?
来源：http://hz.andypj.xyz/gtoufareuh.html

C#:   if (data == null) return;
来源：http://hz.hnxiangtu.top/gtcpxdrbed.html

================================================================================
来源：http://hz.fzhhl.top/gtyabhsrbl.html

C. 函数与作用域
来源：http://hz.cheryme.top/gtyisyrrit.html

================================================================================
来源：http://hz.yueranfly.top/gttyfpwydl.html

[C01] 定义函数
来源：http://hz.chenjidiqi.icu/gtgkfkvtem.html

Py:   def add(a, b): return a + b
来源：http://hz.chenlongwang.top/gtkkzorkyu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dianchejie.cn/gticwmvhji.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zycfv.cn/gtcgojxtii.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxuanxn.top/gtghimfmrm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtgotvnojl.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.52xcode.cn/gtrfxbpreo.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zycfv.cn/gtvqczfdfg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtkiluxuqh.html

[C02] 默认参数
来源：http://hz.0kj1m.cn/gtwistomqj.html

Py:   def greet(name="World"): return name
来源：http://hz.316326.xyz/gtqswbwuze.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zycfv.cn/gtoejcsqut.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.0kj1m.cn/gtswrrwnnk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yuxming.cn/gtrcskcegs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xylfe.cn/gtqjoycicd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhaomingkeji.xyz/gtuyrygzhk.html

Ruby: def greet(name = "World") = name
来源：http://hz.jyoumei.cn/gtcdlzxwpy.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zycfv.cn/gtxamodinr.html

[C03] 可变参数
来源：http://hz.ydzc1.top/gthcvotypt.html

Py:   def total(*args): return sum(args)
来源：http://hz.andypj.xyz/gtjebafyfr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ywan-chungtsiang.top/gtedanwzmy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydzc1.top/gtrkjghdvs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daria6918.cn/gtbpinghce.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gotoacloud.top/gtplhqmebi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cucudq.cn/gtvejxxbiw.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.kuanghao11.cn/gtwubuhicd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xingfuxueyuan.xyz/gtjsfazjeo.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yj202588.top/gtukzwpyph.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.316326.xyz/gtmdsaqzdi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhengqikj.top/gtvrzkmdcs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtcfltcoqi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jlsjyb.cn/gtkoxgqiyx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.aibaodan.cn/gtiqomlhit.html

Go:   // 无：用配置结构体参数
来源：http://hz.yongpay.top/gtnzetwyvt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtiqcvxrbh.html

C#:   f(a: 1, b: 2)
来源：http://hz.hysaishi.cn/gtcuaevemv.html

[C05] 返回多个值
来源：http://hz.xingfuxueyuan.xyz/gtdoytwtip.html

Py:   return a, b
来源：http://hz.yvedp.cn/gtypuwvtzf.html

PHP:  return [$a, $b];
来源：http://hz.daria6918.cn/gtfcczauds.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ybcxt.top/gtfzxoghml.html

TS:   return { a, b };
来源：http://hz.meibo888.top/gtvasjfqwq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shanyushiyangkeji.top/gtcgxukfhj.html

Go:   return a, b
来源：http://hz.chenlongwang.top/gtlsxvcbxx.html

Ruby: return a, b
来源：http://hz.chenzaomai.com/gtaeqckjqk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ydjk.org.cn/gtrojxqejs.html

[C06] 匿名函数 / lambda
来源：http://hz.yj202588.top/gtkipyjcsa.html

Py:   square = lambda x: x * x
来源：http://hz.nanxinkj.top/gtclgriise.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ydjk.org.cn/gtbpntwpyx.html

JS:   const square = x => x * x;
来源：http://hz.jqgufenzy.top/gtlpijpodc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.wangshuangyany.cn/gtnazimcwj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.feifeiyinyue.top/gteroutafg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhixingplan.top/gtcbewhzby.html

Ruby: square = ->(x) { x * x }
来源：http://hz.vqdsnc.cn/gtknksnrra.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hywenlv.cn/gtezdcpemr.html

[C07] 把函数作为参数传入
来源：http://hz.hnxiangtu.top/gtliwkkgcf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinghuilouyu.cn/gttdqeiuxn.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.birdmap.top/gtlumkauhb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yuanzhike.top/gtxdekfjni.html

TS:   arr.map(String)
来源：http://hz.havefunace.top/gtazlbplgn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.andypj.xyz/gtedvgdscb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hnxiangtu.top/gttuqzihlj.html

Ruby: arr.map(&:upcase)
来源：http://hz.xinyue.icu/gtakwmmsyn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.wangshuangyany.cn/gtexkzhjzd.html

[C08] 闭包
来源：http://hz.nanxuanxn.top/gtnsyciokq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.guowangkeji.top/gtyoynorbu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zdqjudy.top/gtsgsursro.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gtknyywbot.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cqqwz.cn/gtjzkuliom.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.kuanghao11.cn/gtuwkitjkr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hywenlv.cn/gtxsixsqph.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yuxming.cn/gtlojpjzwp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj20258.top/gtallfhyjq.html

[C09] 递归
来源：http://hz.wangshuangyany.cn/gtksezooqi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hysaishi.cn/gtzxaukuea.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.52xcode.cn/gteswskilv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangkeji.top/gtsdmvyubh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ppjwa.cn/gtpceqnscw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.mhx1999.top/gtivaockso.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.c1oappe.top/gtkwsizmmx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yonumen.top/gtpukpwprt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxinkj.top/gtmoawefbw.html

[C10] 变量作用域
来源：http://hz.hnqzz.top/gtvphnbhdw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shanyushiyangkeji.top/gtblddkfla.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxuanxn.top/gtdapyvixi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yuxming.cn/gtuhxvtupq.html

TS:   同 JS
来源：http://hz.aibaodan.cn/gtwmhpzufz.html

Java: 方法内为块级作用域
来源：http://hz.cheryme.top/gtwqoigdzh.html

Go:   花括号块级作用域
来源：http://hz.dashuyun.cn/gtbsjhgauc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.wangdashe.top/gtzilkkvla.html

C#:   块级作用域
来源：http://hz.birdmap.top/gtwbpbzzyk.html

[C11] 模块导入与导出
来源：http://hz.cheryme.top/gtjwmpsehn.html

Py:   from module import func
来源：http://hz.zdqjudy.top/gtakbasyyi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj20258.top/gtsqrqdawl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.wangshuangyany.cn/gtrzaypagx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.9152youxi.cn/gteexbgeuv.html

Java: import java.util.List;
来源：http://hz.jyoumei.cn/gtlyvkgwok.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.feifeiyinyue.top/gtunovbbuf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.wangdashe.top/gtgeujkrcv.html

C#:   using System.Text;
来源：http://hz.xuanzx.com/gtgdqtwbfl.html

[C12] 立即执行函数 IIFE
来源：http://hz.kuanghao11.cn/gtkdkilssz.html

Py:   (lambda: print("run"))()
来源：http://hz.jinyuanbaomall.cn/gtelwoxvqa.html

PHP:  (function () { echo "run"; })();
来源：http://hz.mhx1999.top/gtlciqehrw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.kuanghao11.cn/gtztnlpggv.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhiwuduotai.top/gtivyhhzcv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nanxinkj.top/gtzndslcdp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.wangdashe.top/gtiuvaxvrs.html

Ruby: -> { puts "run" }.call
来源：http://hz.meibo888.top/gthxkthnbw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.9152youxi.cn/gtbhjdvgmj.html

[C13] 类型声明 / 类型注解
来源：http://hz.ivvv.top/gtblaziizk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yonumen.top/gtxjtdxmrp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtjnhbahnc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.tian-w.cn/gtjxjyqxsd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuetiantiany.cn/gtaogwmcnv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gttssfasyx.html

Go:   func add(a, b int) int
来源：http://hz.gotoacloud.top/gtgssfdqlc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.bjfxy.top/gtfysgzltc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jianghu66.top/gtzrempgks.html

[C14] 泛型函数
来源：http://hz.feifeiyinyue.top/gttyiozlve.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.mhx1999.top/gtdwacbjew.html

PHP:  // 无泛型
来源：http://hz.chenjidiqi.icu/gtijbtlipy.html

JS:   // 无泛型
来源：http://hz.yanxiufei.cn/gtwvzrorfz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sysykeji.top/gtvwqbapun.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.sufxvd.cn/gtuvxlobia.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zdqjudy.top/gtefcalchk.html

Ruby: # 无泛型
来源：http://hz.hywenlv.cn/gtscfjzoca.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xuanzx.com/gtcrbdtusk.html

[C15] 解构 / 展开参数
来源：http://hz.iojbl.cn/gtcjyzfuaq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zycfv.cn/gtilatlxyw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sweek.top/gtariwsuwi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ivvv.top/gtcsstcovu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xingfuxueyuan.xyz/gtjvdufyzl.html

Java: // 无解构
来源：http://hz.zhijiandao.cn/gtacottvtp.html

Go:   // 无解构
来源：http://hz.ydzc1.top/gtulkhvojx.html

Ruby: a, b = pair
来源：http://hz.dashuyun.cn/gtvsmloete.html

C#:   var (a, b) = pair;
来源：http://hz.cqqwz.cn/gthchlaehn.html

[C16] 函数 / 方法重载
来源：http://hz.bjfxy.top/gtyfsgqmvo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yvedp.cn/gtpswzrxke.html

PHP:  // 无重载
来源：http://hz.bjfxy.top/gtemjwiwiv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.feifeiyinyue.top/gtxsbttcrw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yangfankeji.com/gtjdwmsjys.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhiwuduotai.top/gtxylvowjh.html

Go:   // 无重载：用不同函数名
来源：http://hz.guannengcc.top/gtjwgndblw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.smart0.xyz/gthjxqeirt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cqqwz.cn/gtecdauolq.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtvcmsuvql.html

D. 数组 / 列表 / 集合
来源：http://hz.hnxiangtu.top/gtafsikinu.html

================================================================================
来源：http://hz.shzxlz.cn/gtxvtekvsh.html

[D01] 创建数组 / 列表
来源：http://hz.zhongyouzk.top/gtyhcwdutx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sysykeji.top/gtmmdjewbp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ivvv.top/gtnlanjhrz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sysykeji.top/gtuzqabqgw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.chenzaomai.com/gtmkaeoflq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hongshengwenyu.top/gtohacwoym.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.dashuyun.cn/gtsqfnfebc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xziqi.cn/gtosiqjdss.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.bjfxy.top/gttemkkbgp.html

[D02] 追加元素到末尾
来源：http://hz.tian-w.cn/gtnapkkxwv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shanyushiyangtech.top/gtsnyntepx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jlsjyb.cn/gtbzwxvfez.html

JS:   arr.push(4);
来源：http://hz.gzhubu.top/gtlptijwed.html

TS:   arr.push(4);
来源：http://hz.wangdashe.top/gtnucadoqc.html

Java: list.add(4);
来源：http://hz.andypj.xyz/gtelgprbmm.html

Go:   arr = append(arr, 4)
来源：http://hz.zhijiandao.cn/gtwknrznab.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ppjwa.cn/gtgupnuxiy.html

C#:   list.Add(4);
来源：http://hz.hnqzz.top/gtzottdjcs.html

[D03] 在指定位置插入元素
来源：http://hz.nanxuanxn.top/gtxrygmjxb.html

Py:   arr.insert(0, 0)
来源：http://hz.aizwys.cn/gtxsnozyyi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.aibaodan.cn/gtvhzueiwt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinqigufen.top/gtnfxfogvu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shangyingyoupin.top/gtkkciccfr.html

Java: list.add(0, 0);
来源：http://hz.fzhhl.top/gtnhqmwojb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.pycfn.com/gtaiovadfn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ybcxt.top/gtvplaxmvy.html

C#:   list.Insert(0, 0);
来源：http://hz.xylfe.cn/gtxiuxugat.html

[D04] 删除元素
来源：http://hz.ivvv.top/gtymeyvlgi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shzxlz.cn/gtgkivkgdp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.haohaochexian.top/gtgibvvcae.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhongyouzk.top/gtuxpuxosj.html

TS:   arr.splice(0, 1);
来源：http://hz.hfpthk.cn/gtqqasghtk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shanyushiyangkeji.top/gtgavcxevo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hammf.cn/gtdrfksksm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cheryme.top/gtphfjdrub.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnxiangtu.top/gtyaxxbhwh.html

[D05] 访问与修改元素
来源：http://hz.nwbrower.top/gtqtvocfzo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hywenlv.cn/gttfjcklki.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.tanke756.top/gtdwvhrbuu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.redwolf501.top/gtucrlydmy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xinyue.icu/gtaatuxrly.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yongpay.top/gtoqclmgco.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtcgykbrla.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydzc1.top/gtctzygpju.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jqgufenzy.top/gtvaqsjmcc.html

[D06] 数组长度
来源：http://hz.chenzaomai.com/gtcbsorlxr.html

Py:   len(arr)
来源：http://hz.ywan-chungtsiang.top/gtofehusek.html

PHP:  count($arr);
来源：http://hz.svipenyu.cn/gtoeelgjuh.html

JS:   arr.length
来源：http://hz.jinyuanbaomall.cn/gtqhndyxvh.html

TS:   arr.length
来源：http://hz.zhoulong.xyz/gtnpzzjlzj.html

Java: list.size();
来源：http://hz.gaohongyu789.top/gtmstdgqgi.html

Go:   len(arr)
来源：http://hz.jyoumei.cn/gtyfjoclmm.html

Ruby: arr.length; arr.size
来源：http://hz.daxiang520.top/gtdiupckyw.html

C#:   list.Count;
来源：http://hz.jiagoushi.top/gtreruelin.html

[D07] 切片 / 取子数组
来源：http://hz.yuanzhike.top/gtwytczzuf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shanyushiyangkeji.top/gtmzpbarii.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ppjwa.cn/gttbkctlvt.html

JS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gtltqbdwcc.html

TS:   arr.slice(1, 4);
来源：http://hz.c1oappe.top/gtktflckrp.html

Java: list.subList(1, 4);
来源：http://hz.hywenlv.cn/gtfdlrrqkb.html

Go:   arr[1:4]
来源：http://hz.ybcxt.top/gtomzmpcyk.html

Ruby: arr[1, 3]
来源：http://hz.tianlin.xyz/gtuoamapjx.html

C#:   list.GetRange(1, 3);
来源：http://hz.bjfxy.top/gteiqmzxze.html

[D08] 合并两个数组
来源：http://hz.cdnleiting.top/gtvydhysbt.html

Py:   a + b;  a.extend(b)
来源：http://hz.andypj.xyz/gtibafldns.html

PHP:  array_merge($a, $b);
来源：http://hz.hongshengwenyu.top/gtizljyjlg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.andypj.xyz/gtwfhgkzuu.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtjktepetw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenjidiqi.icu/gtokyltcma.html

Go:   append(a, b...)
来源：http://hz.9152youxi.cn/gtytmfumst.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nanxuanxn.top/gtfmtgzqhs.html

C#:   a.Concat(b).ToList()
来源：http://hz.daxiang520.top/gthcbgbyvt.html

[D09] 排序（升序）
来源：http://hz.zhijiandao.cn/gttowzmoxl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jyoumei.cn/gtuxpscffq.html

PHP:  sort($arr);
来源：http://hz.zhoulong.xyz/gtomhuegui.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sysykeji.top/gtyuwtjdut.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenlongwang.top/gtwwcxeizl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cucudq.cn/gtawyaebsh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtsccgaebd.html

Ruby: arr.sort
来源：http://hz.316326.xyz/gtuthxuomv.html

C#:   list.Sort();
来源：http://hz.andypj.xyz/gtvavgzvfr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.9152youxi.cn/gtqbxvhmsy.html


<!-- 参考信息 -->