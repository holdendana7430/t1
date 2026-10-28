代发 wailian999

Py:   if not data: return
来源：http://hz.quarkkingdee.top/gtkrtvhdwl.html

PHP:  if (!$data) { return; }
来源：http://hz.zhiwuduotai.top/gtbbninibe.html

JS:   if (!data) return;
来源：http://hz.redwolf501.top/gtluotkdeq.html

TS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gtujxzkleq.html

Java: if (data == null) return;
来源：http://hz.pengpengdd.cyou/gttxbyvcbg.html

Go:   if data == nil { return }
来源：http://hz.gogol.net.cn/gtnhmysuzq.html

Ruby: return if data.nil?
来源：http://hz.cheryme.top/gttpjjxtcb.html

C#:   if (data == null) return;
来源：http://hz.hysaishi.cn/gtdynltgqj.html

================================================================================
来源：http://hz.daxiang520.top/gtillhjnfx.html

C. 函数与作用域
来源：http://hz.zhixingplan.top/gtiixxrehj.html

================================================================================
来源：http://hz.pycfn.com/gtsofufjnm.html

[C01] 定义函数
来源：http://hz.daria6918.cn/gtyawiqmoq.html

Py:   def add(a, b): return a + b
来源：http://hz.haohaochexian.top/gtwfuloqpb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuetiantiany.cn/gtctfhbbpp.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tanke756.top/gththefijf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zdqjudy.top/gtwmxvglts.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtpncirpqf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xuanzx.com/gtkfmpclkr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jqgufenzy.top/gtndrurxzx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinqigufen.top/gtbihjrgqc.html

[C02] 默认参数
来源：http://hz.gogol.net.cn/gtvwscxiev.html

Py:   def greet(name="World"): return name
来源：http://hz.jyoumei.cn/gtkncfiiau.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinyuanbaomall.cn/gtrolddzbr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tian-w.cn/gtbkzikplo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.meibo888.top/gtqlpyghaz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.cheryme.top/gtpuxuikuy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.52xcode.cn/gtorrlhlud.html

Ruby: def greet(name = "World") = name
来源：http://hz.ivvv.top/gtknhnerhl.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xuetiantiany.cn/gtorxhecvp.html

[C03] 可变参数
来源：http://hz.dashuyun.cn/gtwdoioaop.html

Py:   def total(*args): return sum(args)
来源：http://hz.xziqi.cn/gtuhrwuzsx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cdnleiting.top/gtjkavubwd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sufxvd.cn/gtlkaksekg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnqzz.top/gtbcdauobq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jyoumei.cn/gtomxmifyg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.nanxuanxn.top/gtfocxsshj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xuanzx.com/gtfulwdbuq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gotoacloud.top/gttdctzasz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shanyushiyangtech.top/gtzgzsukgr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.iojbl.cn/gtqevdchzr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhixingplan.top/gtmlkolmjk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yangfankeji.com/gtuqzqapzt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.52xcode.cn/gtxirwqhtg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shanyushiyangtech.top/gtvpmggvoc.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinqigufen.top/gtswsvfwgt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.9152youxi.cn/gtnbklacas.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhixingplan.top/gtjqqqunqn.html

[C05] 返回多个值
来源：http://hz.chenzaomai.com/gtopzvcpry.html

Py:   return a, b
来源：http://hz.nanxinkj.top/gtqegijfbe.html

PHP:  return [$a, $b];
来源：http://hz.iojbl.cn/gtudjvhmmn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ivvv.top/gtffuzuobj.html

TS:   return { a, b };
来源：http://hz.yongpay.top/gthjgliqqd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jianghu66.top/gtcingnvkh.html

Go:   return a, b
来源：http://hz.guannengcc.top/gturyjgimm.html

Ruby: return a, b
来源：http://hz.havefunace.top/gtnxcpadmo.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sysykeji.top/gtbrkutsiz.html

[C06] 匿名函数 / lambda
来源：http://hz.zhongyouzk.top/gtwbaewssu.html

Py:   square = lambda x: x * x
来源：http://hz.zhijiandao.cn/gtuolibxph.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhoulong.xyz/gtdcgqhogl.html

