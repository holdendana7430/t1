代发 wailian999

[C02] 默认参数
来源：http://hz.ppjwa.cn/gtuvxuofob.html

Py:   def greet(name="World"): return name
来源：http://hz.sysykeji.top/gtyyobnaaq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.bjfxy.top/gtcjomhpat.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.dianchejie.cn/gtqchctvmr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinyuanbaomall.cn/gtzngupihr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.tanke756.top/gtblksddqz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gaohongyu789.top/gtqrswszlg.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhongyouzk.top/gtetwdzhkc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.sufxvd.cn/gtoejotefl.html

[C03] 可变参数
来源：http://hz.zdqjudy.top/gteygjbpnf.html

Py:   def total(*args): return sum(args)
来源：http://hz.aibaodan.cn/gtuagowmxz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.redwolf501.top/gtjmombdfp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.snrcjt.cn/gtpgtxmzzp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.quarkkingdee.top/gtxlmkjmpn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.vqdsnc.cn/gtkgijcghg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xuanzx.com/gtepznmfbd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zdqjudy.top/gtakalqjnt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenjidiqi.icu/gtrjhrbzze.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shzxlz.cn/gtjfxnftbd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yangfankeji.com/gtodamybed.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xuanzx.com/gtzmcpkfjm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtysyijarl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.bjfxy.top/gtruvonphs.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.birdmap.top/gtxzbftonx.html

Go:   // 无：用配置结构体参数
来源：http://hz.yangfankeji.com/gticyvowtd.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhoulong.xyz/gtmedziblh.html

C#:   f(a: 1, b: 2)
来源：http://hz.gotoacloud.top/gtzcysxuwk.html

[C05] 返回多个值
来源：http://hz.pengpengdd.cyou/gtmkoszfrr.html

Py:   return a, b
来源：http://hz.cheryme.top/gtaljigjon.html

PHP:  return [$a, $b];
来源：http://hz.jqgfzy.top/gtegiagfux.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.bjfxy.top/gtgeukdutf.html

TS:   return { a, b };
来源：http://hz.yuanzhike.top/gtbczuligy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.pycfn.com/gtdkihdijp.html

Go:   return a, b
来源：http://hz.iojbl.cn/gtdbnvyste.html

Ruby: return a, b
来源：http://hz.gotoacloud.top/gtwhaqteln.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hnxiangtu.top/gteqdcemxh.html

[C06] 匿名函数 / lambda
来源：http://hz.jinyuanbaomall.cn/gtvwiaiijb.html

Py:   square = lambda x: x * x
来源：http://hz.hammf.cn/gthwloedkx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.dianchejie.cn/gtdnhjkqad.html

JS:   const square = x => x * x;
来源：http://hz.zhoulong.xyz/gthpykudjg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jlsjyb.cn/gtbxzdcesv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jianghu66.top/gtszchljhm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xingfuxueyuan.xyz/gtnviiiipq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.snrcjt.cn/gtfsjoajzy.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gaohongyu789.top/gtljrlfgad.html

[C07] 把函数作为参数传入
来源：http://hz.wangshuangyany.cn/gtrasvdqpb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tian-w.cn/gtewagmhrb.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.fengsongda.top/gtnyqkycyi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cashguo.top/gtejueobcs.html

TS:   arr.map(String)
来源：http://hz.chenjidiqi.icu/gtmkibnxyb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.mhx1999.top/gtamvlotxa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhaomingkeji.xyz/gtqajzwmwt.html

Ruby: arr.map(&:upcase)
来源：http://hz.hnqzz.top/gtzreatbqv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gzhubu.top/gtfbszbmeu.html

[C08] 闭包
来源：http://hz.tian-w.cn/gtryuivdpe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zdqjudy.top/gtisxwbxqn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yanxiufei.cn/gtrmbczezb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shanyushiyangkeji.top/gtpppjmfyw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.havefunace.top/gtblnhtxak.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.kuanghao11.cn/gtupvfgwza.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.chenzaomai.com/gtsrrkzpow.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhixingplan.top/gtspagwusy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hammf.cn/gtphxksmuu.html

