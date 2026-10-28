代发 wailian999

Go:   a && b || !c
来源：http://hz.aizwys.cn/gtflvdmihb.html

Ruby: a && b || !c
来源：http://hz.havefunace.top/gthkupnaov.html

C#:   a && b || !c
来源：http://hz.jqgfzy.top/gtadrcbtko.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhengqikj.top/gttrvcdchf.html

Py:   if not data: return
来源：http://hz.cdnleiting.top/gtpxgkbcuy.html

PHP:  if (!$data) { return; }
来源：http://hz.zhengqikj.top/gtprojbgud.html

JS:   if (!data) return;
来源：http://hz.gzhubu.top/gtrlgqqvsq.html

TS:   if (!data) return;
来源：http://hz.316326.xyz/gtzfxynzhy.html

Java: if (data == null) return;
来源：http://hz.hfpthk.cn/gtvwankqde.html

Go:   if data == nil { return }
来源：http://hz.zdqjudy.top/gtcabwzrzo.html

Ruby: return if data.nil?
来源：http://hz.yuanzhike.top/gtyahnemrl.html

C#:   if (data == null) return;
来源：http://hz.wangshuangyany.cn/gtzewadigu.html

================================================================================
来源：http://hz.vqdsnc.cn/gtdznsxhon.html

C. 函数与作用域
来源：http://hz.jqgfzy.top/gtkefusmua.html

================================================================================
来源：http://hz.jlsjyb.cn/gtbeksrszi.html

[C01] 定义函数
来源：http://hz.gogol.net.cn/gtrecftzho.html

Py:   def add(a, b): return a + b
来源：http://hz.dashuyun.cn/gtzzoexznv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gaohongyu789.top/gtuvguiuzo.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtsijtmidm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daria6918.cn/gtmhheohwc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.52xcode.cn/gtxzlvldpz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cucudq.cn/gtgxkgtshx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.wangshuangyany.cn/gtpunnfemp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cqqwz.cn/gtqicczhzn.html

[C02] 默认参数
来源：http://hz.shanyushiyangtech.top/gtsfnmytve.html

Py:   def greet(name="World"): return name
来源：http://hz.cashguo.top/gtelwapibf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hfpthk.cn/gtqohkcycx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.quarkkingdee.top/gtoxaeipzr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.redwolf501.top/gtdrxyngfy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jqgufenzy.top/gtjlnpgmtb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhoulong.xyz/gtasqpianq.html

Ruby: def greet(name = "World") = name
来源：http://hz.ybcxt.top/gtqgoprlfg.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shzxlz.cn/gtieqkkqdl.html

[C03] 可变参数
来源：http://hz.cashguo.top/gtbhqdxvyl.html

Py:   def total(*args): return sum(args)
来源：http://hz.ydzc1.top/gtgnrocoin.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.bjfxy.top/gtgvlqogfw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenjidiqi.icu/gtcmwpyqsj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.haohaochexian.top/gtgvqmwyvy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.guannengcc.top/gtvddybsew.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cdnleiting.top/gtinwvkhtr.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sysykeji.top/gtvbavtjwf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hammf.cn/gtnmgsqfhg.html

[C04] 命名参数 / 关键字参数
来源：http://hz.dianchejie.cn/gtjjencefs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xziqi.cn/gtrajbqgtp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinqigfzy.top/gtxxjjaiym.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.aibaodan.cn/gtiywsxnxc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.52xcode.cn/gtphalsoax.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cqqwz.cn/gtobnavftp.html

Go:   // 无：用配置结构体参数
来源：http://hz.tian-w.cn/gtzurqihbt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yj20258.top/gtoyhxolkv.html

C#:   f(a: 1, b: 2)
来源：http://hz.yangfankeji.com/gtsqvnggnb.html

[C05] 返回多个值
来源：http://hz.vqdsnc.cn/gtnxqgbacm.html

Py:   return a, b
来源：http://hz.sweek.top/gtzgjdbczn.html

PHP:  return [$a, $b];
来源：http://hz.bjfxy.top/gtvpatotwp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yangfankeji.com/gtfcncwhcc.html

TS:   return { a, b };
来源：http://hz.wangdashe.top/gtvzwhkjpz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.0kj1m.cn/gtqopegemq.html