JS:   const square = x => x * x;
来源：http://hz.ybcxt.top/gteybcpbjs.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.52xcode.cn/gtpmhvzixj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.9152youxi.cn/gtlqbtuvpk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yuxming.cn/gtljecekec.html

Ruby: square = ->(x) { x * x }
来源：http://hz.kuanghao11.cn/gtvrmixhvk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gtbghlneer.html

[C07] 把函数作为参数传入
来源：http://hz.gogol.net.cn/gtgnnnswjm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhijiandao.cn/gttatrsckb.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.quarkkingdee.top/gttevtytvk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jyoumei.cn/gtzgpcyrgr.html

TS:   arr.map(String)
来源：http://hz.haohaochexian.top/gttfjdamdr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgufenzy.top/gtdpxgxbfx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.nanxinkj.top/gttomyurid.html

Ruby: arr.map(&:upcase)
来源：http://hz.sysykeji.top/gtczfxlyly.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jiagoushi.top/gtvfpepttm.html

[C08] 闭包
来源：http://hz.ydjk.org.cn/gtadvnaycy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jlsjyb.cn/gtbjrlydfo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.pengpengdd.cyou/gtveslvmtu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shanyushiyangkeji.top/gtrfzdydfb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtoshifqve.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenjidiqi.icu/gtngwmmlah.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.meibo888.top/gtxzxdcrvl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.daria6918.cn/gtoutyltay.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtitwtygnk.html

[C09] 递归
来源：http://hz.jinqigufen.top/gtegelizup.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ydjk.org.cn/gtvgsrcbut.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yueranfly.top/gtauvqrvyb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.meibo888.top/gtifrolfxr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sysykeji.top/gtesjqvpyt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.fengsongda.top/gtzlyvztah.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhoulong.xyz/gtnzdrdcbt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.c1oappe.top/gtfehrocsy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yuxming.cn/gtkvbrgpyq.html

[C10] 变量作用域
来源：http://hz.ydzc1.top/gtaffjiuds.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shangyingyoupin.top/gtphejtxds.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nwbrower.top/gtadejvdpo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gotoacloud.top/gtyrsvfzmv.html

TS:   同 JS
来源：http://hz.yueranfly.top/gtnyemxvrf.html

Java: 方法内为块级作用域
来源：http://hz.ehwqpu.com/gtexkjhkey.html

Go:   花括号块级作用域
来源：http://hz.birdmap.top/gtrpowgxzw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xuanzx.com/gtgccnwdjm.html

C#:   块级作用域
来源：http://hz.jinghuilouyu.cn/gtmwlhqtak.html

[C11] 模块导入与导出
来源：http://hz.yj202588.top/gtwvrohrkh.html

Py:   from module import func
来源：http://hz.sweek.top/gtkqhuwcjz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hongshengwenyu.top/gtohjyorcw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hongshengwenyu.top/gtwoyyiavm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tianlin.xyz/gtkrhmhmtq.html

Java: import java.util.List;
来源：http://hz.guannengcc.top/gtywfqbpen.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cdnleiting.top/gtwqvvcpih.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.pycfn.com/gtnzasodjy.html

C#:   using System.Text;
来源：http://hz.jqgfzy.top/gtvtpgrurq.html

[C12] 立即执行函数 IIFE
来源：http://hz.ydjk.org.cn/gtivlbfpvx.html

Py:   (lambda: print("run"))()
来源：http://hz.vqdsnc.cn/gtcacugcoc.html

PHP:  (function () { echo "run"; })();
来源：http://hz.guannengcc.top/gtiohztohv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hysaishi.cn/gttksxiufv.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinghuilouyu.cn/gtvfrsnsud.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhoulong.xyz/gtldpxpqts.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.redwolf501.top/gtlcnbzxns.html

Ruby: -> { puts "run" }.call
来源：http://hz.cheryme.top/gtafwiagyc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhengqikj.top/gtnxfclbyv.html

[C13] 类型声明 / 类型注解
来源：http://hz.fengsongda.top/gtykyffijl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenzaomai.com/gtxoojckzf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenzaomai.com/gthybsfhvo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xuanzx.com/gtteeuvopu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuanzx.com/gtfifmtznm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtoswdqutf.html