[C09] 递归
来源：http://hz.sweek.top/gtcluminec.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.52xcode.cn/gtnvwzvblw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yuxming.cn/gtyzxdlfzx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.fengsongda.top/gtmppmseay.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jyoumei.cn/gthanjmooo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yuxming.cn/gtznqnnvcz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dianchejie.cn/gtuuhthsbf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sufxvd.cn/gtsgxwmabo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cdnleiting.top/gtdvffuivy.html

[C10] 变量作用域
来源：http://hz.dianchejie.cn/gtqmutonir.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ivvv.top/gtzyuqloos.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.c1oappe.top/gtsptratde.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.pycfn.com/gtafflkjkv.html

TS:   同 JS
来源：http://hz.hnqzz.top/gtdbtlxrmd.html

Java: 方法内为块级作用域
来源：http://hz.zhiwuduotai.top/gtpyaatrtv.html

Go:   花括号块级作用域
来源：http://hz.zhengqikj.top/gtepcjjdfj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ybcxt.top/gtsmoadbbd.html

C#:   块级作用域
来源：http://hz.xziqi.cn/gtjybqbzwj.html

[C11] 模块导入与导出
来源：http://hz.ywan-chungtsiang.top/gtoqcqzjll.html

Py:   from module import func
来源：http://hz.tianlin.xyz/gtpekmounv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.fengsongda.top/gtfrsyiikp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhoulong.xyz/gtwcxgqmtq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.chenzaomai.com/gtuutxpyjm.html

Java: import java.util.List;
来源：http://hz.ydjk.org.cn/gtrgpimtln.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.chenlongwang.top/gtltxtbaok.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sxryk.cn/gtnnhnkpbd.html

C#:   using System.Text;
来源：http://hz.yangfankeji.com/gtlielnukz.html

[C12] 立即执行函数 IIFE
来源：http://hz.0kj1m.cn/gtwcxjsvox.html

Py:   (lambda: print("run"))()
来源：http://hz.daria6918.cn/gtcsddbgip.html

PHP:  (function () { echo "run"; })();
来源：http://hz.pengpengdd.cyou/gtrubejppl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jqgufenzy.top/gtdyadxtra.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shangyingyoupin.top/gtwsetgxke.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.snrcjt.cn/gtdzixqyxq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yangfankeji.com/gtuydxcztt.html

Ruby: -> { puts "run" }.call
来源：http://hz.hywenlv.cn/gthzbkrfvr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj202588.top/gttltffyem.html

[C13] 类型声明 / 类型注解
来源：http://hz.jinghuilouyu.cn/gtzrcznhjg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.feifeiyinyue.top/gtqvxbniet.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tianlin.xyz/gtkgubslgg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yangfankeji.com/gtkxtbqiqc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xinyue.icu/gtnfhlfstg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ydzc1.top/gtofmlktjb.html

Go:   func add(a, b int) int
来源：http://hz.nwbrower.top/gtgxgzxibl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yueranfly.top/gtqhgbxeed.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hywenlv.cn/gtesuvgfdd.html

[C14] 泛型函数
来源：http://hz.jinghuilouyu.cn/gtuqfgqyic.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.dashuyun.cn/gtebtbtcxs.html

PHP:  // 无泛型
来源：http://hz.xziqi.cn/gtrmmafjqi.html

JS:   // 无泛型
来源：http://hz.hongshengwenyu.top/gtlyhdbssc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ywan-chungtsiang.top/gtumgnehzw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gotoacloud.top/gtgkaqtklr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hfpthk.cn/gtzzjsbdve.html

Ruby: # 无泛型
来源：http://hz.andypj.xyz/gtlmdmeaes.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhaomingkeji.xyz/gtqxlbyrvo.html

[C15] 解构 / 展开参数
来源：http://hz.aizwys.cn/gtkkkutjyt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.havefunace.top/gthrwxlyqn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhaomingkeji.xyz/gtcszlqnyi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yongpay.top/gtfsccijam.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenlongwang.top/gtxmmbmvxa.html

Java: // 无解构
来源：http://hz.shanyushiyangtech.top/gtfuifzvdr.html

Go:   // 无解构
来源：http://hz.shanyushiyangtech.top/gtzffqcnld.html

Ruby: a, b = pair
来源：http://hz.ivvv.top/gtlrmclzux.html

C#:   var (a, b) = pair;
来源：http://hz.ivvv.top/gtanfbxuww.html