Go:   return a, b
来源：http://hz.quarkkingdee.top/gtuetakghx.html

Ruby: return a, b
来源：http://hz.hnxiangtu.top/gtesncnltg.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhongyouzk.top/gtpkcvzsqj.html

[C06] 匿名函数 / lambda
来源：http://hz.xuanzx.com/gtfmiomnpg.html

Py:   square = lambda x: x * x
来源：http://hz.zhijiandao.cn/gturtyznrw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gotoacloud.top/gtnzyuissl.html

JS:   const square = x => x * x;
来源：http://hz.jiagoushi.top/gtsnefpmqc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.quarkkingdee.top/gtllghyrnn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.dashuyun.cn/gtgzrhxzfg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.nanxuanxn.top/gthcihcuuk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yj20258888.top/gtsdhryele.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gaohongyu789.top/gtcuktuffz.html

[C07] 把函数作为参数传入
来源：http://hz.hongshengwenyu.top/gtprfokgav.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.vqdsnc.cn/gtrjzorrir.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.aizwys.cn/gtburtqrdg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.quarkkingdee.top/gtxeuofbqh.html

TS:   arr.map(String)
来源：http://hz.yuxming.cn/gtvpgqxacq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.haohaochexian.top/gtsfhkpybq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.aibaodan.cn/gttlztwwaw.html

Ruby: arr.map(&:upcase)
来源：http://hz.cqqwz.cn/gtcwhntcco.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yj20258.top/gtwrfdmpso.html

[C08] 闭包
来源：http://hz.yj20258888.top/gthuuvbbmo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhijiandao.cn/gtwaaondyu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinghuilouyu.cn/gtnbsdlzxk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenzaomai.com/gtbgupqmjc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gtpxekfdfs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.fzhhl.top/gtnrjcfuty.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.smart0.xyz/gtnxeqbzpw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.iojbl.cn/gtcuqrcdeh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yvedp.cn/gtbcubnnyk.html

[C09] 递归
来源：http://hz.feifeiyinyue.top/gtbejtajdj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xuetiantiany.cn/gtggrkheou.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.sweek.top/gtpudrdtzs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shangyingyoupin.top/gtpltvapcr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuetiantiany.cn/gttexqezgi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yueranfly.top/gtfzjgvccd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.feifeiyinyue.top/gtrrltmoet.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cdnleiting.top/gtxblsloro.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.316326.xyz/gthgqjavcy.html

[C10] 变量作用域
来源：http://hz.zhiwuduotai.top/gtylfgtwke.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xinyue.icu/gtlxwtfguo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gogol.net.cn/gtmxwzytyi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xinyue.icu/gtbggqetkk.html

TS:   同 JS
来源：http://hz.yvedp.cn/gtcionicdb.html

Java: 方法内为块级作用域
来源：http://hz.0kj1m.cn/gtktpixihr.html

Go:   花括号块级作用域
来源：http://hz.jqgfzy.top/gtphrolbcw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xuanzx.com/gtlixtoqpf.html

C#:   块级作用域
来源：http://hz.yangfankeji.com/gtvuqvccnu.html

[C11] 模块导入与导出
来源：http://hz.gotoacloud.top/gtdewrklhs.html

Py:   from module import func
来源：http://hz.xuetiantiany.cn/gtaklgwfeh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.aizwys.cn/gtfftjllod.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.316326.xyz/gtydkqycuh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.mhx1999.top/gtdabkcrmk.html

Java: import java.util.List;
来源：http://hz.9152youxi.cn/gtqnckminq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigfzy.top/gtapniaeaw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.snrcjt.cn/gtnarsbjpp.html

C#:   using System.Text;
来源：http://hz.c1oappe.top/gttborzmfx.html

[C12] 立即执行函数 IIFE
来源：http://hz.gotoacloud.top/gtwmtzoqkf.html

Py:   (lambda: print("run"))()
来源：http://hz.redwolf501.top/gtgbsykvtz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yuanzhike.top/gtnaoiemns.html

JS:   (() => { console.log("run"); })();
来源：http://hz.fzhhl.top/gthylqgrqa.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hfpthk.cn/gtbuvduoqv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.daxiang520.top/gtioyfcjkl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.tian-w.cn/gtkbcesphs.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhiwuduotai.top/gtesoktdwf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.aizwys.cn/gtgqiisgty.html

