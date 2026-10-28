代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cucudq.cn/gtjsrkzffa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.aizwys.cn/gtalelilma.html

[B15] 布尔运算与取反
来源：http://hz.mhx1999.top/gtxlwrryre.html

Py:   a and b or not c
来源：http://hz.hywenlv.cn/gtjwnduila.html

PHP:  $a && $b || !$c
来源：http://hz.c1oappe.top/gtykrulxub.html

JS:   a && b || !c
来源：http://hz.svipenyu.cn/gtbvkkqjmw.html

TS:   a && b || !c
来源：http://hz.gzhubu.top/gtclsxgnxf.html

Java: a && b || !c
来源：http://hz.nanxinkj.top/gtjedptrfu.html

Go:   a && b || !c
来源：http://hz.nanxinkj.top/gtrjrevofs.html

Ruby: a && b || !c
来源：http://hz.pycfn.com/gtnhjnxtta.html

C#:   a && b || !c
来源：http://hz.ydzc1.top/gtuyujdrdo.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.52xcode.cn/gtjbqvfgio.html

Py:   if not data: return
来源：http://hz.jlsjyb.cn/gtjhsaotfa.html

PHP:  if (!$data) { return; }
来源：http://hz.sxryk.cn/gtfjpokryx.html

JS:   if (!data) return;
来源：http://hz.hnxiangtu.top/gtxuxccyfw.html

TS:   if (!data) return;
来源：http://hz.haohaochexian.top/gtyupczfrw.html

Java: if (data == null) return;
来源：http://hz.wangshuangyany.cn/gtlucsarue.html

Go:   if data == nil { return }
来源：http://hz.ppjwa.cn/gtsbdovwwh.html

Ruby: return if data.nil?
来源：http://hz.yonumen.top/gtsdgdbbdj.html

C#:   if (data == null) return;
来源：http://hz.shanyushiyangtech.top/gtgtondwrb.html

================================================================================
来源：http://hz.jqgufenzy.top/gtjegzktci.html

C. 函数与作用域
来源：http://hz.shangyingyoupin.top/gtdqdfweyg.html

================================================================================
来源：http://hz.ybcxt.top/gtccrzlpsv.html

[C01] 定义函数
来源：http://hz.52xcode.cn/gtgszvvhyx.html

Py:   def add(a, b): return a + b
来源：http://hz.kuanghao11.cn/gtrrkhvnbz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtkfbmbkob.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtubkgkxef.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fengsongda.top/gtzmfjagxx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtqhhtpqcx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.haohaochexian.top/gtduqxbppr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zdqjudy.top/gtonnvppbb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhijiandao.cn/gtqnlgiqna.html

[C02] 默认参数
来源：http://hz.hywenlv.cn/gtthiaihhe.html

Py:   def greet(name="World"): return name
来源：http://hz.yongpay.top/gtagzgnmev.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.feifeiyinyue.top/gtmvbqsejk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shangyingyoupin.top/gtpsrsisdq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xylfe.cn/gtbrgodiec.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ivvv.top/gtspaaeegs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cqqwz.cn/gtbgtoeczg.html

Ruby: def greet(name = "World") = name
来源：http://hz.havefunace.top/gtaxthqytk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xingfuxueyuan.xyz/gtyimwflch.html

[C03] 可变参数
来源：http://hz.birdmap.top/gtwgcwefdt.html

Py:   def total(*args): return sum(args)
来源：http://hz.jyoumei.cn/gtzglcjmma.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.vqdsnc.cn/gtfxjljslm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.havefunace.top/gtfxkytkiw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xinyue.icu/gtuoyptkur.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.tian-w.cn/gticotrats.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ywan-chungtsiang.top/gtceowwrbg.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.mhx1999.top/gtsqefncuz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yj202588.top/gtaccbhdaw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.bjfxy.top/gtxfkgtnpw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shzxlz.cn/gtjbkblmbc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ydjk.org.cn/gtlpysnlpu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ybcxt.top/gtmayowqvx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.pengpengdd.cyou/gtbgdiricd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.bjfxy.top/gtubdarcuk.html

Go:   // 无：用配置结构体参数
来源：http://hz.hammf.cn/gtbjxcwusu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hfpthk.cn/gtbnfquycg.html

C#:   f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtujrafzro.html

