代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://hz.chenjidiqi.icu/gtbgieworv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jqgfzy.top/gtwjhujogq.html

[B15] 布尔运算与取反
来源：http://hz.guannengcc.top/gtjcmaohen.html

Py:   a and b or not c
来源：http://hz.yj202588.top/gtvdvukofa.html

PHP:  $a && $b || !$c
来源：http://hz.xuetiantiany.cn/gtqvblvrif.html

JS:   a && b || !c
来源：http://hz.fzhhl.top/gthjpeoybk.html

TS:   a && b || !c
来源：http://hz.yangfankeji.com/gtvelfsiew.html

Java: a && b || !c
来源：http://hz.cqqwz.cn/gtuwuqchgs.html

Go:   a && b || !c
来源：http://hz.xinyue.icu/gtuzkfqyvk.html

Ruby: a && b || !c
来源：http://hz.gaohongyu789.top/gtmkqkalqj.html

C#:   a && b || !c
来源：http://hz.yj20258.top/gtrimwhncx.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ivvv.top/gtggsbsiyb.html

Py:   if not data: return
来源：http://hz.c1oappe.top/gtwdosalwg.html

PHP:  if (!$data) { return; }
来源：http://hz.jinqigufen.top/gtjamkrzpr.html

JS:   if (!data) return;
来源：http://hz.gzhubu.top/gtndgnuowi.html

TS:   if (!data) return;
来源：http://hz.0kj1m.cn/gtuazsozgc.html

Java: if (data == null) return;
来源：http://hz.bjfxy.top/gtydffancd.html

Go:   if data == nil { return }
来源：http://hz.xuanzx.com/gtqboyywqj.html

Ruby: return if data.nil?
来源：http://hz.chenjidiqi.icu/gtmiznbcqa.html

C#:   if (data == null) return;
来源：http://hz.yvedp.cn/gtqphbkxgg.html

================================================================================
来源：http://hz.316326.xyz/gtkfxwuiog.html

C. 函数与作用域
来源：http://hz.ivvv.top/gtlrtafuhq.html

================================================================================
来源：http://hz.hnxiangtu.top/gttgwbmobe.html

[C01] 定义函数
来源：http://hz.jiagoushi.top/gtjvslcacd.html

Py:   def add(a, b): return a + b
来源：http://hz.bjfxy.top/gtpiswendm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tanke756.top/gtrbtshgav.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xziqi.cn/gtcptkzuji.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.vqdsnc.cn/gtwqoveebc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtuyrasmnp.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhixingplan.top/gtaolnnsdz.html

Ruby: def add(a, b); a + b; end
来源：http://hz.dianchejie.cn/gtivwjaxwm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yanxiufei.cn/gtlvnpyrnf.html

[C02] 默认参数
来源：http://hz.kuanghao11.cn/gtqcejuxaf.html

Py:   def greet(name="World"): return name
来源：http://hz.shanyushiyangtech.top/gtbkdihufm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hywenlv.cn/gtcyqywpio.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhaomingkeji.xyz/gtpijswtms.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ppjwa.cn/gtzdkcbkqs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinqigufen.top/gtquicngol.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xuanzx.com/gtcmbhhazs.html

Ruby: def greet(name = "World") = name
来源：http://hz.yvedp.cn/gtwpxbgjtf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gzhubu.top/gtxgdkrsih.html

[C03] 可变参数
来源：http://hz.xziqi.cn/gtsithtxoy.html

Py:   def total(*args): return sum(args)
来源：http://hz.havefunace.top/gtyjiojqnt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.feifeiyinyue.top/gtqqxwvovt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jianghu66.top/gtdmazotlr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenlongwang.top/gtlqdajswu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.aizwys.cn/gtkapdtyzc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hysaishi.cn/gtgetruqwm.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yuanzhike.top/gtpatpddlq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhoulong.xyz/gthhnucjho.html

[C04] 命名参数 / 关键字参数
来源：http://hz.guowangkeji.top/gtarxefbmb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shanyushiyangtech.top/gttmknxenh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.fzhhl.top/gtvgsemuqm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jqgfzy.top/gthojbiewr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ybcxt.top/gteahodhzs.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hywenlv.cn/gtqllksvar.html