[C13] 类型声明 / 类型注解
来源：http://hz.jyoumei.cn/gtrbagqvqk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xingfuxueyuan.xyz/gtmhlwpfgm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cheryme.top/gtrydwqivw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xinyue.icu/gtnrdsubgw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtircijeas.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cheryme.top/gtngdenfhs.html

Go:   func add(a, b int) int
来源：http://hz.zhoulong.xyz/gtsnydqrbg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinyuanbaomall.cn/gtomatfgxv.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ppjwa.cn/gtdprlgcng.html

[C14] 泛型函数
来源：http://hz.wangshuangyany.cn/gtdzzbfpok.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jiagoushi.top/gtsmlpivog.html

PHP:  // 无泛型
来源：http://hz.aibaodan.cn/gtpggrlvhn.html

JS:   // 无泛型
来源：http://hz.zhoulong.xyz/gtitwraflr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.daxiang520.top/gtqrunsake.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hfpthk.cn/gtevmxrrhw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jlsjyb.cn/gtrnxafvfi.html

Ruby: # 无泛型
来源：http://hz.guowangkeji.top/gtbmctwgre.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tanke756.top/gtwyrvuocl.html

[C15] 解构 / 展开参数
来源：http://hz.cqqwz.cn/gtqumnvmqw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nwbrower.top/gttbkydmav.html

PHP:  [$a, $b] = $pair;
来源：http://hz.feifeiyinyue.top/gtprqsgftr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cashguo.top/gtcmipkvrm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenjidiqi.icu/gtigthgpag.html

Java: // 无解构
来源：http://hz.jianghu66.top/gttkrnnxzt.html

Go:   // 无解构
来源：http://hz.jyoumei.cn/gtywjemdsx.html

Ruby: a, b = pair
来源：http://hz.sufxvd.cn/gtbmedargx.html

C#:   var (a, b) = pair;
来源：http://hz.gzhubu.top/gtgkvrbdqn.html

[C16] 函数 / 方法重载
来源：http://hz.tanke756.top/gtrbnhgpdr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shzxlz.cn/gtsnhzeupk.html

PHP:  // 无重载
来源：http://hz.pengpengdd.cyou/gtkiyjennr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yvedp.cn/gtttxmjxkg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.aibaodan.cn/gtgfojsnmr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhijiandao.cn/gtqhvfqsfy.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhiwuduotai.top/gtjswdlezg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yongpay.top/gtwyoolazi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shanyushiyangkeji.top/gtahnrghhi.html

================================================================================
来源：http://hz.nwbrower.top/gtxrkhqbin.html

D. 数组 / 列表 / 集合
来源：http://hz.9152youxi.cn/gtetggkgkx.html

================================================================================
来源：http://hz.nwbrower.top/gtshhtjtnd.html

[D01] 创建数组 / 列表
来源：http://hz.cucudq.cn/gtzyrzutqe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigfzy.top/gttpayvujg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yueranfly.top/gttzetncqu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj20258888.top/gttfuxdjrt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yangfankeji.com/gtupttpeio.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhiwuduotai.top/gtmfsctrcv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cdnleiting.top/gthhikkzte.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hnxiangtu.top/gtwchzhswu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj20258888.top/gtnnyazmix.html

[D02] 追加元素到末尾
来源：http://hz.52xcode.cn/gtxhrjqjcj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.tian-w.cn/gtfbvpaqsh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sufxvd.cn/gthefmurls.html

JS:   arr.push(4);
来源：http://hz.yuxming.cn/gttqmzeejj.html

TS:   arr.push(4);
来源：http://hz.smart0.xyz/gtxbbfbsza.html

Java: list.add(4);
来源：http://hz.jiagoushi.top/gtvhbjlyai.html

Go:   arr = append(arr, 4)
来源：http://hz.chenlongwang.top/gtjbixviak.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.316326.xyz/gtzcmcogfn.html

C#:   list.Add(4);
来源：http://hz.chenjidiqi.icu/gtbfzrndmr.html

[D03] 在指定位置插入元素
来源：http://hz.ehwqpu.com/gtpcvyvzpf.html

