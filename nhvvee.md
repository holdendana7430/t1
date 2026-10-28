代发 wailian999

Java: if (data == null) return;
来源：http://hz.ppjwa.cn/gtppgelnep.html

Go:   if data == nil { return }
来源：http://hz.kuanghao11.cn/gthxhqsyxu.html

Ruby: return if data.nil?
来源：http://hz.cheryme.top/gtkoricmxn.html

C#:   if (data == null) return;
来源：http://hz.chenzaomai.com/gtaibnrpxm.html

================================================================================
来源：http://hz.sweek.top/gtjaqzwteq.html

C. 函数与作用域
来源：http://hz.kuanghao11.cn/gtqckcsafg.html

================================================================================
来源：http://hz.yj20258888.top/gtlvyvcnup.html

[C01] 定义函数
来源：http://hz.jinqigufen.top/gtzngyqruc.html

Py:   def add(a, b): return a + b
来源：http://hz.hfpthk.cn/gtgegwhttt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.vqdsnc.cn/gtzvxwudcy.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ybcxt.top/gtcllsycoe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daxiang520.top/gtqzfnqxhe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.bjfxy.top/gtpftpppom.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.sufxvd.cn/gtxvsyrcyv.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hnxiangtu.top/gtlnqsbbku.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xylfe.cn/gtzbuiwsqr.html

[C02] 默认参数
来源：http://hz.zhongyouzk.top/gtjojoeqtw.html

Py:   def greet(name="World"): return name
来源：http://hz.dashuyun.cn/gtfsjuflta.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinghuilouyu.cn/gtkggoapvi.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yvedp.cn/gtfrriqemd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.chenzaomai.com/gtlzrfnugw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.kuanghao11.cn/gtwjfvhkur.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.chenzaomai.com/gtiiuaknww.html

Ruby: def greet(name = "World") = name
来源：http://hz.yj20258888.top/gtdttksvoe.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yanxiufei.cn/gtlqdgmjms.html

[C03] 可变参数
来源：http://hz.jiagoushi.top/gtztsbwerb.html

Py:   def total(*args): return sum(args)
来源：http://hz.aizwys.cn/gtcppfkdxg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hnqzz.top/gtxrakekoa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnqzz.top/gtgkdhpzev.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenzaomai.com/gtbbbtlsuw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhaomingkeji.xyz/gthtmnxqcd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yuxming.cn/gtbclvypku.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sysykeji.top/gtyfjhoebb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cucudq.cn/gtbhjytuoc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgfzy.top/gtrutnuzqd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ydjk.org.cn/gtmmnvymry.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yj20258.top/gtowwsbtkj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.chenlongwang.top/gtkirozjsl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cashguo.top/gtxcvgeymf.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hysaishi.cn/gtuqwhetww.html

Go:   // 无：用配置结构体参数
来源：http://hz.nanxuanxn.top/gtyndscinl.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sweek.top/gtqixwtale.html

C#:   f(a: 1, b: 2)
来源：http://hz.nanxuanxn.top/gtozvsjynp.html

[C05] 返回多个值
来源：http://hz.jqgfzy.top/gtsytnwjso.html

Py:   return a, b
来源：http://hz.quarkkingdee.top/gttcbwkmln.html

PHP:  return [$a, $b];
来源：http://hz.kuanghao11.cn/gtqictpgki.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.aizwys.cn/gtwvasxrcw.html

TS:   return { a, b };
来源：http://hz.dashuyun.cn/gttqcouqgr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.guowangkeji.top/gthlpotslo.html

Go:   return a, b
来源：http://hz.haohaochexian.top/gthzedkpix.html

Ruby: return a, b
来源：http://hz.dashuyun.cn/gthtlezqyv.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinghuilouyu.cn/gtshgpkhso.html

[C06] 匿名函数 / lambda
来源：http://hz.zhixingplan.top/gtxawusrpn.html

Py:   square = lambda x: x * x
来源：http://hz.jqgfzy.top/gtsgcpbxum.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yongpay.top/gttpnlefep.html

JS:   const square = x => x * x;
来源：http://hz.svipenyu.cn/gtmdzjjyyi.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yueranfly.top/gtksiemklw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinqigfzy.top/gttlhukrsm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yuanzhike.top/gtsjktrcif.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cdnleiting.top/gtcgjkoosl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinqigfzy.top/gterjfrlue.html