Go:   // 无：用配置结构体参数
来源：http://hz.yj20258.top/gtkblbvrpz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tanke756.top/gtxjblgswe.html

C#:   f(a: 1, b: 2)
来源：http://hz.yonumen.top/gtzkejjvmj.html

[C05] 返回多个值
来源：http://hz.shanyushiyangkeji.top/gtnvhcowna.html

Py:   return a, b
来源：http://hz.sweek.top/gtoqvevwqh.html

PHP:  return [$a, $b];
来源：http://hz.0kj1m.cn/gtpmufgofe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhongyouzk.top/gtatlvqelk.html

TS:   return { a, b };
来源：http://hz.guannengcc.top/gtjiekikqf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.aibaodan.cn/gtebqwcfoh.html

Go:   return a, b
来源：http://hz.mhx1999.top/gtdyfmjudm.html

Ruby: return a, b
来源：http://hz.xziqi.cn/gtlbwauzhb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sysykeji.top/gtokcojvjg.html

[C06] 匿名函数 / lambda
来源：http://hz.ehwqpu.com/gtjhwrmwub.html

Py:   square = lambda x: x * x
来源：http://hz.ybcxt.top/gtxvdqxtps.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.kuanghao11.cn/gtlinmlhgt.html

JS:   const square = x => x * x;
来源：http://hz.dashuyun.cn/gtbjpjkrbs.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jianghu66.top/gtgqcgnyct.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhixingplan.top/gtvospsors.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ehwqpu.com/gtrlsybkck.html

Ruby: square = ->(x) { x * x }
来源：http://hz.gzhubu.top/gtbbcutdrs.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj202588.top/gtpwtzutxh.html

[C07] 把函数作为参数传入
来源：http://hz.ywan-chungtsiang.top/gtqzewlmrf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shangyingyoupin.top/gtqkurstyt.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hongshengwenyu.top/gtnwltyyns.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shuidangran.top/gtlqvyjxls.html

TS:   arr.map(String)
来源：http://hz.jiagoushi.top/gtqzqgqrzt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhiwuduotai.top/gtvsgjafad.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.dashuyun.cn/gtnlkqffkj.html

Ruby: arr.map(&:upcase)
来源：http://hz.shuidangran.top/gtbwdecxlg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.316326.xyz/gtygvxcgew.html

[C08] 闭包
来源：http://hz.yuxming.cn/gtkmnyznmf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gogol.net.cn/gtcscollli.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gogol.net.cn/gtepispfxl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jqgfzy.top/gtjoplpqcz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jiagoushi.top/gtxzfvbnuw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.smart0.xyz/gthwomvapi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ivvv.top/gttzjnuety.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xingfuxueyuan.xyz/gtbcluihld.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gtjjienndu.html

[C09] 递归
来源：http://hz.jinyuanbaomall.cn/gteotytjvr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xuetiantiany.cn/gtrzubftge.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.meibo888.top/gtzsucvane.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenzaomai.com/gthnltwfqo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.andypj.xyz/gtoaeaiims.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.aizwys.cn/gtqelahpou.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zdqjudy.top/gtosqyiyuj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.guowangkeji.top/gtyksoallr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xingfuxueyuan.xyz/gtoksrweny.html

[C10] 变量作用域
来源：http://hz.hongshengwenyu.top/gtlmoejlsk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yj20258.top/gtnuvhulns.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hammf.cn/gtnrbwbfso.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ydjk.org.cn/gtjbhxocls.html

TS:   同 JS
来源：http://hz.gotoacloud.top/gtpuumyztx.html

Java: 方法内为块级作用域
来源：http://hz.pycfn.com/gtwvccagns.html

Go:   花括号块级作用域
来源：http://hz.ivvv.top/gtpjhsctpg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.pycfn.com/gtbqzsjylg.html

C#:   块级作用域
来源：http://hz.tianlin.xyz/gtwjobrbmn.html

[C11] 模块导入与导出
来源：http://hz.jinqigfzy.top/gtbeeogfhr.html

Py:   from module import func
来源：http://hz.pycfn.com/gtxxzcride.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hywenlv.cn/gtixfqenum.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cheryme.top/gtgteztnpz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.iojbl.cn/gtssihsreu.html

Java: import java.util.List;
来源：http://hz.yanxiufei.cn/gtslzaafnz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.chenzaomai.com/gttocuezxe.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sufxvd.cn/gtuzcplcxl.html

