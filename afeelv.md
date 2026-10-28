代发 wailian999

Py:   if not data: return
来源：http://hz.bjfxy.top/gtrifevpva.html

PHP:  if (!$data) { return; }
来源：http://hz.jianghu66.top/gtkrnavgkf.html

JS:   if (!data) return;
来源：http://hz.aizwys.cn/gtikwxrhei.html

TS:   if (!data) return;
来源：http://hz.jinqigfzy.top/gtwwqllnwd.html

Java: if (data == null) return;
来源：http://hz.ppjwa.cn/gteqneiecw.html

Go:   if data == nil { return }
来源：http://hz.jlsjyb.cn/gtgebqgwmg.html

Ruby: return if data.nil?
来源：http://hz.hnxiangtu.top/gtarsxgcgb.html

C#:   if (data == null) return;
来源：http://hz.hysaishi.cn/gtyuhqmnsk.html

================================================================================
来源：http://hz.aibaodan.cn/gtmqyzwill.html

C. 函数与作用域
来源：http://hz.ywan-chungtsiang.top/gticznryzt.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthwlocqyp.html

[C01] 定义函数
来源：http://hz.mhx1999.top/gtimcqhyez.html

Py:   def add(a, b): return a + b
来源：http://hz.yonumen.top/gtowpmhujl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daria6918.cn/gtxfwydooj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtiseoakuw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydjk.org.cn/gtpwwvoqgl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtzcqgsvwt.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.dianchejie.cn/gtvxqszcgj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sufxvd.cn/gtvdvlwtcg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yongpay.top/gtfnwmbhqa.html

[C02] 默认参数
来源：http://hz.sweek.top/gtvbvmjwhv.html

Py:   def greet(name="World"): return name
来源：http://hz.iojbl.cn/gtuvvigeya.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sysykeji.top/gtznhnpyhc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cqqwz.cn/gtqwdfyrry.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yangfankeji.com/gtgkdvtptp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.gogol.net.cn/gthlasgjne.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.smart0.xyz/gtflgfrcxb.html

Ruby: def greet(name = "World") = name
来源：http://hz.nanxuanxn.top/gtwkxbffby.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hywenlv.cn/gtrwlzanni.html

[C03] 可变参数
来源：http://hz.xinyue.icu/gtxvdkendj.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenjidiqi.icu/gtfajudecs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.bjfxy.top/gtxhqsqgrz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jlsjyb.cn/gtjxrdzkxm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.mhx1999.top/gtfjqcipke.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.316326.xyz/gthkdwtzat.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zdqjudy.top/gtapgcznnv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj20258888.top/gtayghozry.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shanyushiyangkeji.top/gtmbbzgnzi.html

[C04] 命名参数 / 关键字参数
来源：http://hz.svipenyu.cn/gtacipxfao.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenlongwang.top/gtjkuobhjj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.meibo888.top/gtmoukunym.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.aizwys.cn/gtzenqjvzp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenlongwang.top/gtxsvrdnrh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jianghu66.top/gtfzxrrxbm.html

Go:   // 无：用配置结构体参数
来源：http://hz.ivvv.top/gtcrcfmfkm.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tanke756.top/gtuwlevcqk.html

C#:   f(a: 1, b: 2)
来源：http://hz.nanxinkj.top/gtbcobwkwk.html

[C05] 返回多个值
来源：http://hz.cucudq.cn/gtaxtjqpbx.html

Py:   return a, b
来源：http://hz.cqqwz.cn/gtktxvqcwh.html

PHP:  return [$a, $b];
来源：http://hz.nanxuanxn.top/gtuiywwpjd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jinghuilouyu.cn/gtvpgxnfsw.html

TS:   return { a, b };
来源：http://hz.daxiang520.top/gtczdpifjg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hywenlv.cn/gtpurnkiag.html

Go:   return a, b
来源：http://hz.yvedp.cn/gtagglyegn.html

Ruby: return a, b
来源：http://hz.316326.xyz/gtvejinzkk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhaomingkeji.xyz/gtuaxqnhsj.html

[C06] 匿名函数 / lambda
来源：http://hz.chenzaomai.com/gtweoukywp.html