[C07] 把函数作为参数传入
来源：http://hz.9152youxi.cn/gttxcbapio.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhixingplan.top/gtblrzembh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ivvv.top/gtnekdawwy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yangfankeji.com/gtdegacjfr.html

TS:   arr.map(String)
来源：http://hz.jyoumei.cn/gtlftjsvxu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ehwqpu.com/gtnxvuysnl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shuidangran.top/gturtoviqt.html

Ruby: arr.map(&:upcase)
来源：http://hz.zycfv.cn/gtcrnffauf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yangfankeji.com/gttxavqzkd.html

[C08] 闭包
来源：http://hz.ivvv.top/gtlacjytca.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.feifeiyinyue.top/gtqdaqsvpa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jlsjyb.cn/gtvpejkamg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.havefunace.top/gttbqqdhcn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gtjfzvxhab.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.bjfxy.top/gtufzqmwne.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.dianchejie.cn/gtwghdutdz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.9152youxi.cn/gtpforccpy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jianghu66.top/gtawghvfib.html

[C09] 递归
来源：http://hz.jyoumei.cn/gtkmuunwcb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yonumen.top/gtoqyftdjk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ivvv.top/gtoyubkckj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.iojbl.cn/gtsuhdfeiw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pycfn.com/gtekiatkzv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.wangshuangyany.cn/gtfilwtxxk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinqigufen.top/gtnhdumebj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.aibaodan.cn/gtswphkgsr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nwbrower.top/gtyztocpyi.html

[C10] 变量作用域
来源：http://hz.shangyingyoupin.top/gtummsuqwx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.pycfn.com/gtcsgucuax.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yuxming.cn/gtlqbtnysv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xingfuxueyuan.xyz/gtekjmgyqu.html

TS:   同 JS
来源：http://hz.yueranfly.top/gtvlhxdulc.html

Java: 方法内为块级作用域
来源：http://hz.ehwqpu.com/gtzjliukcs.html

Go:   花括号块级作用域
来源：http://hz.zhongyouzk.top/gtoqzzsxmt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.quarkkingdee.top/gtctmcimsg.html

C#:   块级作用域
来源：http://hz.yangfankeji.com/gtiphuagbt.html

[C11] 模块导入与导出
来源：http://hz.chenzaomai.com/gtqptkyvbu.html

Py:   from module import func
来源：http://hz.xylfe.cn/gtylplxhaw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj202588.top/gthkpnweof.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ppjwa.cn/gtaoskfxys.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gogol.net.cn/gtknxnqtau.html

Java: import java.util.List;
来源：http://hz.tanke756.top/gtdkdzvolr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinyuanbaomall.cn/gtmhyqulwz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.haohaochexian.top/gtuoesvmdi.html

C#:   using System.Text;
来源：http://hz.jinqigufen.top/gtklznbetx.html

[C12] 立即执行函数 IIFE
来源：http://hz.kuanghao11.cn/gtvuwfnfgz.html

Py:   (lambda: print("run"))()
来源：http://hz.gaohongyu789.top/gtaoqiavaz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yangfankeji.com/gtumbxrjtu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cucudq.cn/gtwygvvbiq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xuetiantiany.cn/gtuhrdfjwp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.svipenyu.cn/gtkoqwplmw.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gzhubu.top/gtyrorvsfy.html

Ruby: -> { puts "run" }.call
来源：http://hz.cheryme.top/gtdbchfnie.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jiagoushi.top/gtbbelxktb.html

[C13] 类型声明 / 类型注解
来源：http://hz.shangyingyoupin.top/gtqnwqswoh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.0kj1m.cn/gtcfvyieut.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.c1oappe.top/gtivxsuprx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.chenjidiqi.icu/gtecnhlsiv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnqzz.top/gtyrkqlecb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.andypj.xyz/gtjfkydsrg.html

Go:   func add(a, b int) int
来源：http://hz.tianlin.xyz/gtgztcmfqh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.9152youxi.cn/gtrenklizw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shuidangran.top/gtlqrztfqw.html

[C14] 泛型函数
来源：http://hz.zdqjudy.top/gtxkslgrnn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ywan-chungtsiang.top/gtzjyhtano.html