Go:   func add(a, b int) int
来源：http://hz.jlsjyb.cn/gtebaccjmp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ybcxt.top/gtbkwdhyjn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.wangshuangyany.cn/gtnxgiuske.html

[C14] 泛型函数
来源：http://hz.cdnleiting.top/gtqoqjktuk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.andypj.xyz/gttfyuedsh.html

PHP:  // 无泛型
来源：http://hz.sxryk.cn/gtpptqcxau.html

JS:   // 无泛型
来源：http://hz.cashguo.top/gtitlylick.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jlsjyb.cn/gtwipmadwy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shzxlz.cn/gtkhqptoyc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj202588.top/gtfuasflpk.html

Ruby: # 无泛型
来源：http://hz.ywan-chungtsiang.top/gtijwvumcb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pengpengdd.cyou/gtnzqenxyr.html

[C15] 解构 / 展开参数
来源：http://hz.yuanzhike.top/gttgttswhd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.haohaochexian.top/gtxbgkmwqz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.daxiang520.top/gtwpmqicdc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yonumen.top/gtbyusffdw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yj20258.top/gtlnfisbvv.html

Java: // 无解构
来源：http://hz.yvedp.cn/gtszqxwdrz.html

Go:   // 无解构
来源：http://hz.ehwqpu.com/gtrbynzzeh.html

Ruby: a, b = pair
来源：http://hz.tianlin.xyz/gtyuhcxcxq.html

C#:   var (a, b) = pair;
来源：http://hz.haohaochexian.top/gtxoluvxod.html

[C16] 函数 / 方法重载
来源：http://hz.feifeiyinyue.top/gtdbxbaxnp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.0kj1m.cn/gtiwvnmkqe.html

PHP:  // 无重载
来源：http://hz.xylfe.cn/gttirxbrzo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxuanxn.top/gtjnviqpnu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jqgfzy.top/gtnbzycayq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cqqwz.cn/gtltpugjpg.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhengqikj.top/gtbenlxlpm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.pengpengdd.cyou/gtallhkhbp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yuxming.cn/gtnlhlhikf.html

================================================================================
来源：http://hz.zhongyouzk.top/gtmdhsoloq.html

D. 数组 / 列表 / 集合
来源：http://hz.jinqigufen.top/gtfmhlsree.html

================================================================================
来源：http://hz.haohaochexian.top/gtkiqqgywy.html

[D01] 创建数组 / 列表
来源：http://hz.hysaishi.cn/gterlzvqgc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hnxiangtu.top/gtsqnlcqqx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jqgufenzy.top/gtheadtgrw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.snrcjt.cn/gtcoaexzlp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hywenlv.cn/gtkzjdzynz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.andypj.xyz/gtplypricx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yongpay.top/gteohlqwnm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.dashuyun.cn/gtacvukpyh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gzhubu.top/gtmwruefca.html

[D02] 追加元素到末尾
来源：http://hz.xingfuxueyuan.xyz/gtsnunhgtj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.wangshuangyany.cn/gtmhwhpwwr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgfzy.top/gteqajxufu.html

JS:   arr.push(4);
来源：http://hz.ydjk.org.cn/gtckspkxua.html

TS:   arr.push(4);
来源：http://hz.yj20258888.top/gtlconcrhu.html

Java: list.add(4);
来源：http://hz.c1oappe.top/gtmvymvymp.html

Go:   arr = append(arr, 4)
来源：http://hz.316326.xyz/gtquxitrhy.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jiagoushi.top/gtfyrmbccs.html

C#:   list.Add(4);
来源：http://hz.jinqigfzy.top/gtmwpuhegc.html

[D03] 在指定位置插入元素
来源：http://hz.pycfn.com/gtzedjexmk.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangkeji.top/gtinergcuq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yvedp.cn/gtvqilvqez.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ydjk.org.cn/gtcijsmgyp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yonumen.top/gtjsbfjrby.html

Java: list.add(0, 0);
来源：http://hz.hfpthk.cn/gtxspzuyfw.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.redwolf501.top/gthhfhuuye.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.fzhhl.top/gtmjxkafxz.html