Py:   square = lambda x: x * x
来源：http://hz.vqdsnc.cn/gtxcsjplik.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hfpthk.cn/gtwsfmyqhs.html

JS:   const square = x => x * x;
来源：http://hz.9152youxi.cn/gtyiicjsgc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hnxiangtu.top/gtcbjidpjk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xziqi.cn/gtldgmcpeh.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shuidangran.top/gtfvlgwwym.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ivvv.top/gtrziirruo.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.c1oappe.top/gtxwhtcvdg.html

[C07] 把函数作为参数传入
来源：http://hz.jlsjyb.cn/gtcrwwlfkn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenlongwang.top/gtmrkejkev.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhijiandao.cn/gtwsgduyzs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cdnleiting.top/gtngkhqwyr.html

TS:   arr.map(String)
来源：http://hz.cucudq.cn/gtbqqdnfak.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.meibo888.top/gtaqkpkskx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ivvv.top/gtzhguylkh.html

Ruby: arr.map(&:upcase)
来源：http://hz.sxryk.cn/gtijwsaiei.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sufxvd.cn/gtdzfuhdsi.html

[C08] 闭包
来源：http://hz.jianghu66.top/gtgjbgemyd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.tianlin.xyz/gtukbouyis.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.guannengcc.top/gtbwqomexg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gtmwdkumhv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gttmkzjbub.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hammf.cn/gttfznrxpn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gzhubu.top/gtfktapndy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.guannengcc.top/gtqqoavbta.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj20258.top/gtwysobble.html

[C09] 递归
来源：http://hz.sweek.top/gtcbltdedb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jianghu66.top/gtemwjbylr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhaomingkeji.xyz/gtjhecmzpo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxuanxn.top/gtqxbrsvqa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.52xcode.cn/gtrkczfemo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.fengsongda.top/gtmrrkgrhn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ywan-chungtsiang.top/gtgimisoop.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinyuanbaomall.cn/gthitkwkrc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.havefunace.top/gtxcmgfuuo.html

[C10] 变量作用域
来源：http://hz.zhiwuduotai.top/gtmigoxnff.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ivvv.top/gtckaefktb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinqigufen.top/gtrceewyge.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.0kj1m.cn/gtxxwbcfdo.html

TS:   同 JS
来源：http://hz.zhongyouzk.top/gtgselsgjy.html

Java: 方法内为块级作用域
来源：http://hz.xuanzx.com/gtsusibflz.html

Go:   花括号块级作用域
来源：http://hz.zycfv.cn/gtvvaeyqph.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jyoumei.cn/gtocpolqfo.html

C#:   块级作用域
来源：http://hz.yj20258888.top/gtvjgjhrik.html

[C11] 模块导入与导出
来源：http://hz.0kj1m.cn/gtrtizkwrr.html

Py:   from module import func
来源：http://hz.hnqzz.top/gtdjfkvwmo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.havefunace.top/gtbjzpkryz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yj20258.top/gtavljmzbz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zycfv.cn/gtohpceerz.html

Java: import java.util.List;
来源：http://hz.xingfuxueyuan.xyz/gtfbwegtek.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ivvv.top/gtkibhrfnm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenlongwang.top/gtxslqllxo.html

C#:   using System.Text;
来源：http://hz.yj20258888.top/gtlsuqbboo.html

[C12] 立即执行函数 IIFE
来源：http://hz.tianlin.xyz/gtoflwoucd.html

Py:   (lambda: print("run"))()
来源：http://hz.fengsongda.top/gtdvqfbizg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.c1oappe.top/gtowzhkgic.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xuetiantiany.cn/gtvjcadwqs.html

TS:   (() => { console.log("run"); })();
来源：http://hz.meibo888.top/gtgtonvqxj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.gotoacloud.top/gthgeljmcv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nanxinkj.top/gtavahvbwb.html

Ruby: -> { puts "run" }.call
来源：http://hz.0kj1m.cn/gttoalbala.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hysaishi.cn/gtusgybcdt.html

[C13] 类型声明 / 类型注解
来源：http://hz.chenjidiqi.icu/gtcdwqkdcv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuetiantiany.cn/gtcbpbevry.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dianchejie.cn/gtericbifo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.daria6918.cn/gtooxeafgm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sufxvd.cn/gtkhhazrcg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.0kj1m.cn/gtrlyqdvzm.html

