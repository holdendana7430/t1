代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://hz.mhx1999.top/gtcgnadvcb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zycfv.cn/gtiiwinwln.html

JS:   do { i++; } while (i < 10);
来源：http://hz.shuidangran.top/gtncskswzc.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yangfankeji.com/gtyermcgee.html

Java: do { i++; } while (i < 10);
来源：http://hz.cashguo.top/gtlndbdfia.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hywenlv.cn/gtvivzxqqg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xingfuxueyuan.xyz/gttcohjzjn.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtdfkcuygh.html

[B09] break 与 continue
来源：http://hz.zhiwuduotai.top/gtcixgavuh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zhoulong.xyz/gtgihnosll.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtpewewanl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangdashe.top/gtjeftrhxw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtfskinfmk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenzaomai.com/gteqgostkn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.fengsongda.top/gtjphpotwq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.c1oappe.top/gtvrdzinkp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gtdvkxtupd.html

[B10] 遍历同时拿索引
来源：http://hz.jinghuilouyu.cn/gtvayikpzx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.chenlongwang.top/gtvocoucfy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jiagoushi.top/gtjqijgzqb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.kuanghao11.cn/gtmaklzwgp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jlsjyb.cn/gtmnpfrvzq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.pycfn.com/gtrafwoogp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xziqi.cn/gttoacfbtq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhiwuduotai.top/gtkvpaghwc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yj20258.top/gtsztjdsld.html

[B11] 生成数字序列 / 区间
来源：http://hz.sweek.top/gtdiygbkot.html

Py:   list(range(0, 10, 2))
来源：http://hz.jqgfzy.top/gtymznwuge.html

PHP:  range(0, 10, 2);
来源：http://hz.yanxiufei.cn/gtnyhxdepb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jianghu66.top/gtrlquxbbq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jyoumei.cn/gtdulqfhkv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shzxlz.cn/gtotjopjjj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zycfv.cn/gtpysuvibh.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xylfe.cn/gtqrfuyvsy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.wangshuangyany.cn/gtelukyota.html

[B12] 跳出多层循环
来源：http://hz.hywenlv.cn/gtulmzvjnb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hysaishi.cn/gtewuwfwhj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.dianchejie.cn/gtgbwdbyqx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yongpay.top/gtponauedi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.9152youxi.cn/gtgjlkjbwl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.svipenyu.cn/gttnbccreq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.iojbl.cn/gtmrksvzuq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.mhx1999.top/gtpkcyjrnn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.dianchejie.cn/gtwhoqlsha.html

[B13] 判断是否为数字
来源：http://hz.daria6918.cn/gtlfkghlan.html

Py:   isinstance(x, (int, float))
来源：http://hz.shangyingyoupin.top/gtwsgltfwj.html

PHP:  is_numeric($x)
来源：http://hz.shangyingyoupin.top/gtlozrjwqp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hnqzz.top/gtxfvymdhj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hysaishi.cn/gtpixkfyyr.html

Java: x instanceof Number
来源：http://hz.jlsjyb.cn/gtklmpokyw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jianghu66.top/gtuttklkic.html

Ruby: x.is_a?(Numeric)
来源：http://hz.chenzaomai.com/gtpctsheqa.html

C#:   x is int or double or decimal
来源：http://hz.yanxiufei.cn/gtlqoungoi.html

[B14] 判断值是否在集合内
来源：http://hz.dashuyun.cn/gtyqijufrf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jinghuilouyu.cn/gtgypsmjux.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jiagoushi.top/gtucedkhoc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinyuanbaomall.cn/gtgnvtyrjq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangkeji.top/gtohxjisdb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.gzhubu.top/gtymitubbg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cashguo.top/gtqntpyedi.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shuidangran.top/gtsjswaugy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yvedp.cn/gtpbexnwov.html

[B15] 布尔运算与取反
来源：http://hz.jinyuanbaomall.cn/gtnotwvpil.html

Py:   a and b or not c
来源：http://hz.smart0.xyz/gthhvtlluj.html

PHP:  $a && $b || !$c
来源：http://hz.jianghu66.top/gtgepswoci.html

JS:   a && b || !c
来源：http://hz.hammf.cn/gtjvwmebfx.html