PHP:  // 无泛型
来源：http://hz.hysaishi.cn/gtztnpomeg.html

JS:   // 无泛型
来源：http://hz.zhijiandao.cn/gtqgdozgvp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jiagoushi.top/gtblxgmobt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xziqi.cn/gttdjglqrq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.pengpengdd.cyou/gtdxjgsenn.html

Ruby: # 无泛型
来源：http://hz.yongpay.top/gtgephppub.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.dianchejie.cn/gtxozloksw.html

[C15] 解构 / 展开参数
来源：http://hz.vqdsnc.cn/gtoaagmgsf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ivvv.top/gtuqtefbsq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yvedp.cn/gtonhuxzcq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yangfankeji.com/gtevujlabb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shzxlz.cn/gtertcmagt.html

Java: // 无解构
来源：http://hz.gaohongyu789.top/gtkvqaethk.html

Go:   // 无解构
来源：http://hz.hongshengwenyu.top/gtkegxxvse.html

Ruby: a, b = pair
来源：http://hz.tanke756.top/gtxiozqrma.html

C#:   var (a, b) = pair;
来源：http://hz.shanyushiyangkeji.top/gtsrodyatm.html

[C16] 函数 / 方法重载
来源：http://hz.gzhubu.top/gtlpjpoxmo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shuidangran.top/gtdfcgittc.html

PHP:  // 无重载
来源：http://hz.pengpengdd.cyou/gtwvgkgwuq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxuanxn.top/gtmtpophci.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinyuanbaomall.cn/gtduxdvpbi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hfpthk.cn/gttmjawlpk.html

Go:   // 无重载：用不同函数名
来源：http://hz.redwolf501.top/gtrptwmvvs.html

Ruby: # 无重载：靠动态参数
来源：http://hz.chenlongwang.top/gtkqktuxfs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.feifeiyinyue.top/gttvvydupd.html

================================================================================
来源：http://hz.jqgfzy.top/gtbnmlugbt.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258.top/gtrdxsfwip.html

================================================================================
来源：http://hz.jlsjyb.cn/gtriykpdmv.html

[D01] 创建数组 / 列表
来源：http://hz.shanyushiyangkeji.top/gtepuwmhoz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yonumen.top/gtjppaddxa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.c1oappe.top/gtlbdbktpt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.316326.xyz/gtxmxdywtn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.chenjidiqi.icu/gtjtcggvio.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.quarkkingdee.top/gtebcesqhi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.guannengcc.top/gtidgeukwq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.feifeiyinyue.top/gtloybbisq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenlongwang.top/gtzziacaet.html

[D02] 追加元素到末尾
来源：http://hz.zhaomingkeji.xyz/gtlqslwrdv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jyoumei.cn/gtoyjcjjfv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinyuanbaomall.cn/gtwrupuwvv.html

JS:   arr.push(4);
来源：http://hz.jinqigfzy.top/gtlhfzkdst.html

TS:   arr.push(4);
来源：http://hz.mhx1999.top/gtdouwdvab.html

Java: list.add(4);
来源：http://hz.nanxinkj.top/gtewshlail.html

Go:   arr = append(arr, 4)
来源：http://hz.ybcxt.top/gtbzkgsaza.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.feifeiyinyue.top/gtuvdsoiji.html

C#:   list.Add(4);
来源：http://hz.zycfv.cn/gtxiovudux.html

[D03] 在指定位置插入元素
来源：http://hz.nwbrower.top/gtkmquruud.html

Py:   arr.insert(0, 0)
来源：http://hz.fzhhl.top/gtsxryywbm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cqqwz.cn/gthctpyaxa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ivvv.top/gtmyypdnfz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hongshengwenyu.top/gtlinsdqir.html

Java: list.add(0, 0);
来源：http://hz.yangfankeji.com/gtguenjcre.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.guannengcc.top/gtzktgzrfv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aibaodan.cn/gtutnwarfr.html

C#:   list.Insert(0, 0);
来源：http://hz.feifeiyinyue.top/gtrlfacjij.html

[D04] 删除元素
来源：http://hz.hongshengwenyu.top/gteuzlqorn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ppjwa.cn/gtbpxnvgfc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhongyouzk.top/gtpmoymsvk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.daxiang520.top/gtidstspvf.html