C#:   using System.Text;
来源：http://hz.sweek.top/gtdnceeond.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj202588.top/gtjcmfwxed.html

Py:   (lambda: print("run"))()
来源：http://hz.kuanghao11.cn/gthyilumce.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sufxvd.cn/gtjzirbkld.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ivvv.top/gtllahxkuu.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj20258888.top/gtjsmtxhkz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nanxinkj.top/gthejspxyw.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cheryme.top/gtebtlqbfr.html

Ruby: -> { puts "run" }.call
来源：http://hz.smart0.xyz/gtoxfsjuty.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shangyingyoupin.top/gtomgaudfd.html

[C13] 类型声明 / 类型注解
来源：http://hz.sysykeji.top/gtcxunfarj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.c1oappe.top/gtngfsawpm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tanke756.top/gtamfeobuv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.aizwys.cn/gtjhbpljnf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuanzx.com/gtamhezzld.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.birdmap.top/gtfeswwznl.html

Go:   func add(a, b int) int
来源：http://hz.xuanzx.com/gtgbnasigv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gogol.net.cn/gtrpkmdzmc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.meibo888.top/gtztkirdjn.html

[C14] 泛型函数
来源：http://hz.xingfuxueyuan.xyz/gtfqoqlkum.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zdqjudy.top/gtgjbrnoct.html

PHP:  // 无泛型
来源：http://hz.dashuyun.cn/gtmscanhpg.html

JS:   // 无泛型
来源：http://hz.pengpengdd.cyou/gtckezzsui.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shanyushiyangkeji.top/gtctsgmpyu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hysaishi.cn/gtsjaskweu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xuetiantiany.cn/gtuwrgdqfz.html

Ruby: # 无泛型
来源：http://hz.pycfn.com/gtrcfhbkmd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhijiandao.cn/gtlwsdkwkh.html

[C15] 解构 / 展开参数
来源：http://hz.zycfv.cn/gtyysggtfa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.pengpengdd.cyou/gtmtmmtzyp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhixingplan.top/gthwxnhgcd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.meibo888.top/gtnaafjcjd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.0kj1m.cn/gtxiwhoedt.html

Java: // 无解构
来源：http://hz.shzxlz.cn/gtqctzjeeb.html

Go:   // 无解构
来源：http://hz.zhixingplan.top/gttmcuevab.html

Ruby: a, b = pair
来源：http://hz.ivvv.top/gtevfejtrr.html

C#:   var (a, b) = pair;
来源：http://hz.cheryme.top/gtrroljzho.html

[C16] 函数 / 方法重载
来源：http://hz.pengpengdd.cyou/gtpmdlzdjc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.52xcode.cn/gtudytrddp.html

PHP:  // 无重载
来源：http://hz.svipenyu.cn/gtnsrdanis.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.meibo888.top/gtrngynrtj.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jianghu66.top/gttwtnmzdg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhaomingkeji.xyz/gteufnpdhz.html

Go:   // 无重载：用不同函数名
来源：http://hz.yangfankeji.com/gtgvenfvkq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shanyushiyangkeji.top/gtyhqtxneg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.andypj.xyz/gtvijrbngn.html

================================================================================
来源：http://hz.aizwys.cn/gtmlzcxtwi.html

D. 数组 / 列表 / 集合
来源：http://hz.ydzc1.top/gttokttwyc.html

================================================================================
来源：http://hz.xziqi.cn/gtsarvigzt.html

[D01] 创建数组 / 列表
来源：http://hz.gzhubu.top/gtvlvognpo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gaohongyu789.top/gtqpvlcbyf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenzaomai.com/gtuupvrhua.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.fzhhl.top/gtyyeggcwt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.birdmap.top/gtngevouvv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hfpthk.cn/gtvvmzpqbn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yuanzhike.top/gtkyfyohxy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangdashe.top/gtleizluks.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhoulong.xyz/gtorjoigzb.html

[D02] 追加元素到末尾
来源：http://hz.shzxlz.cn/gtoridgsoi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cdnleiting.top/gteiynwbaz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sxryk.cn/gtqlifpsfb.html

JS:   arr.push(4);
来源：http://hz.jinqigfzy.top/gtjxmjtxuj.html