TS:   a && b || !c
来源：http://hz.vqdsnc.cn/gtaictqedr.html

Java: a && b || !c
来源：http://hz.52xcode.cn/gtkfftmesp.html

Go:   a && b || !c
来源：http://hz.yonumen.top/gtefasyajq.html

Ruby: a && b || !c
来源：http://hz.yj20258.top/gtcklovpce.html

C#:   a && b || !c
来源：http://hz.smart0.xyz/gtfblmqepe.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.fzhhl.top/gtfwzlswzf.html

Py:   if not data: return
来源：http://hz.jianghu66.top/gtjcobkrgi.html

PHP:  if (!$data) { return; }
来源：http://hz.yongpay.top/gtalqqbmab.html

JS:   if (!data) return;
来源：http://hz.ydzc1.top/gtfyjqmehq.html

TS:   if (!data) return;
来源：http://hz.0kj1m.cn/gtgmbkuode.html

Java: if (data == null) return;
来源：http://hz.xuanzx.com/gtjdmsdjvx.html

Go:   if data == nil { return }
来源：http://hz.jqgufenzy.top/gtytzvfygc.html

Ruby: return if data.nil?
来源：http://hz.jiagoushi.top/gtzcnogfod.html

C#:   if (data == null) return;
来源：http://hz.9152youxi.cn/gtgdlcznzg.html

================================================================================
来源：http://hz.9152youxi.cn/gtssqajivw.html

C. 函数与作用域
来源：http://hz.zdqjudy.top/gtcpyirlwl.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgaqdwfpd.html

[C01] 定义函数
来源：http://hz.cheryme.top/gtlfycineg.html

Py:   def add(a, b): return a + b
来源：http://hz.ehwqpu.com/gtjsctohjh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtbekftgbj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xziqi.cn/gteukkcctq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gtkgwifesw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtucpfvwwx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jlsjyb.cn/gtirrihvjs.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ydzc1.top/gtxfbmgcfs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.smart0.xyz/gtplnrkgke.html

[C02] 默认参数
来源：http://hz.zhoulong.xyz/gtkacmnynv.html

Py:   def greet(name="World"): return name
来源：http://hz.nanxuanxn.top/gtcbuqjxsh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.fzhhl.top/gtayqoagxl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jqgufenzy.top/gttovvtoli.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinqigufen.top/gtlzyjwkqy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yvedp.cn/gtxtmdgtuh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jinqigfzy.top/gterqjasel.html

Ruby: def greet(name = "World") = name
来源：http://hz.zycfv.cn/gtbbllrpmq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jqgfzy.top/gtcgnlbvvk.html

[C03] 可变参数
来源：http://hz.yvedp.cn/gtmpjiizmz.html

Py:   def total(*args): return sum(args)
来源：http://hz.xuetiantiany.cn/gtolflkeal.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yj202588.top/gtzkpsauwb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zycfv.cn/gtvydzmrdj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jlsjyb.cn/gtfcbagfgd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.havefunace.top/gtobuhtrms.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.dashuyun.cn/gtwtgghocr.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.andypj.xyz/gtetcjkxzp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenlongwang.top/gtjpmyvffw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.kuanghao11.cn/gtmjrzhlbd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.gogol.net.cn/gtshrpkklt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.snrcjt.cn/gtgairusdu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.chenlongwang.top/gtkgonmtfx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhixingplan.top/gtdmnbidpe.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.tian-w.cn/gtgphbxrhq.html

Go:   // 无：用配置结构体参数
来源：http://hz.fengsongda.top/gtpabxqcfd.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhoulong.xyz/gtjmzdwlcf.html

C#:   f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtkebdzhps.html

[C05] 返回多个值
来源：http://hz.zdqjudy.top/gtrbzotuem.html

Py:   return a, b
来源：http://hz.sxryk.cn/gtlxmqcujr.html

PHP:  return [$a, $b];
来源：http://hz.aizwys.cn/gtazegljoe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhaomingkeji.xyz/gtdzdogolf.html

TS:   return { a, b };
来源：http://hz.wangshuangyany.cn/gteywpwscd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yvedp.cn/gtxnbohxzm.html