[C16] 函数 / 方法重载
来源：http://hz.nanxinkj.top/gtvjmdymdf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yj20258888.top/gtmrapkoce.html

PHP:  // 无重载
来源：http://hz.sxryk.cn/gtrixjlcgg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ydzc1.top/gtokejsbah.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.9152youxi.cn/gtigqrfbzl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sxryk.cn/gthlqzihwc.html

Go:   // 无重载：用不同函数名
来源：http://hz.birdmap.top/gtnmxadxdy.html

Ruby: # 无重载：靠动态参数
来源：http://hz.birdmap.top/gtccxcrksy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yvedp.cn/gtyyzjhtey.html

================================================================================
来源：http://hz.birdmap.top/gteheicuei.html

D. 数组 / 列表 / 集合
来源：http://hz.xuanzx.com/gtboqnyqmy.html

================================================================================
来源：http://hz.aibaodan.cn/gthqeymxxv.html

[D01] 创建数组 / 列表
来源：http://hz.chenjidiqi.icu/gtbtdounyg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigfzy.top/gtcejmpcqw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.nanxinkj.top/gtdpvhdxmb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tian-w.cn/gtzthugeun.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.chenzaomai.com/gtbshkkczt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.daxiang520.top/gtljcgumnn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hnxiangtu.top/gtsdgjjlhx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.svipenyu.cn/gtsrarljgv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinqigufen.top/gtqpilnjsx.html

[D02] 追加元素到末尾
来源：http://hz.xinyue.icu/gtmsntpxmn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hnqzz.top/gtfspdxvol.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.pycfn.com/gtdajnvajk.html

JS:   arr.push(4);
来源：http://hz.hnqzz.top/gtydmyqtxc.html

TS:   arr.push(4);
来源：http://hz.9152youxi.cn/gtnkllvzrk.html

Java: list.add(4);
来源：http://hz.52xcode.cn/gtoorqtfcv.html

Go:   arr = append(arr, 4)
来源：http://hz.hammf.cn/gtxbzygcev.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daxiang520.top/gtluwzfgyu.html

C#:   list.Add(4);
来源：http://hz.pycfn.com/gtbwsnaywx.html

[D03] 在指定位置插入元素
来源：http://hz.gotoacloud.top/gtzhrgjrxw.html

Py:   arr.insert(0, 0)
来源：http://hz.yj20258888.top/gtbpeyshdh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hongshengwenyu.top/gtyehlwfxa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.316326.xyz/gtgrimqgjf.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shzxlz.cn/gtefnwcjoy.html

Java: list.add(0, 0);
来源：http://hz.hysaishi.cn/gtmndqwdnp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhoulong.xyz/gtvbwzjakl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jlsjyb.cn/gtjdsmmwkk.html

C#:   list.Insert(0, 0);
来源：http://hz.hnxiangtu.top/gtjtwwkcfa.html

[D04] 删除元素
来源：http://hz.fengsongda.top/gtvltqwgfo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.birdmap.top/gtzcuicsrw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.daria6918.cn/gttdbjsgvm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ppjwa.cn/gtybtyyqod.html

TS:   arr.splice(0, 1);
来源：http://hz.fengsongda.top/gtfivewfei.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.guannengcc.top/gttgirtyqt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.svipenyu.cn/gtlikhjkll.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.svipenyu.cn/gtygpbfvda.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhiwuduotai.top/gtoxuzfsso.html

[D05] 访问与修改元素
来源：http://hz.pycfn.com/gthsllekcz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jlsjyb.cn/gtmvizkyfz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.tanke756.top/gtvzmgkxta.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sufxvd.cn/gtzoogyjhd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhoulong.xyz/gtucyorkhi.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yonumen.top/gtyjrrfjif.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jqgfzy.top/gtjtbaxtbp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.smart0.xyz/gtpwlsloif.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.birdmap.top/gtwawxubnp.html

[D06] 数组长度
来源：http://hz.yj20258.top/gtjbspifws.html

Py:   len(arr)
来源：http://hz.jianghu66.top/gtmkpalqmn.html

PHP:  count($arr);
来源：http://hz.wangshuangyany.cn/gtoyuybttu.html