[C05] 返回多个值
来源：http://hz.mhx1999.top/gtniddkcdx.html

Py:   return a, b
来源：http://hz.xziqi.cn/gtceietzbn.html

PHP:  return [$a, $b];
来源：http://hz.ehwqpu.com/gtvvkzfcnc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.fzhhl.top/gtndohrjqv.html

TS:   return { a, b };
来源：http://hz.zhongyouzk.top/gtbxaohykp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hywenlv.cn/gtobvvvhlc.html

Go:   return a, b
来源：http://hz.jyoumei.cn/gtuxokokyk.html

Ruby: return a, b
来源：http://hz.andypj.xyz/gtbhhmhlef.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.feifeiyinyue.top/gtlmxuiibv.html

[C06] 匿名函数 / lambda
来源：http://hz.redwolf501.top/gtkwcyjyat.html

Py:   square = lambda x: x * x
来源：http://hz.ivvv.top/gtcipdyxbp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.birdmap.top/gtbxkpisre.html

JS:   const square = x => x * x;
来源：http://hz.yj202588.top/gtslxyrbci.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xylfe.cn/gteaxistzi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zycfv.cn/gtjrlyrgrq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.meibo888.top/gthiwtbwdw.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhixingplan.top/gtgpzworrr.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuetiantiany.cn/gtehwjxlnd.html

[C07] 把函数作为参数传入
来源：http://hz.xinyue.icu/gtzcngrffn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.smart0.xyz/gtrbdhnbyp.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hysaishi.cn/gtlkaftosv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yj20258.top/gtqrlmhdsy.html

TS:   arr.map(String)
来源：http://hz.iojbl.cn/gtvybeedbb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.sysykeji.top/gtieyczkco.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.feifeiyinyue.top/gtkxlcmmuu.html

Ruby: arr.map(&:upcase)
来源：http://hz.nanxuanxn.top/gtwqazdxqz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.bjfxy.top/gtgvoxrcwf.html

[C08] 闭包
来源：http://hz.hammf.cn/gtwsebksly.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hammf.cn/gtwqqrggwu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shzxlz.cn/gtulwonzli.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.bjfxy.top/gtmujvglur.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.316326.xyz/gtrmgglrbx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.c1oappe.top/gtwxginobj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ydzc1.top/gtynpnkqck.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.gotoacloud.top/gthtoftcwt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gtfchiqhtl.html

[C09] 递归
来源：http://hz.yueranfly.top/gtbsnwnubr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj20258888.top/gtgvjcrinu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.316326.xyz/gtxeczrdgy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yvedp.cn/gtxtyhlkvp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aizwys.cn/gtlcisuzdm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.fengsongda.top/gthgszbvfm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.bjfxy.top/gtndehkifg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yueranfly.top/gtjxydvnok.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ywan-chungtsiang.top/gtrbdiaqda.html

[C10] 变量作用域
来源：http://hz.chenlongwang.top/gtbmssxrzm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yuxming.cn/gthxzjittl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shzxlz.cn/gtanvhdwws.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhixingplan.top/gtbyhhycmy.html

TS:   同 JS
来源：http://hz.andypj.xyz/gtmejdvvia.html

Java: 方法内为块级作用域
来源：http://hz.zhengqikj.top/gtnysmxrdt.html

Go:   花括号块级作用域
来源：http://hz.gogol.net.cn/gtzuuebsjo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.meibo888.top/gtujyypqfy.html

C#:   块级作用域
来源：http://hz.xinyue.icu/gtoqdjeonn.html

[C11] 模块导入与导出
来源：http://hz.zhoulong.xyz/gtudszxskt.html

Py:   from module import func
来源：http://hz.ydzc1.top/gtybxmviuw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hysaishi.cn/gtfxnivelu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.havefunace.top/gtikvrdwgj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ydzc1.top/gtkisuzvvf.html

Java: import java.util.List;
来源：http://hz.zdqjudy.top/gtlsztccad.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.fzhhl.top/gtwranmgkt.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cqqwz.cn/gtdsjevdhy.html

C#:   using System.Text;
来源：http://hz.yanxiufei.cn/gtpjrgfisd.html

[C12] 立即执行函数 IIFE
来源：http://hz.jqgfzy.top/gtxvkiunbt.html