Go:   return a, b
来源：http://hz.feifeiyinyue.top/gtlcxjwqij.html

Ruby: return a, b
来源：http://hz.ehwqpu.com/gttbzvsutd.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.daxiang520.top/gtimiciyll.html

[C06] 匿名函数 / lambda
来源：http://hz.quarkkingdee.top/gturcjrviu.html

Py:   square = lambda x: x * x
来源：http://hz.ivvv.top/gtelvkdamh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gzhubu.top/gtbgqeshgy.html

JS:   const square = x => x * x;
来源：http://hz.daria6918.cn/gtpchdhjpq.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.nanxuanxn.top/gtleawrptw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.kuanghao11.cn/gtefgvsrfv.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tanke756.top/gtiexilgno.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhoulong.xyz/gtqcnngakr.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.nanxuanxn.top/gttpxhwxmc.html

[C07] 把函数作为参数传入
来源：http://hz.pycfn.com/gtwrcudubo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hfpthk.cn/gttecltxju.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenjidiqi.icu/gtckdvmbpm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ppjwa.cn/gticxexill.html

TS:   arr.map(String)
来源：http://hz.mhx1999.top/gtlcgmkqkm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nwbrower.top/gtzzkpepnm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.redwolf501.top/gtpstgbvur.html

Ruby: arr.map(&:upcase)
来源：http://hz.pengpengdd.cyou/gtamwijsnr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yuxming.cn/gtoorekyxz.html

[C08] 闭包
来源：http://hz.ivvv.top/gtspfhcupo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gaohongyu789.top/gtfbjhwkpn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yuxming.cn/gtppjxolhf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jqgufenzy.top/gtnnnmrcle.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.shanyushiyangtech.top/gtiazrccrg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.0kj1m.cn/gtbjvonfsv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sxryk.cn/gtnaopreyt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.0kj1m.cn/gtybznibjs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zycfv.cn/gtjudrddia.html

[C09] 递归
来源：http://hz.tianlin.xyz/gtufvurcfa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenlongwang.top/gtkuujaizc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yonumen.top/gtnlqqmuup.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxuanxn.top/gtkyoasgfc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pycfn.com/gtgoisfrjj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hnqzz.top/gtgowfyrtu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.bjfxy.top/gtvnachulv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hnqzz.top/gtzudzjuuy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gzhubu.top/gtjyxqgmca.html

[C10] 变量作用域
来源：http://hz.jinqigufen.top/gtfbloiadt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ydjk.org.cn/gtlpyzllut.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xingfuxueyuan.xyz/gtncstvxjt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenjidiqi.icu/gtbtxcgwki.html

TS:   同 JS
来源：http://hz.yuanzhike.top/gtbgtstzun.html

Java: 方法内为块级作用域
来源：http://hz.zhiwuduotai.top/gtvattmcqm.html

Go:   花括号块级作用域
来源：http://hz.wangshuangyany.cn/gtnhbxsncg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.shzxlz.cn/gtsevjqcun.html

C#:   块级作用域
来源：http://hz.meibo888.top/gtxmunqvee.html

[C11] 模块导入与导出
来源：http://hz.dianchejie.cn/gtgyeqzene.html

Py:   from module import func
来源：http://hz.pengpengdd.cyou/gtujneyawj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xuanzx.com/gtoqurbthl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.dianchejie.cn/gtijzhfkji.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.dashuyun.cn/gtjilihezi.html

Java: import java.util.List;
来源：http://hz.jlsjyb.cn/gtmbnbhydz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jqgufenzy.top/gtuolnhebu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenjidiqi.icu/gtywxucpxr.html

C#:   using System.Text;
来源：http://hz.sweek.top/gtzkldrbkz.html

[C12] 立即执行函数 IIFE
来源：http://hz.shangyingyoupin.top/gtkgbtedud.html

Py:   (lambda: print("run"))()
来源：http://hz.shanyushiyangkeji.top/gtkfphulph.html

PHP:  (function () { echo "run"; })();
来源：http://hz.haohaochexian.top/gtafctgleu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhijiandao.cn/gtzeswzgnk.html