TS:   arr.push(4);
来源：http://hz.shuidangran.top/gtfbetpemq.html

Java: list.add(4);
来源：http://hz.ydzc1.top/gttgujnzgc.html

Go:   arr = append(arr, 4)
来源：http://hz.yj20258.top/gtxyppotfm.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.sweek.top/gttxjrjrdk.html

C#:   list.Add(4);
来源：http://hz.ybcxt.top/gtvlqvbkdq.html

[D03] 在指定位置插入元素
来源：http://hz.tian-w.cn/gtftjweohr.html

Py:   arr.insert(0, 0)
来源：http://hz.havefunace.top/gtarwdauob.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hongshengwenyu.top/gtukrabbzg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.svipenyu.cn/gtthporibl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jlsjyb.cn/gtsnmcigzm.html

Java: list.add(0, 0);
来源：http://hz.dashuyun.cn/gtgoencpls.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shzxlz.cn/gtrnwkokmn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.havefunace.top/gtkgqsquah.html

C#:   list.Insert(0, 0);
来源：http://hz.zycfv.cn/gtuggaxfxf.html

[D04] 删除元素
来源：http://hz.dianchejie.cn/gtrqtxyfsx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinqigfzy.top/gtaesbytwk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.birdmap.top/gtlupfkvkk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.daxiang520.top/gtohcedkdb.html

TS:   arr.splice(0, 1);
来源：http://hz.hysaishi.cn/gtfqybwxfq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xziqi.cn/gtbbzeiwow.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.aibaodan.cn/gtkzuitcna.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.9152youxi.cn/gtxyttodsa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ivvv.top/gtkdmhtnbu.html

[D05] 访问与修改元素
来源：http://hz.ybcxt.top/gtlqsusorn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hammf.cn/gtpgbzhztl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj202588.top/gtlimkjonj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cqqwz.cn/gtdhuysizq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sweek.top/gtqrgxddoe.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cashguo.top/gtwdycktdl.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sweek.top/gtpixovthx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xylfe.cn/gtdmeaitgc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.havefunace.top/gtfwpodrwj.html

[D06] 数组长度
来源：http://hz.yuanzhike.top/gtolikawog.html

Py:   len(arr)
来源：http://hz.hnxiangtu.top/gtufikqsuz.html

PHP:  count($arr);
来源：http://hz.andypj.xyz/gtfljtffav.html

JS:   arr.length
来源：http://hz.jqgfzy.top/gtfmfffuwh.html

TS:   arr.length
来源：http://hz.yongpay.top/gtanmhyobg.html

Java: list.size();
来源：http://hz.ywan-chungtsiang.top/gtbptwlsyw.html

Go:   len(arr)
来源：http://hz.havefunace.top/gtoxcyotgy.html

Ruby: arr.length; arr.size
来源：http://hz.havefunace.top/gtuhimjhdy.html

C#:   list.Count;
来源：http://hz.guannengcc.top/gtuffpewrx.html

[D07] 切片 / 取子数组
来源：http://hz.wangdashe.top/gtemaxzoyt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cqqwz.cn/gtaaigddda.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yuxming.cn/gtihgyjiow.html

JS:   arr.slice(1, 4);
来源：http://hz.hywenlv.cn/gtmeeqcsey.html

TS:   arr.slice(1, 4);
来源：http://hz.wangdashe.top/gtdtcjqvgr.html

Java: list.subList(1, 4);
来源：http://hz.havefunace.top/gtzbpftoke.html

Go:   arr[1:4]
来源：http://hz.hfpthk.cn/gthodjhcwd.html

Ruby: arr[1, 3]
来源：http://hz.yonumen.top/gtbffsnvqg.html

C#:   list.GetRange(1, 3);
来源：http://hz.bjfxy.top/gtpzlznumu.html

[D08] 合并两个数组
来源：http://hz.hammf.cn/gtbnfbrdyi.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenlongwang.top/gtgyzceogg.html

PHP:  array_merge($a, $b);
来源：http://hz.zhixingplan.top/gtadlgmkfc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shanyushiyangtech.top/gtnbgrjtqt.html

TS:   [...a, ...b];
来源：http://hz.nwbrower.top/gtgufqgojz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sweek.top/gtxlqcgxqu.html