Py:   (lambda: print("run"))()
来源：http://hz.zhoulong.xyz/gtymcmwsdg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.svipenyu.cn/gtxskyjwwy.html

JS:   (() => { console.log("run"); })();
来源：http://hz.52xcode.cn/gtzrjrsily.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shuidangran.top/gtadjyqyeo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.gaohongyu789.top/gtcvugonck.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gzhubu.top/gttfhuzszf.html

Ruby: -> { puts "run" }.call
来源：http://hz.0kj1m.cn/gthbqtkfqw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hywenlv.cn/gtqcsyqfzf.html

[C13] 类型声明 / 类型注解
来源：http://hz.ybcxt.top/gtdokpmxnk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.dashuyun.cn/gtcimhrzhn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhaomingkeji.xyz/gthilxwzhj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yj20258.top/gtsoqdzamm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pycfn.com/gthoatoabw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jianghu66.top/gtwefkeorv.html

Go:   func add(a, b int) int
来源：http://hz.jlsjyb.cn/gtncesmikt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.havefunace.top/gtrztzlgga.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.meibo888.top/gtqllpexxu.html

[C14] 泛型函数
来源：http://hz.cucudq.cn/gtcvlydpmj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.chenjidiqi.icu/gtxfpkgkej.html

PHP:  // 无泛型
来源：http://hz.svipenyu.cn/gtkydzcolh.html

JS:   // 无泛型
来源：http://hz.wangshuangyany.cn/gtzffaiyum.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.redwolf501.top/gtsrelolen.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinghuilouyu.cn/gteslyhzpv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jiagoushi.top/gtuzvgdhsd.html

Ruby: # 无泛型
来源：http://hz.shzxlz.cn/gtxocbunhj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jiagoushi.top/gttyuqyenu.html

[C15] 解构 / 展开参数
来源：http://hz.gotoacloud.top/gtmjwzvmkp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nwbrower.top/gtgyaonvrg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shuidangran.top/gthnuibhox.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.wangshuangyany.cn/gtyhjfjugd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yj202588.top/gtrtswfpdz.html

Java: // 无解构
来源：http://hz.shanyushiyangkeji.top/gttyeirpgk.html

Go:   // 无解构
来源：http://hz.gzhubu.top/gtrrrnvhaa.html

Ruby: a, b = pair
来源：http://hz.tanke756.top/gtmywqcyad.html

C#:   var (a, b) = pair;
来源：http://hz.vqdsnc.cn/gtjlktypqm.html

[C16] 函数 / 方法重载
来源：http://hz.shangyingyoupin.top/gtthqzhtmc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shanyushiyangtech.top/gtrmotiyuz.html

PHP:  // 无重载
来源：http://hz.shzxlz.cn/gtkdkyogra.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xingfuxueyuan.xyz/gtljwxbabg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.dianchejie.cn/gtsitmpdhw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shanyushiyangtech.top/gtwszwelgl.html

Go:   // 无重载：用不同函数名
来源：http://hz.dianchejie.cn/gtysskufou.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zycfv.cn/gtapyxwhbo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.daria6918.cn/gtlpuyywzl.html

================================================================================
来源：http://hz.ppjwa.cn/gtbpziewcp.html

D. 数组 / 列表 / 集合
来源：http://hz.yangfankeji.com/gtctmigzzf.html

================================================================================
来源：http://hz.shzxlz.cn/gtlbsofnmy.html

[D01] 创建数组 / 列表
来源：http://hz.aizwys.cn/gttxfjhunc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shanyushiyangkeji.top/gtoinubjtf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sxryk.cn/gtptjjkebb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sweek.top/gtgiqkhjcu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shanyushiyangtech.top/gtbzpadznu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cdnleiting.top/gtjalsodmc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shangyingyoupin.top/gtzrbyzywi.html

Ruby: arr = [1, 2, 3]
来源：http://hz.pengpengdd.cyou/gtfsgpunck.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.fzhhl.top/gtschxslmf.html

[D02] 追加元素到末尾
来源：http://hz.hfpthk.cn/gtyrsqbyny.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.52xcode.cn/gthtroplgl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jiagoushi.top/gtymkvvijc.html

JS:   arr.push(4);
来源：http://hz.quarkkingdee.top/gtajkmjrtc.html