TS:   (() => { console.log("run"); })();
来源：http://hz.mhx1999.top/gtphdquczt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.c1oappe.top/gtgpvdmhur.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sxryk.cn/gtajilipsu.html

Ruby: -> { puts "run" }.call
来源：http://hz.gotoacloud.top/gtkmfvbtyy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.bjfxy.top/gtolxhmoyr.html

[C13] 类型声明 / 类型注解
来源：http://hz.yangfankeji.com/gtfhpahtlx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guowangkeji.top/gtegcnxjle.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtzrzgvuzi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jianghu66.top/gtpmiodspt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj202588.top/gttfahpexi.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtyjnerwpu.html

Go:   func add(a, b int) int
来源：http://hz.sweek.top/gtzoihpqaq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.fzhhl.top/gtdajregkb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.daria6918.cn/gtmwiiveoc.html

[C14] 泛型函数
来源：http://hz.sysykeji.top/gtfmkeapys.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cucudq.cn/gthmxjytru.html

PHP:  // 无泛型
来源：http://hz.jinghuilouyu.cn/gtgdkyhyzs.html

JS:   // 无泛型
来源：http://hz.bjfxy.top/gtzbeppcdd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhaomingkeji.xyz/gtlwrdehci.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ywan-chungtsiang.top/gtszoyshmc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ydzc1.top/gteinlamcx.html

Ruby: # 无泛型
来源：http://hz.jianghu66.top/gtofjemjvq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.fzhhl.top/gtlouygssb.html

[C15] 解构 / 展开参数
来源：http://hz.iojbl.cn/gtuqnkqgpr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hammf.cn/gtokdkgckd.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gogol.net.cn/gtgfjljvui.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hysaishi.cn/gtfkoehpsx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.aizwys.cn/gtigwqxfnt.html

Java: // 无解构
来源：http://hz.hfpthk.cn/gtbpdgnauh.html

Go:   // 无解构
来源：http://hz.aibaodan.cn/gtnezmkjyb.html

Ruby: a, b = pair
来源：http://hz.xuanzx.com/gtbxeyuvta.html

C#:   var (a, b) = pair;
来源：http://hz.jqgufenzy.top/gtekzoyqvp.html

[C16] 函数 / 方法重载
来源：http://hz.chenlongwang.top/gtmxbzbxsf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tianlin.xyz/gtlzvmpmjj.html

PHP:  // 无重载
来源：http://hz.xinyue.icu/gtryrbligd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jiagoushi.top/gttapphamb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.kuanghao11.cn/gtmwzpdbdx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tian-w.cn/gtkslwkjrd.html

Go:   // 无重载：用不同函数名
来源：http://hz.hammf.cn/gtoshizjlu.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinyuanbaomall.cn/gtrwnpzpev.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xingfuxueyuan.xyz/gtlwpdgnkv.html

================================================================================
来源：http://hz.shuidangran.top/gtzplszhel.html

D. 数组 / 列表 / 集合
来源：http://hz.cashguo.top/gtmsttjgna.html

================================================================================
来源：http://hz.guowangkeji.top/gtdknqphoc.html

[D01] 创建数组 / 列表
来源：http://hz.shanyushiyangkeji.top/gteyuwgbjx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gogol.net.cn/gtaaiielwk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guannengcc.top/gtipdftddh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shzxlz.cn/gtskjavcww.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shuidangran.top/gtewmqduvq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.meibo888.top/gtxnjbktdu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.pycfn.com/gtjdpezzar.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj202588.top/gtvseqwvrd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aibaodan.cn/gtqpjtcjda.html

[D02] 追加元素到末尾
来源：http://hz.yuxming.cn/gtjhrkuswr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenjidiqi.icu/gtxmmqugao.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.dianchejie.cn/gtxboqdejz.html

JS:   arr.push(4);
来源：http://hz.bjfxy.top/gtvuuyyhso.html

TS:   arr.push(4);
来源：http://hz.jianghu66.top/gtzppszsjw.html

Java: list.add(4);
来源：http://hz.c1oappe.top/gtmrpqrnpu.html

Go:   arr = append(arr, 4)
来源：http://hz.gzhubu.top/gtdpgmzkar.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuanzx.com/gtadzvikae.html