C#:   list.Insert(0, 0);
来源：http://hz.yvedp.cn/gtceojpebv.html

[D04] 删除元素
来源：http://hz.vqdsnc.cn/gtcofncanv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuanzx.com/gtzwmwhrvx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.daxiang520.top/gtalhdwevh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jyoumei.cn/gtdintogph.html

TS:   arr.splice(0, 1);
来源：http://hz.pycfn.com/gtdccmjrqi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.fzhhl.top/gtaypqlgry.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cashguo.top/gthqlopapj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.havefunace.top/gttcgjqbnt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.redwolf501.top/gtwfkyemve.html

[D05] 访问与修改元素
来源：http://hz.jinghuilouyu.cn/gtzruplyyx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ehwqpu.com/gtxzqrgjll.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sysykeji.top/gtefjkrfoy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hywenlv.cn/gtlhnngdki.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xuanzx.com/gtydkgqvss.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinqigfzy.top/gtokcawzpg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.guannengcc.top/gtvrbcwfeq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sufxvd.cn/gthhpwwtom.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nanxinkj.top/gtqymzgkav.html

[D06] 数组长度
来源：http://hz.yj20258888.top/gtcbbqfopi.html

Py:   len(arr)
来源：http://hz.chenlongwang.top/gtamwzheyt.html

PHP:  count($arr);
来源：http://hz.dianchejie.cn/gtkitrqnkw.html

JS:   arr.length
来源：http://hz.yangfankeji.com/gthvmtwpon.html

TS:   arr.length
来源：http://hz.cucudq.cn/gtcdcivxvi.html

Java: list.size();
来源：http://hz.cashguo.top/gtqshssrme.html

Go:   len(arr)
来源：http://hz.nanxinkj.top/gtrunppbib.html

Ruby: arr.length; arr.size
来源：http://hz.jianghu66.top/gtygurffpa.html

C#:   list.Count;
来源：http://hz.ybcxt.top/gtujhlsexq.html

[D07] 切片 / 取子数组
来源：http://hz.zhijiandao.cn/gtwwhzozho.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gaohongyu789.top/gtjpeozxpo.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhiwuduotai.top/gtyveyyyek.html

JS:   arr.slice(1, 4);
来源：http://hz.andypj.xyz/gtacbgtjeq.html

TS:   arr.slice(1, 4);
来源：http://hz.0kj1m.cn/gteijwazfa.html

Java: list.subList(1, 4);
来源：http://hz.sweek.top/gtswwwtkbz.html

Go:   arr[1:4]
来源：http://hz.yueranfly.top/gtjaxrcugn.html

Ruby: arr[1, 3]
来源：http://hz.0kj1m.cn/gtapjwjvbv.html

C#:   list.GetRange(1, 3);
来源：http://hz.zycfv.cn/gtdzsrxiyu.html

[D08] 合并两个数组
来源：http://hz.nanxuanxn.top/gtgshselnk.html

Py:   a + b;  a.extend(b)
来源：http://hz.jqgfzy.top/gtyrallgdu.html

PHP:  array_merge($a, $b);
来源：http://hz.316326.xyz/gtkluugwzh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ehwqpu.com/gtypwlpfwv.html

TS:   [...a, ...b];
来源：http://hz.yj20258888.top/gtqnngsquk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ivvv.top/gtexkvjzdp.html

Go:   append(a, b...)
来源：http://hz.feifeiyinyue.top/gtwjrxskuo.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hammf.cn/gtysnxavwy.html

C#:   a.Concat(b).ToList()
来源：http://hz.yueranfly.top/gtmtgtgxsb.html

[D09] 排序（升序）
来源：http://hz.xingfuxueyuan.xyz/gthyfqehty.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtbzguejxk.html

PHP:  sort($arr);
来源：http://hz.vqdsnc.cn/gtxpjancvc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.9152youxi.cn/gteyqrmofe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhijiandao.cn/gtrcidskrm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shangyingyoupin.top/gtuczhgnuk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hammf.cn/gtwlyjaxax.html

Ruby: arr.sort
来源：http://hz.yvedp.cn/gtiwmpymyr.html