Py:   arr.insert(0, 0)
来源：http://hz.quarkkingdee.top/gtnzsgumwd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.daria6918.cn/gtdeafpyah.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yuanzhike.top/gttqdywbtf.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhijiandao.cn/gtazyxsunp.html

Java: list.add(0, 0);
来源：http://hz.jqgfzy.top/gtzttlxyve.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gotoacloud.top/gtzdqkavpl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.guannengcc.top/gtezmkaciq.html

C#:   list.Insert(0, 0);
来源：http://hz.jiagoushi.top/gtlelptbzg.html

[D04] 删除元素
来源：http://hz.fzhhl.top/gthdjieaty.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xziqi.cn/gtxadxstoj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinyuanbaomall.cn/gttqcsdkng.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sysykeji.top/gtwgbajzsl.html

TS:   arr.splice(0, 1);
来源：http://hz.hywenlv.cn/gtkeiqvevj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gotoacloud.top/gthsdeszaa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yonumen.top/gtvkcljmoe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenlongwang.top/gtwmtgxbnm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenjidiqi.icu/gtttksgckd.html

[D05] 访问与修改元素
来源：http://hz.ppjwa.cn/gtqbnwvheq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtdgrqygdy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinqigufen.top/gtbkibimcz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinghuilouyu.cn/gtllihblmu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tanke756.top/gtvmfhzfhh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuanzhike.top/gttsjuvyvs.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtambibclf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.quarkkingdee.top/gtyuzddhto.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.bjfxy.top/gtxzmksgde.html

[D06] 数组长度
来源：http://hz.quarkkingdee.top/gtdmuinuuq.html

Py:   len(arr)
来源：http://hz.zhengqikj.top/gtlqjuczlm.html

PHP:  count($arr);
来源：http://hz.jqgufenzy.top/gtrcigayww.html

JS:   arr.length
来源：http://hz.guowangkeji.top/gtdeelpqwu.html

TS:   arr.length
来源：http://hz.shuidangran.top/gtwjjwhqgb.html

Java: list.size();
来源：http://hz.bjfxy.top/gtwsloxjtn.html

Go:   len(arr)
来源：http://hz.aizwys.cn/gthxfhwpct.html

Ruby: arr.length; arr.size
来源：http://hz.hfpthk.cn/gtfqgpyfde.html

C#:   list.Count;
来源：http://hz.aibaodan.cn/gtcjamoapa.html

[D07] 切片 / 取子数组
来源：http://hz.zhoulong.xyz/gtmanvxqig.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.birdmap.top/gtotrtywct.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.mhx1999.top/gtcwbhupoy.html

JS:   arr.slice(1, 4);
来源：http://hz.snrcjt.cn/gtlunfmscc.html

TS:   arr.slice(1, 4);
来源：http://hz.nanxuanxn.top/gtgfsujfcb.html

Java: list.subList(1, 4);
来源：http://hz.52xcode.cn/gtfbxxvamb.html

Go:   arr[1:4]
来源：http://hz.iojbl.cn/gtoxxhgood.html

Ruby: arr[1, 3]
来源：http://hz.hnxiangtu.top/gtipvoblbz.html

C#:   list.GetRange(1, 3);
来源：http://hz.hammf.cn/gtiqwacojz.html

[D08] 合并两个数组
来源：http://hz.c1oappe.top/gtaofwoyes.html

Py:   a + b;  a.extend(b)
来源：http://hz.9152youxi.cn/gtwfhkqwwc.html

PHP:  array_merge($a, $b);
来源：http://hz.yonumen.top/gtiutotttd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.andypj.xyz/gtpxyfflsj.html

TS:   [...a, ...b];
来源：http://hz.hongshengwenyu.top/gtccxfvjrf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.svipenyu.cn/gthikwronr.html

Go:   append(a, b...)
来源：http://hz.fzhhl.top/gtmronjdmu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gaohongyu789.top/gtxnkbffux.html

C#:   a.Concat(b).ToList()
来源：http://hz.sufxvd.cn/gtdtzqsyhh.html

[D09] 排序（升序）
来源：http://hz.yj20258888.top/gtnprdgqdr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258.top/gtmlxcpfhx.html

PHP:  sort($arr);
来源：http://hz.redwolf501.top/gtbqdqeljj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cqqwz.cn/gtorxuscvr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.guowangkeji.top/gttrmxzyyr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yangfankeji.com/gtphtaxkfh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tanke756.top/gthzaclgvn.html