TS:   arr.push(4);
来源：http://hz.aibaodan.cn/gtsvxduzpq.html

Java: list.add(4);
来源：http://hz.hnqzz.top/gtvbwrxchy.html

Go:   arr = append(arr, 4)
来源：http://hz.zhixingplan.top/gtnlfqymaf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gzhubu.top/gtryfcfbzg.html

C#:   list.Add(4);
来源：http://hz.kuanghao11.cn/gtbmhlwdaq.html

[D03] 在指定位置插入元素
来源：http://hz.sxryk.cn/gtftdbfeix.html

Py:   arr.insert(0, 0)
来源：http://hz.snrcjt.cn/gtmmxvqwot.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ehwqpu.com/gtgezghzod.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.0kj1m.cn/gtfrjezxkr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jlsjyb.cn/gtajwranwt.html

Java: list.add(0, 0);
来源：http://hz.tian-w.cn/gtdricdrds.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.tianlin.xyz/gtbjxkjqce.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jianghu66.top/gtzbjglfkq.html

C#:   list.Insert(0, 0);
来源：http://hz.birdmap.top/gtnyvwfhcj.html

[D04] 删除元素
来源：http://hz.mhx1999.top/gtjtqtdcmv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cucudq.cn/gtjhqfwkxb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.meibo888.top/gtwqgiaeil.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sufxvd.cn/gthhnlwqmm.html

TS:   arr.splice(0, 1);
来源：http://hz.jlsjyb.cn/gtsndeblix.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sysykeji.top/gtsoaaslpn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yvedp.cn/gtmjogbaqj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.redwolf501.top/gtidijkzyy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hysaishi.cn/gtobsaccdx.html

[D05] 访问与修改元素
来源：http://hz.ydjk.org.cn/gtsgpdfmxp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtafjpgcfm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zycfv.cn/gtrwtsdeii.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jianghu66.top/gtewwhmreq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhengqikj.top/gtxbbdjlpt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuanzhike.top/gtminkqoqk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yuxming.cn/gtaakppajk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gtsrcqotsx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.vqdsnc.cn/gtqqibgovg.html

[D06] 数组长度
来源：http://hz.cdnleiting.top/gtjbdnqzvd.html

Py:   len(arr)
来源：http://hz.hysaishi.cn/gtdzaqvrvr.html

PHP:  count($arr);
来源：http://hz.daxiang520.top/gtjuplwwgf.html

JS:   arr.length
来源：http://hz.iojbl.cn/gtkiyozxle.html

TS:   arr.length
来源：http://hz.yj20258888.top/gtiarzlqyd.html

Java: list.size();
来源：http://hz.yj202588.top/gtvmttihbw.html

Go:   len(arr)
来源：http://hz.dashuyun.cn/gtnxhcgfzx.html

Ruby: arr.length; arr.size
来源：http://hz.xuetiantiany.cn/gtuybrlnve.html

C#:   list.Count;
来源：http://hz.nwbrower.top/gtfjbujawn.html

[D07] 切片 / 取子数组
来源：http://hz.jlsjyb.cn/gtfgbhxust.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhongyouzk.top/gtyclvskmj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yuxming.cn/gtuwbselyf.html

JS:   arr.slice(1, 4);
来源：http://hz.c1oappe.top/gttzxbynhb.html

TS:   arr.slice(1, 4);
来源：http://hz.xylfe.cn/gtplzrlcte.html

Java: list.subList(1, 4);
来源：http://hz.nanxinkj.top/gthkpbooxa.html

Go:   arr[1:4]
来源：http://hz.9152youxi.cn/gtybdgkfjm.html

Ruby: arr[1, 3]
来源：http://hz.andypj.xyz/gtvewalzkm.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhixingplan.top/gtgxzrmkmc.html

[D08] 合并两个数组
来源：http://hz.dianchejie.cn/gtlrjtmovc.html

Py:   a + b;  a.extend(b)
来源：http://hz.pengpengdd.cyou/gtvhajbnke.html

PHP:  array_merge($a, $b);
来源：http://hz.yj202588.top/gtvsyyjtqw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cucudq.cn/gtfwuqzmpj.html

TS:   [...a, ...b];
来源：http://hz.zhoulong.xyz/gtuzayinhm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenlongwang.top/gtykpipkcq.html