Go:   append(a, b...)
来源：http://hz.nanxinkj.top/gtekgnaqqq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hongshengwenyu.top/gtxwybhtve.html

C#:   a.Concat(b).ToList()
来源：http://hz.jyoumei.cn/gtcmkzecsh.html

[D09] 排序（升序）
来源：http://hz.jinghuilouyu.cn/gtkkendwln.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuetiantiany.cn/gtuaxmexzj.html

PHP:  sort($arr);
来源：http://hz.tian-w.cn/gtfoyjgwwp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.pengpengdd.cyou/gtwzpofkvg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.dianchejie.cn/gtwziubuld.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hnqzz.top/gtcahdjvcm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ehwqpu.com/gtawhtpalz.html

Ruby: arr.sort
来源：http://hz.shzxlz.cn/gtqmdthytv.html

C#:   list.Sort();
来源：http://hz.ydzc1.top/gtkghcstjt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ydzc1.top/gtyunrcrvk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xinyue.icu/gtelzvisia.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jyoumei.cn/gtwtesqivn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gtxhfjtmce.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.iojbl.cn/gtvsuvjtdk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.chenzaomai.com/gtgtruuild.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sufxvd.cn/gtesrbwrws.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shuidangran.top/gtwsdyvzde.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.pengpengdd.cyou/gtorbnpqmi.html

[D11] 反转数组
来源：http://hz.chenlongwang.top/gtlsehxoon.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.wangdashe.top/gtvuezpxsw.html

PHP:  array_reverse($arr);
来源：http://hz.ywan-chungtsiang.top/gteljcxhzf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xziqi.cn/gtrrrkjcrg.html

TS:   [...arr].reverse();
来源：http://hz.yj202588.top/gteuxvwxju.html

Java: Collections.reverse(list);
来源：http://hz.xinyue.icu/gtcjlidgav.html

Go:   slices.Reverse(arr)
来源：http://hz.jianghu66.top/gtrjdnlepr.html

Ruby: arr.reverse
来源：http://hz.chenzaomai.com/gtklvbaqcp.html

C#:   list.Reverse();
来源：http://hz.daxiang520.top/gtqnqndvlg.html

[D12] 查找元素下标
来源：http://hz.vqdsnc.cn/gttygwldga.html

Py:   arr.index(x);  x in arr
来源：http://hz.shanyushiyangtech.top/gtdncetwpu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.feifeiyinyue.top/gtjucgvwee.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtkcxdiulb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgufenzy.top/gtahkjiusz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zdqjudy.top/gtncwoxcwd.html

Go:   slices.Index(arr, x)
来源：http://hz.feifeiyinyue.top/gtdvwhnemj.html

Ruby: arr.index(x)
来源：http://hz.jianghu66.top/gthqzwqulm.html

C#:   list.IndexOf(x);
来源：http://hz.cashguo.top/gtqfgfgyfu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.meibo888.top/gtedxjlurl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.pengpengdd.cyou/gtbhxnjagr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shanyushiyangtech.top/gtotatofvb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cucudq.cn/gtyrdlcqim.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtcrbywrhk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hnqzz.top/gtwjkoanhm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jlsjyb.cn/gtawamsqsq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gzhubu.top/gtcunnsqir.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhijiandao.cn/gtikbmxxzu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.c1oappe.top/gtmsqstmnw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yuxming.cn/gtdkrsutwf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.vqdsnc.cn/gtvfnpxnhu.html

JS:   arr.map(x => x * 2)
来源：http://hz.jianghu66.top/gtrswndyjl.html

TS:   arr.map(x => x * 2)
来源：http://hz.aizwys.cn/gtiisqdosd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jianghu66.top/gtqlmxnutg.html

Go:   // 手写循环
来源：http://hz.nanxinkj.top/gtqgjjkxjx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yj20258888.top/gtjvugunyb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tianlin.xyz/gtrdflitsp.html

[D15] 去重
来源：http://hz.nanxinkj.top/gtxqgymlaj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jiagoushi.top/gthdifustx.html

PHP:  array_unique($arr);
来源：http://hz.smart0.xyz/gtrhwkpeut.html

JS:   [...new Set(arr)]
来源：http://hz.nwbrower.top/gteweszjto.html


<!-- 参考信息 -->