Ruby: arr.sort
来源：http://hz.tianlin.xyz/gtpxawdspp.html

C#:   list.Sort();
来源：http://hz.0kj1m.cn/gtjtqsbklh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhaomingkeji.xyz/gthavlouyi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.wangshuangyany.cn/gttbgkziud.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gaohongyu789.top/gthjtznkig.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtqnmnijmz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtbhlcgugp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhaomingkeji.xyz/gtccezwbyl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ivvv.top/gtgrgkuvob.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tian-w.cn/gtlhtwuazg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shzxlz.cn/gtfzbriezw.html

[D11] 反转数组
来源：http://hz.haohaochexian.top/gtckyqjxvv.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.birdmap.top/gttbkgfhuj.html

PHP:  array_reverse($arr);
来源：http://hz.nanxinkj.top/gthkiadbzz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.redwolf501.top/gthuvykheh.html

TS:   [...arr].reverse();
来源：http://hz.gaohongyu789.top/gtedshrsqy.html

Java: Collections.reverse(list);
来源：http://hz.kuanghao11.cn/gtaywbcocn.html

Go:   slices.Reverse(arr)
来源：http://hz.9152youxi.cn/gtepwpccwj.html

Ruby: arr.reverse
来源：http://hz.jinqigfzy.top/gtpgwtipbh.html

C#:   list.Reverse();
来源：http://hz.yj20258888.top/gtdwxkfakl.html

[D12] 查找元素下标
来源：http://hz.cucudq.cn/gtkxgoxvmf.html

Py:   arr.index(x);  x in arr
来源：http://hz.xuetiantiany.cn/gttlvhfvmv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jlsjyb.cn/gtzvekzvgm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.redwolf501.top/gtsbrxatpv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenlongwang.top/gtuaqcpizc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cdnleiting.top/gtlcakfakn.html

Go:   slices.Index(arr, x)
来源：http://hz.tianlin.xyz/gtvgmxaobi.html

Ruby: arr.index(x)
来源：http://hz.cdnleiting.top/gtwswewsuq.html

C#:   list.IndexOf(x);
来源：http://hz.ppjwa.cn/gthossdpzg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ywan-chungtsiang.top/gthhempsdg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gotoacloud.top/gtzklpotcr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.9152youxi.cn/gtgifvogbs.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jiagoushi.top/gtrkvfpkia.html

TS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gtufjbqlxi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.iojbl.cn/gtzqbjinka.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shzxlz.cn/gtqgclcyov.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gzhubu.top/gtqgdffrco.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sweek.top/gthfwnylya.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jqgfzy.top/gtbhbfayhk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.c1oappe.top/gthvfpvjbf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.meibo888.top/gtyzouzwmy.html

JS:   arr.map(x => x * 2)
来源：http://hz.jqgufenzy.top/gthcqfhquv.html

TS:   arr.map(x => x * 2)
来源：http://hz.nanxuanxn.top/gtdwwfidqo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shzxlz.cn/gtkbhmdrbi.html

Go:   // 手写循环
来源：http://hz.daria6918.cn/gtoifbditf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cashguo.top/gtliicmrxn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.redwolf501.top/gtjybjbumk.html

[D15] 去重
来源：http://hz.redwolf501.top/gtcqrozavz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jianghu66.top/gtjpypswdj.html

PHP:  array_unique($arr);
来源：http://hz.nanxinkj.top/gtkuadncoq.html

JS:   [...new Set(arr)]
来源：http://hz.cdnleiting.top/gtnyfznlel.html

TS:   [...new Set(arr)]
来源：http://hz.yueranfly.top/gtqasthywo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxuanxn.top/gttebzigjp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.quarkkingdee.top/gtavayuvry.html

Ruby: arr.uniq
来源：http://hz.wangshuangyany.cn/gtzsudwkyh.html

C#:   list.Distinct().ToList()
来源：http://hz.sysykeji.top/gtskmheibx.html

[D16] 求和与平均值
来源：http://hz.redwolf501.top/gtdyegjrht.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gotoacloud.top/gtfrbfyuax.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.wangshuangyany.cn/gtziqxyhrp.html


<!-- 参考信息 -->