JS:   arr.length
来源：http://hz.ybcxt.top/gtcbbhoyuc.html

TS:   arr.length
来源：http://hz.jiagoushi.top/gteyslnwxq.html

Java: list.size();
来源：http://hz.fzhhl.top/gtivylrvta.html

Go:   len(arr)
来源：http://hz.sufxvd.cn/gtvksyzbqv.html

Ruby: arr.length; arr.size
来源：http://hz.fengsongda.top/gtwzfwpvha.html

C#:   list.Count;
来源：http://hz.yanxiufei.cn/gtfhfkprxo.html

[D07] 切片 / 取子数组
来源：http://hz.vqdsnc.cn/gtuiqunsvi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.svipenyu.cn/gtirysvzzt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shzxlz.cn/gtzmvihfwe.html

JS:   arr.slice(1, 4);
来源：http://hz.yonumen.top/gtpzbcljxg.html

TS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtaegehtvm.html

Java: list.subList(1, 4);
来源：http://hz.nwbrower.top/gtlinugsfx.html

Go:   arr[1:4]
来源：http://hz.fzhhl.top/gtmjdwvmzq.html

Ruby: arr[1, 3]
来源：http://hz.nanxuanxn.top/gtroxclyde.html

C#:   list.GetRange(1, 3);
来源：http://hz.hysaishi.cn/gtbcafjmip.html

[D08] 合并两个数组
来源：http://hz.mhx1999.top/gtjizjoeft.html

Py:   a + b;  a.extend(b)
来源：http://hz.iojbl.cn/gtrdrxbdug.html

PHP:  array_merge($a, $b);
来源：http://hz.316326.xyz/gtucukyahr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cdnleiting.top/gtdaelkxda.html

TS:   [...a, ...b];
来源：http://hz.gzhubu.top/gtchhiaqte.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cashguo.top/gtetfaksvp.html

Go:   append(a, b...)
来源：http://hz.vqdsnc.cn/gtqrvqzilg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.fengsongda.top/gtdzthvbbr.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhoulong.xyz/gtjvzzcqpj.html

[D09] 排序（升序）
来源：http://hz.zhijiandao.cn/gtzlijdgnq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sysykeji.top/gtiuotntoq.html

PHP:  sort($arr);
来源：http://hz.meibo888.top/gtvaudmijr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.bjfxy.top/gtnsukpqac.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shanyushiyangtech.top/gtuccvidiv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yongpay.top/gtwfcjlteo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jyoumei.cn/gteiitdnzm.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gtulkyfyxe.html

C#:   list.Sort();
来源：http://hz.sysykeji.top/gtmsnxvdth.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hywenlv.cn/gtnsmebejp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhiwuduotai.top/gtpbnjvkic.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.andypj.xyz/gtjvusfyew.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.snrcjt.cn/gthvbovrsf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinyuanbaomall.cn/gtwltdsqbt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhiwuduotai.top/gtiwzgbxdi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.nwbrower.top/gtrxfvbgjn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hnqzz.top/gthpckqygg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ybcxt.top/gtzkdjwyba.html

[D11] 反转数组
来源：http://hz.shanyushiyangkeji.top/gtncjomkvq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sxryk.cn/gticcprtff.html

PHP:  array_reverse($arr);
来源：http://hz.hongshengwenyu.top/gtbehffnzb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cdnleiting.top/gtqxtduidk.html

TS:   [...arr].reverse();
来源：http://hz.zhiwuduotai.top/gtsoolmwaw.html

Java: Collections.reverse(list);
来源：http://hz.chenzaomai.com/gtsojgyptd.html

Go:   slices.Reverse(arr)
来源：http://hz.yvedp.cn/gtcwzabxdo.html

Ruby: arr.reverse
来源：http://hz.ydzc1.top/gtsvarvkcn.html

C#:   list.Reverse();
来源：http://hz.guannengcc.top/gtnhhegycz.html

[D12] 查找元素下标
来源：http://hz.fzhhl.top/gtmucpfzut.html

Py:   arr.index(x);  x in arr
来源：http://hz.0kj1m.cn/gtnwojfnra.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hammf.cn/gtjdvvfnrm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhaomingkeji.xyz/gtmmwqnnce.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gtbjhuezty.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jqgfzy.top/gtanslostq.html