C#:   list.Sort();
来源：http://hz.shangyingyoupin.top/gttdkjgvzx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.daria6918.cn/gtoxyskxed.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.guowangkeji.top/gtzvpnvnqb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.quarkkingdee.top/gtkcnscush.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangtech.top/gtazemawfa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yangfankeji.com/gtrsjwrxid.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhengqikj.top/gthnnfxssm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhaomingkeji.xyz/gtvbyjismd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.9152youxi.cn/gtmrdruydo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xingfuxueyuan.xyz/gtzrxlxwvw.html

[D11] 反转数组
来源：http://hz.fzhhl.top/gtulxdchkl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ydjk.org.cn/gtsqhywbcs.html

PHP:  array_reverse($arr);
来源：http://hz.tian-w.cn/gthsqhxmhp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yvedp.cn/gtqseyfnvd.html

TS:   [...arr].reverse();
来源：http://hz.hfpthk.cn/gtixtbujvu.html

Java: Collections.reverse(list);
来源：http://hz.zhixingplan.top/gthasdriqd.html

Go:   slices.Reverse(arr)
来源：http://hz.9152youxi.cn/gtugxqxowl.html

Ruby: arr.reverse
来源：http://hz.mhx1999.top/gtqxiupbpq.html

C#:   list.Reverse();
来源：http://hz.hysaishi.cn/gtfyvymytj.html

[D12] 查找元素下标
来源：http://hz.jinqigfzy.top/gtjpmnbzkb.html

Py:   arr.index(x);  x in arr
来源：http://hz.hnxiangtu.top/gtvvzwyxsa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ydjk.org.cn/gtemvlzmff.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xuanzx.com/gtvgdywlze.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.kuanghao11.cn/gtthskydlo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.daxiang520.top/gtqurgsrxn.html

Go:   slices.Index(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtinjlevlp.html

Ruby: arr.index(x)
来源：http://hz.cashguo.top/gteveymyhx.html

C#:   list.IndexOf(x);
来源：http://hz.yongpay.top/gteinwkxdb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.svipenyu.cn/gtifvsnhyh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhiwuduotai.top/gtfdfytljl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenzaomai.com/gtwznoimrd.html

JS:   arr.filter(x => x > 3)
来源：http://hz.0kj1m.cn/gtdjpllxhs.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ehwqpu.com/gtolfbfdsb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hnxiangtu.top/gttnjxliva.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.daxiang520.top/gtfnpyrfsw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.meibo888.top/gtcafiwvgv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yangfankeji.com/gtvamntogk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.daxiang520.top/gtzxzkhlgt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.kuanghao11.cn/gtfewigzuq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aibaodan.cn/gtgijxhpjl.html

JS:   arr.map(x => x * 2)
来源：http://hz.fengsongda.top/gtiedfepfk.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhiwuduotai.top/gtvmgglzuj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.pengpengdd.cyou/gtgalalqrk.html

Go:   // 手写循环
来源：http://hz.jiagoushi.top/gteehpwcds.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cheryme.top/gtygjcmubd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuxming.cn/gtxtosmaxp.html

[D15] 去重
来源：http://hz.wangdashe.top/gtdxxhbqkh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hnxiangtu.top/gtddwmuxek.html

PHP:  array_unique($arr);
来源：http://hz.nwbrower.top/gterqqahkd.html

JS:   [...new Set(arr)]
来源：http://hz.dianchejie.cn/gtfeehroof.html

TS:   [...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gtmqghtzij.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.quarkkingdee.top/gtymfxdpbn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yvedp.cn/gtzaitdvyw.html

Ruby: arr.uniq
来源：http://hz.shanyushiyangkeji.top/gttwahsqty.html

C#:   list.Distinct().ToList()
来源：http://hz.fzhhl.top/gtdseflnhu.html

[D16] 求和与平均值
来源：http://hz.hnqzz.top/gtngvnhrhe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ivvv.top/gtpwmyuawr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cdnleiting.top/gtfbxtnaun.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinyuanbaomall.cn/gtykhecjji.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenlongwang.top/gtylqabzzi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.guannengcc.top/gtwfyhkhsh.html

Go:   // 手写循环累加
来源：http://hz.havefunace.top/gtcvspeove.html


<!-- 参考信息 -->