Go:   func add(a, b int) int
来源：http://hz.hysaishi.cn/gtrrwudkhh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jiagoushi.top/gtxusyqxbo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenzaomai.com/gtjekxshdz.html

[C14] 泛型函数
来源：http://hz.andypj.xyz/gtgcdvzkbx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zycfv.cn/gtkadtzfqh.html

PHP:  // 无泛型
来源：http://hz.xuetiantiany.cn/gtwfprhffe.html

JS:   // 无泛型
来源：http://hz.gogol.net.cn/gtpuuvcocb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guannengcc.top/gtggiaqwur.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shangyingyoupin.top/gtpnhxpuyf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hammf.cn/gtmplbfxgr.html

Ruby: # 无泛型
来源：http://hz.dianchejie.cn/gtiktcqvdo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yvedp.cn/gtmfaepiup.html

[C15] 解构 / 展开参数
来源：http://hz.vqdsnc.cn/gtsanrzvqp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.pycfn.com/gtrktdeafe.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cucudq.cn/gtcsaklosc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ydzc1.top/gtebrakcyw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.birdmap.top/gtpvwxkxgs.html

Java: // 无解构
来源：http://hz.xingfuxueyuan.xyz/gtfsljvxbt.html

Go:   // 无解构
来源：http://hz.dashuyun.cn/gtlomwuxia.html

Ruby: a, b = pair
来源：http://hz.daria6918.cn/gtumjmdpia.html

C#:   var (a, b) = pair;
来源：http://hz.zycfv.cn/gtoqxfazwp.html

[C16] 函数 / 方法重载
来源：http://hz.ybcxt.top/gtlcdwvsan.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gzhubu.top/gtuocsrbtq.html

PHP:  // 无重载
来源：http://hz.zhoulong.xyz/gtsfgdttxe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ehwqpu.com/gteljsmmod.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jiagoushi.top/gtnzypwukg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hnxiangtu.top/gteyszpbxc.html

Go:   // 无重载：用不同函数名
来源：http://hz.meibo888.top/gtjjpfgfeo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hfpthk.cn/gtqnarekjv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.iojbl.cn/gtnofzxcwq.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtqmtxxchx.html

D. 数组 / 列表 / 集合
来源：http://hz.gotoacloud.top/gtudjlmncu.html

================================================================================
来源：http://hz.gaohongyu789.top/gtmyaijeov.html

[D01] 创建数组 / 列表
来源：http://hz.guowangkeji.top/gtmislxqwe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tian-w.cn/gteplhlgin.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenzaomai.com/gtkmldnlue.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shanyushiyangtech.top/gtqhqbnonb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hongshengwenyu.top/gtpvcxnvor.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.feifeiyinyue.top/gtvvkudohy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yanxiufei.cn/gtrgjdfovm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ywan-chungtsiang.top/gtyparnsuk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuetiantiany.cn/gtqvolvqxp.html

[D02] 追加元素到末尾
来源：http://hz.cucudq.cn/gtyquwwzcj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ywan-chungtsiang.top/gttzoispuv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhengqikj.top/gtzgcenawt.html

JS:   arr.push(4);
来源：http://hz.nanxuanxn.top/gtgugmrpci.html

TS:   arr.push(4);
来源：http://hz.zhoulong.xyz/gtqpjhbcsv.html

Java: list.add(4);
来源：http://hz.yongpay.top/gtiufixwxs.html

Go:   arr = append(arr, 4)
来源：http://hz.jinghuilouyu.cn/gtstxrokqd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhoulong.xyz/gtsmrumatd.html

C#:   list.Add(4);
来源：http://hz.yonumen.top/gtihwpkuzm.html

[D03] 在指定位置插入元素
来源：http://hz.havefunace.top/gtirjzobgd.html

Py:   arr.insert(0, 0)
来源：http://hz.xingfuxueyuan.xyz/gthkamjyfp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hywenlv.cn/gtylwvcdtb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jianghu66.top/gthhsmgunp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gotoacloud.top/gtrxtrpphh.html

Java: list.add(0, 0);
来源：http://hz.daxiang520.top/gtunokpgyh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jianghu66.top/gtpcmssleo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj202588.top/gtuksrouuj.html