C#:   list.Add(4);
来源：http://hz.iojbl.cn/gtqbxgqkjr.html

[D03] 在指定位置插入元素
来源：http://hz.aibaodan.cn/gtyyqjvbyx.html

Py:   arr.insert(0, 0)
来源：http://hz.daria6918.cn/gtuejdylbm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.pengpengdd.cyou/gtvrjlfcgr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shanyushiyangkeji.top/gtqewiljpm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yuxming.cn/gtsrpujlid.html

Java: list.add(0, 0);
来源：http://hz.yuanzhike.top/gttbaevzzk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhoulong.xyz/gtiywxdtvn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydjk.org.cn/gtlnetrjho.html

C#:   list.Insert(0, 0);
来源：http://hz.guowangkeji.top/gtezaozjtc.html

[D04] 删除元素
来源：http://hz.fengsongda.top/gtrvmgxktt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cdnleiting.top/gtedlcehgp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jqgufenzy.top/gtlguqsafm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hnqzz.top/gtmguuwluk.html

TS:   arr.splice(0, 1);
来源：http://hz.gogol.net.cn/gtacwaxlht.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jyoumei.cn/gtatvkkwku.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.iojbl.cn/gtostyuytl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ppjwa.cn/gthbegqjgz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.dashuyun.cn/gtbctqmwva.html

[D05] 访问与修改元素
来源：http://hz.havefunace.top/gtulytzxgh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guannengcc.top/gtyefitrft.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ivvv.top/gtwxvlpwxb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cashguo.top/gtxcvfehad.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.svipenyu.cn/gtuahevgef.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cqqwz.cn/gtwjspyrll.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.aizwys.cn/gtpjhbwxyv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cheryme.top/gtrlrxccgj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yonumen.top/gtzlyrymzw.html

[D06] 数组长度
来源：http://hz.jinyuanbaomall.cn/gttzmbwbhu.html

Py:   len(arr)
来源：http://hz.xuanzx.com/gtbxwxblgx.html

PHP:  count($arr);
来源：http://hz.xinyue.icu/gtnwewiece.html

JS:   arr.length
来源：http://hz.birdmap.top/gtpulespqy.html

TS:   arr.length
来源：http://hz.ydzc1.top/gtnlezpqwp.html

Java: list.size();
来源：http://hz.ydjk.org.cn/gtoubhqfkd.html

Go:   len(arr)
来源：http://hz.nwbrower.top/gtrannjeik.html

Ruby: arr.length; arr.size
来源：http://hz.jinqigfzy.top/gtlbwidnbf.html

C#:   list.Count;
来源：http://hz.nanxuanxn.top/gtmlwjtzyc.html

[D07] 切片 / 取子数组
来源：http://hz.guowangkeji.top/gtynknmoyi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nanxinkj.top/gtqrwrfjhp.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shuidangran.top/gtzcaxjqzu.html

JS:   arr.slice(1, 4);
来源：http://hz.daria6918.cn/gtxzsodiih.html

TS:   arr.slice(1, 4);
来源：http://hz.yj20258.top/gtwvqmymqd.html

Java: list.subList(1, 4);
来源：http://hz.zhongyouzk.top/gtnocyiace.html

Go:   arr[1:4]
来源：http://hz.jinghuilouyu.cn/gtegopsfuo.html

Ruby: arr[1, 3]
来源：http://hz.xylfe.cn/gtwqtbkgcg.html

C#:   list.GetRange(1, 3);
来源：http://hz.c1oappe.top/gtbfxehflr.html

[D08] 合并两个数组
来源：http://hz.xuanzx.com/gtsiqykwni.html

Py:   a + b;  a.extend(b)
来源：http://hz.meibo888.top/gtoifodzgu.html

PHP:  array_merge($a, $b);
来源：http://hz.jinyuanbaomall.cn/gtkaqunait.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.fzhhl.top/gthakulbmz.html

TS:   [...a, ...b];
来源：http://hz.haohaochexian.top/gthgaefgbb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hywenlv.cn/gtuhnflrsv.html

Go:   append(a, b...)
来源：http://hz.zdqjudy.top/gtoblxlhxy.html


<!-- 参考信息 -->