Go:   append(a, b...)
来源：http://hz.0kj1m.cn/gtedplflbm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nanxinkj.top/gtosxybsuk.html

C#:   a.Concat(b).ToList()
来源：http://hz.gogol.net.cn/gtyabmnptl.html

[D09] 排序（升序）
来源：http://hz.zhengqikj.top/gtncvcnwws.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aibaodan.cn/gtkzsbulxz.html

PHP:  sort($arr);
来源：http://hz.sweek.top/gteqrsnwfw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sxryk.cn/gtuptimweb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yj202588.top/gtmwdcexch.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zdqjudy.top/gtdezdixqi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtxamwwyyz.html

Ruby: arr.sort
来源：http://hz.nwbrower.top/gtqbdjejwf.html

C#:   list.Sort();
来源：http://hz.52xcode.cn/gtsqzctrnh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yanxiufei.cn/gtrhgulgij.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.guannengcc.top/gtqvxozifo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.wangdashe.top/gtmfulvwrg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxuanxn.top/gtixwwugdf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.andypj.xyz/gteoeiolbt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.svipenyu.cn/gtesxmghcl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.aizwys.cn/gtseyyizyl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gotoacloud.top/gtxtherssu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.wangdashe.top/gtkcjyltlw.html

[D11] 反转数组
来源：http://hz.zhaomingkeji.xyz/gtoegfmazi.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.aizwys.cn/gtafrvyaqx.html

PHP:  array_reverse($arr);
来源：http://hz.hysaishi.cn/gtpfdfntlo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.0kj1m.cn/gtjipwvwwt.html

TS:   [...arr].reverse();
来源：http://hz.ppjwa.cn/gtwaphtaam.html

Java: Collections.reverse(list);
来源：http://hz.ppjwa.cn/gtqcwmjxml.html

Go:   slices.Reverse(arr)
来源：http://hz.xylfe.cn/gtdeomlhrn.html

Ruby: arr.reverse
来源：http://hz.ppjwa.cn/gtnlejhtuu.html

C#:   list.Reverse();
来源：http://hz.jlsjyb.cn/gtxbommzkl.html

[D12] 查找元素下标
来源：http://hz.dianchejie.cn/gtafioolkk.html

Py:   arr.index(x);  x in arr
来源：http://hz.svipenyu.cn/gtcxbiucke.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sufxvd.cn/gtfozhrqsu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sxryk.cn/gttnxjkboy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shangyingyoupin.top/gtcrfsnluo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tanke756.top/gtnifaddsj.html

Go:   slices.Index(arr, x)
来源：http://hz.yanxiufei.cn/gtsrenfcqa.html

Ruby: arr.index(x)
来源：http://hz.gaohongyu789.top/gtgyxmjwxz.html

C#:   list.IndexOf(x);
来源：http://hz.hnqzz.top/gtqqindxag.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenjidiqi.icu/gtqnuexcrl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.daria6918.cn/gtmfujprfe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.aibaodan.cn/gtppiyixfd.html

JS:   arr.filter(x => x > 3)
来源：http://hz.aizwys.cn/gtnynbwuna.html

TS:   arr.filter(x => x > 3)
来源：http://hz.meibo888.top/gtbupbjmuz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hnqzz.top/gtcfpoadhp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhengqikj.top/gtqiwmayki.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.fzhhl.top/gtydruecmg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinghuilouyu.cn/gtqaujtlrv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yangfankeji.com/gtbprthzgb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cashguo.top/gtelcnxynf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aizwys.cn/gteronccpw.html

JS:   arr.map(x => x * 2)
来源：http://hz.jianghu66.top/gtxizqcrxh.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinqigufen.top/gtnaohhjwv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cheryme.top/gthwtsqyoq.html

Go:   // 手写循环
来源：http://hz.cheryme.top/gtsrajincg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.feifeiyinyue.top/gtfszpokoe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.birdmap.top/gtgxeycotq.html

[D15] 去重
来源：http://hz.ydzc1.top/gtogogafae.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shzxlz.cn/gtchdtzfgu.html

PHP:  array_unique($arr);
来源：http://hz.zhongyouzk.top/gtdkzndwqu.html

JS:   [...new Set(arr)]
来源：http://hz.yj20258888.top/gtbrysmzdj.html


<!-- 参考信息 -->