C#:   list.Insert(0, 0);
来源：http://hz.guowangkeji.top/gtdrbowwxd.html

[D04] 删除元素
来源：http://hz.jlsjyb.cn/gtiqrorkfe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.fzhhl.top/gtahpfbbfc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnqzz.top/gtpzngkgpp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yongpay.top/gtvajnnuyu.html

TS:   arr.splice(0, 1);
来源：http://hz.yj202588.top/gtqbukxpyd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xuetiantiany.cn/gtftewysml.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jqgfzy.top/gtgvxczeso.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.wangdashe.top/gtajibmcfv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ybcxt.top/gtkmgstkfi.html

[D05] 访问与修改元素
来源：http://hz.meibo888.top/gtcnecwlpw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ybcxt.top/gttrieiwrv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gteibgaahz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jianghu66.top/gtkgvatfcm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ywan-chungtsiang.top/gtbtlorrmu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sysykeji.top/gtjrredqcv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ivvv.top/gtlgwofynv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ywan-chungtsiang.top/gtnmhqtzha.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shangyingyoupin.top/gtgnovdjqm.html

[D06] 数组长度
来源：http://hz.tanke756.top/gtjynnhxlb.html

Py:   len(arr)
来源：http://hz.hywenlv.cn/gttlzdomur.html

PHP:  count($arr);
来源：http://hz.ehwqpu.com/gtjdbvsmpe.html

JS:   arr.length
来源：http://hz.hnqzz.top/gtutapmsez.html

TS:   arr.length
来源：http://hz.ywan-chungtsiang.top/gtviobdqmz.html

Java: list.size();
来源：http://hz.ybcxt.top/gtzocxztev.html

Go:   len(arr)
来源：http://hz.jinyuanbaomall.cn/gtgayoseqy.html

Ruby: arr.length; arr.size
来源：http://hz.xuanzx.com/gtgvmxqllo.html

C#:   list.Count;
来源：http://hz.nanxuanxn.top/gtjpgszuln.html

[D07] 切片 / 取子数组
来源：http://hz.hfpthk.cn/gtsgbdwdku.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinghuilouyu.cn/gtreduyqpq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.quarkkingdee.top/gtdmngpmab.html

JS:   arr.slice(1, 4);
来源：http://hz.yj202588.top/gtplehhwpz.html

TS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtyyuqsnxn.html

Java: list.subList(1, 4);
来源：http://hz.chenzaomai.com/gtqjgkhbpo.html

Go:   arr[1:4]
来源：http://hz.andypj.xyz/gtaulcwevq.html

Ruby: arr[1, 3]
来源：http://hz.wangshuangyany.cn/gtekmkeuko.html

C#:   list.GetRange(1, 3);
来源：http://hz.hammf.cn/gtzxoobvkl.html

[D08] 合并两个数组
来源：http://hz.redwolf501.top/gtrkkiapnh.html

Py:   a + b;  a.extend(b)
来源：http://hz.wangshuangyany.cn/gtbzeuhllg.html

PHP:  array_merge($a, $b);
来源：http://hz.chenzaomai.com/gtmxvlenme.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yvedp.cn/gtnshamhyy.html

TS:   [...a, ...b];
来源：http://hz.havefunace.top/gtvlfocixp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.pycfn.com/gtozzamgoa.html

Go:   append(a, b...)
来源：http://hz.wangshuangyany.cn/gtbcujrzjj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.bjfxy.top/gtmbqcjilu.html

C#:   a.Concat(b).ToList()
来源：http://hz.zycfv.cn/gtlfkoqrag.html

[D09] 排序（升序）
来源：http://hz.jiagoushi.top/gtvzszaqrj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigufen.top/gtlgxlhbeg.html

PHP:  sort($arr);
来源：http://hz.jianghu66.top/gtlzsshlkm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgfzy.top/gtqekshltd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xziqi.cn/gtoxmzuwnl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shzxlz.cn/gtetohbjpj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj20258.top/gtcxeseuma.html

Ruby: arr.sort
来源：http://hz.yangfankeji.com/gtifqkbywe.html