Go:   slices.Index(arr, x)
来源：http://hz.shzxlz.cn/gtuqnfxofv.html

Ruby: arr.index(x)
来源：http://hz.xingfuxueyuan.xyz/gtucvdswom.html

C#:   list.IndexOf(x);
来源：http://hz.daria6918.cn/gtbxtorajy.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ybcxt.top/gtoidwwcie.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.guowangkeji.top/gtoghnosmc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jiagoushi.top/gthvmvnsrp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gthkjkyyqo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinqigfzy.top/gtflmblhid.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenjidiqi.icu/gthpobjemk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhoulong.xyz/gtlttshygu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.0kj1m.cn/gtsxjcguxv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tanke756.top/gtfsbqwviv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jqgufenzy.top/gtzaagbyil.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xylfe.cn/gtiwoarfzm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.wangdashe.top/gtscngxldp.html

JS:   arr.map(x => x * 2)
来源：http://hz.yuxming.cn/gtvwgddgnj.html

TS:   arr.map(x => x * 2)
来源：http://hz.tianlin.xyz/gtrfgzbdwf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cheryme.top/gtiqsecqdm.html

Go:   // 手写循环
来源：http://hz.c1oappe.top/gtrvwltniv.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shzxlz.cn/gtfhgwnxko.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.havefunace.top/gtrpzfmmbk.html

[D15] 去重
来源：http://hz.snrcjt.cn/gtpyyvbskm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.iojbl.cn/gtlhvzljve.html

PHP:  array_unique($arr);
来源：http://hz.hnxiangtu.top/gtyicbknde.html

JS:   [...new Set(arr)]
来源：http://hz.ybcxt.top/gtwkhrmirg.html

TS:   [...new Set(arr)]
来源：http://hz.snrcjt.cn/gtoibwhthw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ydzc1.top/gtyxxvxkrz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258888.top/gtludgvvjv.html

Ruby: arr.uniq
来源：http://hz.aizwys.cn/gtenjgqtci.html

C#:   list.Distinct().ToList()
来源：http://hz.jiagoushi.top/gtcmwmvdzf.html

[D16] 求和与平均值
来源：http://hz.snrcjt.cn/gtstlzplbq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jqgfzy.top/gtshkqzdud.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.dianchejie.cn/gtfeyowiwi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gogol.net.cn/gtnlnyqzil.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nwbrower.top/gttgkcqvzu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xuanzx.com/gtzuczvoyv.html

Go:   // 手写循环累加
来源：http://hz.hongshengwenyu.top/gtgtpssesb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shuidangran.top/gtnbbyxmkn.html

C#:   list.Sum();  list.Average()
来源：http://hz.shanyushiyangtech.top/gthgcpetvc.html

[D17] 最大值与最小值
来源：http://hz.nwbrower.top/gthennqpap.html

Py:   max(arr);  min(arr)
来源：http://hz.gogol.net.cn/gtkoyyuxlh.html

PHP:  max($arr);  min($arr);
来源：http://hz.hysaishi.cn/gtckkipttl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cqqwz.cn/gtlvtqqhpw.html

TS:   Math.max(...arr);
来源：http://hz.yj20258888.top/gthtcynyzt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuanzhike.top/gtcklhhoiu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.svipenyu.cn/gtbyosxpok.html

Ruby: arr.max;  arr.min
来源：http://hz.tian-w.cn/gtxvxthhon.html

C#:   list.Max();  list.Min()
来源：http://hz.andypj.xyz/gtccrexqgg.html

[D18] 扁平化嵌套数组
来源：http://hz.tian-w.cn/gtrkdwrkou.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cdnleiting.top/gtjwzhghtz.html

PHP:  array_merge(...$nested);
来源：http://hz.redwolf501.top/gtygbhljjd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.dashuyun.cn/gtyrdlxxsc.html

TS:   nested.flat();
来源：http://hz.yvedp.cn/gtireppvbr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yonumen.top/gtrquynmhy.html

Go:   // 手写双层循环
来源：http://hz.haohaochexian.top/gtuwmfglea.html

Ruby: nested.flatten
来源：http://hz.sweek.top/gthoqnnnvv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.316326.xyz/gtsktahpuw.html


<!-- 参考信息 -->