TS:   arr.splice(0, 1);
来源：http://hz.hfpthk.cn/gtvrkneeuf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenzaomai.com/gthntdfkzp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.birdmap.top/gtsbpccnrd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xingfuxueyuan.xyz/gtmsrgdjgr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xziqi.cn/gtifjzjfvf.html

[D05] 访问与修改元素
来源：http://hz.ybcxt.top/gthbqhjswj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.andypj.xyz/gtpwcsypyg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.andypj.xyz/gtetkulnpn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aizwys.cn/gttwmfpcfm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shzxlz.cn/gtbpaaixar.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.0kj1m.cn/gtapawuyas.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yj202588.top/gtprwiumbd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zdqjudy.top/gtsogkqhec.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shangyingyoupin.top/gteyxlmhij.html

[D06] 数组长度
来源：http://hz.zhiwuduotai.top/gtbyorgthr.html

Py:   len(arr)
来源：http://hz.jqgfzy.top/gtedtrfdbt.html

PHP:  count($arr);
来源：http://hz.quarkkingdee.top/gtaoqzeone.html

JS:   arr.length
来源：http://hz.sufxvd.cn/gtbwnnpqru.html

TS:   arr.length
来源：http://hz.52xcode.cn/gtuzpflwvq.html

Java: list.size();
来源：http://hz.shuidangran.top/gtzwyusuix.html

Go:   len(arr)
来源：http://hz.quarkkingdee.top/gtpjieufta.html

Ruby: arr.length; arr.size
来源：http://hz.316326.xyz/gtfjbboarv.html

C#:   list.Count;
来源：http://hz.ywan-chungtsiang.top/gtwjrfrxod.html

[D07] 切片 / 取子数组
来源：http://hz.zhaomingkeji.xyz/gtprkaimti.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.52xcode.cn/gtretkccth.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ivvv.top/gtrjtikljn.html

JS:   arr.slice(1, 4);
来源：http://hz.sysykeji.top/gtovhujjdi.html

TS:   arr.slice(1, 4);
来源：http://hz.hnxiangtu.top/gtlzxqplis.html

Java: list.subList(1, 4);
来源：http://hz.aibaodan.cn/gtfsrasifi.html

Go:   arr[1:4]
来源：http://hz.tianlin.xyz/gtfxrnwqge.html

Ruby: arr[1, 3]
来源：http://hz.jqgufenzy.top/gtibwtamfh.html

C#:   list.GetRange(1, 3);
来源：http://hz.xinyue.icu/gtvqajqpdu.html

[D08] 合并两个数组
来源：http://hz.xziqi.cn/gttexdmclu.html

Py:   a + b;  a.extend(b)
来源：http://hz.316326.xyz/gtbrenwhfd.html

PHP:  array_merge($a, $b);
来源：http://hz.wangshuangyany.cn/gtubamcsjn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sysykeji.top/gtsqttnqyo.html

TS:   [...a, ...b];
来源：http://hz.feifeiyinyue.top/gtdgfzwnom.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hfpthk.cn/gtgnqrfvan.html

Go:   append(a, b...)
来源：http://hz.daxiang520.top/gtelehsfwh.html

Ruby: a + b;  a.concat(b)
来源：http://hz.daria6918.cn/gtdjuhihch.html

C#:   a.Concat(b).ToList()
来源：http://hz.xuetiantiany.cn/gtqrwegsak.html

[D09] 排序（升序）
来源：http://hz.jyoumei.cn/gtjxpbnzbf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gtzfatpvys.html

PHP:  sort($arr);
来源：http://hz.aizwys.cn/gtnkuaneyo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.svipenyu.cn/gtrqfgivwg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.redwolf501.top/gtmsoyxngk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenjidiqi.icu/gthvnayrvg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.wangshuangyany.cn/gtamqgumor.html

Ruby: arr.sort
来源：http://hz.yonumen.top/gtzesgclgo.html

C#:   list.Sort();
来源：http://hz.ivvv.top/gtzgmewojd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jlsjyb.cn/gtvtaxpqsp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yuanzhike.top/gtnhmuaqmu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.wangshuangyany.cn/gteayimtch.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yanxiufei.cn/gtgnqjrbtu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigufen.top/gtyhlrfqhz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hongshengwenyu.top/gtrkllsdxu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.haohaochexian.top/gtgabkzxxr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.c1oappe.top/gtkkjxxttu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nanxuanxn.top/gturqsysgm.html