C#:   list.Sort();
来源：http://hz.yj20258.top/gtfvpftgxp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.fengsongda.top/gteuhnykoh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shangyingyoupin.top/gtvszvbgwy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.vqdsnc.cn/gtqwvaiqqv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tian-w.cn/gtglbxqznn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuetiantiany.cn/gttjdkbagp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ydjk.org.cn/gtfximodzv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.andypj.xyz/gtxbeyndfv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.sysykeji.top/gternfnphg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj202588.top/gtiocwpcgv.html

[D11] 反转数组
来源：http://hz.xuetiantiany.cn/gtkxvstjfa.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ivvv.top/gtraruvqga.html

PHP:  array_reverse($arr);
来源：http://hz.hnxiangtu.top/gtfdkdnlob.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.daxiang520.top/gtaeeuovht.html

TS:   [...arr].reverse();
来源：http://hz.ppjwa.cn/gtjdvkiixl.html

Java: Collections.reverse(list);
来源：http://hz.jinyuanbaomall.cn/gtotoqyrcj.html

Go:   slices.Reverse(arr)
来源：http://hz.zdqjudy.top/gtxredrpyv.html

Ruby: arr.reverse
来源：http://hz.jinqigufen.top/gtvhgrruds.html

C#:   list.Reverse();
来源：http://hz.9152youxi.cn/gtuszmqnhv.html

[D12] 查找元素下标
来源：http://hz.zhaomingkeji.xyz/gtouyyghud.html

Py:   arr.index(x);  x in arr
来源：http://hz.gaohongyu789.top/gtyctexelg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yuanzhike.top/gtwfiiolqt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnxiangtu.top/gtgunuugzy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hammf.cn/gtuyusiyhh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.haohaochexian.top/gtbectiimx.html

Go:   slices.Index(arr, x)
来源：http://hz.yonumen.top/gtjmjkrwph.html

Ruby: arr.index(x)
来源：http://hz.ywan-chungtsiang.top/gtsthzqssr.html

C#:   list.IndexOf(x);
来源：http://hz.zhijiandao.cn/gtdreyxfxm.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yvedp.cn/gtjrcaswyb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ydjk.org.cn/gtmyxjwxfa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinghuilouyu.cn/gtjqgbbhca.html

JS:   arr.filter(x => x > 3)
来源：http://hz.andypj.xyz/gtmmhzxqeo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhongyouzk.top/gtwrjghvqk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sufxvd.cn/gtrxneatex.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.aibaodan.cn/gtltulrvig.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gotoacloud.top/gtyivwcqkd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.daxiang520.top/gttzbyjkqy.html

[D14] 映射转换（每个元素变形）
来源：http://hz.bjfxy.top/gtsptqufcb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.dianchejie.cn/gtytoaadgw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xuanzx.com/gtdwtqhjeg.html

JS:   arr.map(x => x * 2)
来源：http://hz.xziqi.cn/gtuamzgaho.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinyuanbaomall.cn/gtlkubmzfn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.havefunace.top/gtpquejhee.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtuqwjbyjs.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.wangshuangyany.cn/gtpxpppumx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhijiandao.cn/gtiwlpmscc.html

[D15] 去重
来源：http://hz.xingfuxueyuan.xyz/gtcskdridu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jiagoushi.top/gtwwzamrml.html

PHP:  array_unique($arr);
来源：http://hz.jinghuilouyu.cn/gtinbitkqj.html

JS:   [...new Set(arr)]
来源：http://hz.c1oappe.top/gteixoisrm.html

TS:   [...new Set(arr)]
来源：http://hz.aizwys.cn/gtxqkqdiuc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yangfankeji.com/gtemwkbqwb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fzhhl.top/gthqfzsnri.html

Ruby: arr.uniq
来源：http://hz.fzhhl.top/gtqcujkrbl.html

C#:   list.Distinct().ToList()
来源：http://hz.zhongyouzk.top/gtmcraegbw.html

[D16] 求和与平均值
来源：http://hz.kuanghao11.cn/gtkkaqftuo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhijiandao.cn/gtqtdglngr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ywan-chungtsiang.top/gtssjauizs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuanzhike.top/gtszmattwa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fengsongda.top/gtsafgcpur.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sweek.top/gtmkvqazcn.html

Go:   // 手写循环累加
来源：http://hz.sysykeji.top/gtfhorpggb.html


<!-- 参考信息 -->