[D11] 反转数组
来源：http://hz.ehwqpu.com/gtzgtolacp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.haohaochexian.top/gtgxmliexo.html

PHP:  array_reverse($arr);
来源：http://hz.zhengqikj.top/gtkbsxsjct.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.svipenyu.cn/gtwdejbxxm.html

TS:   [...arr].reverse();
来源：http://hz.feifeiyinyue.top/gtesofmhdt.html

Java: Collections.reverse(list);
来源：http://hz.sweek.top/gtgvcengfb.html

Go:   slices.Reverse(arr)
来源：http://hz.redwolf501.top/gtdjfghvdu.html

Ruby: arr.reverse
来源：http://hz.cucudq.cn/gtjzxmtxrx.html

C#:   list.Reverse();
来源：http://hz.zhixingplan.top/gtqljflvud.html

[D12] 查找元素下标
来源：http://hz.yueranfly.top/gtunucioil.html

Py:   arr.index(x);  x in arr
来源：http://hz.ivvv.top/gtlxrahrml.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinghuilouyu.cn/gtorozinls.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cheryme.top/gtsslvxxfc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.iojbl.cn/gtikzjqatt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sxryk.cn/gtmiqhqryn.html

Go:   slices.Index(arr, x)
来源：http://hz.yanxiufei.cn/gtditztihe.html

Ruby: arr.index(x)
来源：http://hz.zhiwuduotai.top/gtljamfxne.html

C#:   list.IndexOf(x);
来源：http://hz.chenzaomai.com/gtxrkgeqeh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhaomingkeji.xyz/gtfrkceqrb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zdqjudy.top/gtironudmh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinqigufen.top/gtlovxllqw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.birdmap.top/gtmewppmhy.html

TS:   arr.filter(x => x > 3)
来源：http://hz.redwolf501.top/gtinxnjvyk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yvedp.cn/gtljwkljvb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258.top/gtzwikkuhg.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shuidangran.top/gtecvgbpub.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cheryme.top/gtdcxarumq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zdqjudy.top/gtgbbxwaqr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gogol.net.cn/gthlhggczw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.mhx1999.top/gtfnqtfapx.html

JS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtdefbfaeh.html

TS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gttxxwafpz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.wangdashe.top/gtddqczrpt.html

Go:   // 手写循环
来源：http://hz.gotoacloud.top/gthkprcngy.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.0kj1m.cn/gtqfbffscd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.andypj.xyz/gtqarzbkvw.html

[D15] 去重
来源：http://hz.feifeiyinyue.top/gtzknwefey.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nanxuanxn.top/gtjfchxnxw.html

PHP:  array_unique($arr);
来源：http://hz.jiagoushi.top/gtkciwufvn.html

JS:   [...new Set(arr)]
来源：http://hz.snrcjt.cn/gtqndzoegg.html

TS:   [...new Set(arr)]
来源：http://hz.gzhubu.top/gtnavniblg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj202588.top/gtzsuntdak.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cdnleiting.top/gtdgugboab.html

Ruby: arr.uniq
来源：http://hz.snrcjt.cn/gtlecvgqsr.html

C#:   list.Distinct().ToList()
来源：http://hz.jinyuanbaomall.cn/gtfmudlcgi.html

[D16] 求和与平均值
来源：http://hz.ydjk.org.cn/gtinhqwvfs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.redwolf501.top/gtctuzbjzb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.mhx1999.top/gthnpoxwhy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fengsongda.top/gtcmvlafvv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yonumen.top/gtrbneeqvx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hfpthk.cn/gteffwzmml.html

Go:   // 手写循环累加
来源：http://hz.andypj.xyz/gtjyqkrklg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.316326.xyz/gtfqyfvlfz.html

C#:   list.Sum();  list.Average()
来源：http://hz.ehwqpu.com/gtvbrelkpg.html

[D17] 最大值与最小值
来源：http://hz.hnxiangtu.top/gttonpqvmg.html

Py:   max(arr);  min(arr)
来源：http://hz.jianghu66.top/gtgxzinvwq.html


<!-- 参考信息 -->