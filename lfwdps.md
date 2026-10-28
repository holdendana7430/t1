代发 wailian999

================================================================================
来源：http://hz.wangdashe.top/gtbqabfany.html

C. 函数与作用域
来源：http://hz.yuxming.cn/gteryowjne.html

================================================================================
来源：http://hz.daxiang520.top/gtsfatckra.html

[C01] 定义函数
来源：http://hz.hongshengwenyu.top/gtsqluhnxs.html

Py:   def add(a, b): return a + b
来源：http://hz.hywenlv.cn/gtxemdfgji.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yangfankeji.com/gtamwdlzqh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtpcnoifrz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhixingplan.top/gtjgivfwug.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.svipenyu.cn/gthkceqwcf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinqigfzy.top/gtqhvlkeqo.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhaomingkeji.xyz/gtilklrqab.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.guowangkeji.top/gtcgbunkpt.html

[C02] 默认参数
来源：http://hz.hnxiangtu.top/gtwybndppz.html

Py:   def greet(name="World"): return name
来源：http://hz.aizwys.cn/gtygajpvgs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.mhx1999.top/gtvyrpieal.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ydjk.org.cn/gttklkvgiq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ywan-chungtsiang.top/gtczycwxkg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.wangdashe.top/gtchhgmgkn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xuetiantiany.cn/gtrghtcwbe.html

Ruby: def greet(name = "World") = name
来源：http://hz.sxryk.cn/gthdlqlwua.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ivvv.top/gtjlbxovfj.html

[C03] 可变参数
来源：http://hz.ivvv.top/gtlgqnvyhp.html

Py:   def total(*args): return sum(args)
来源：http://hz.shuidangran.top/gtkbmqczjt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ehwqpu.com/gtpstsfaoh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yangfankeji.com/gtiakdkunk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.birdmap.top/gtoqwvtcyt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhengqikj.top/gtqqlmkxvs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.chenzaomai.com/gtpinmzavp.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ydzc1.top/gtzalaawfv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.c1oappe.top/gtbiekruvn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinqigfzy.top/gtrlkokzti.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yuanzhike.top/gtgfsvlicl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinyuanbaomall.cn/gtoruaoepc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.nanxuanxn.top/gtxzwyuxlb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xuanzx.com/gtksvbfnwt.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.gzhubu.top/gtgeuntrve.html

Go:   // 无：用配置结构体参数
来源：http://hz.dashuyun.cn/gtwlfkaboz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.0kj1m.cn/gtnmkuovqo.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtmlqapqoa.html

[C05] 返回多个值
来源：http://hz.gzhubu.top/gtfewlaopz.html

Py:   return a, b
来源：http://hz.jyoumei.cn/gtspubgmpr.html

PHP:  return [$a, $b];
来源：http://hz.zhengqikj.top/gtpqlxudlr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhijiandao.cn/gtxpkqvdqm.html

TS:   return { a, b };
来源：http://hz.guowangkeji.top/gtazsuiqti.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cashguo.top/gtyderjdws.html

Go:   return a, b
来源：http://hz.fzhhl.top/gtdytzibin.html

Ruby: return a, b
来源：http://hz.ivvv.top/gtkzallzks.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yvedp.cn/gtfvgkjoqj.html

[C06] 匿名函数 / lambda
来源：http://hz.cdnleiting.top/gtcjbntlwz.html

Py:   square = lambda x: x * x
来源：http://hz.tian-w.cn/gtijlfzxzp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.kuanghao11.cn/gtiyuybcjr.html

JS:   const square = x => x * x;
来源：http://hz.fengsongda.top/gtusfzkgmd.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sxryk.cn/gtfhznarqt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhijiandao.cn/gtorgomhwo.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ywan-chungtsiang.top/gtcmgsmogm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hnqzz.top/gtepoxlznx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.nanxinkj.top/gtrzqmrttz.html

[C07] 把函数作为参数传入
来源：http://hz.hfpthk.cn/gteugwjlol.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tanke756.top/gtnpgedfkh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shanyushiyangtech.top/gtkqececld.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hfpthk.cn/gtnmejugdk.html

TS:   arr.map(String)
来源：http://hz.pycfn.com/gtnjpvzdro.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hywenlv.cn/gtzybtpepy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sxryk.cn/gtnufjxzck.html

Ruby: arr.map(&:upcase)
来源：http://hz.tanke756.top/gtwkpkycup.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xinyue.icu/gtnqegwlem.html

[C08] 闭包
来源：http://hz.wangshuangyany.cn/gtldpwbjuh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.pycfn.com/gtbibjrsly.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tianlin.xyz/gtcfyodlup.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.redwolf501.top/gtnmddycli.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sweek.top/gthmuqfqgl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.fzhhl.top/gtuihnovos.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shanyushiyangkeji.top/gtqacvxeii.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.andypj.xyz/gtbzljvgrs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj20258888.top/gtpeyomthu.html

[C09] 递归
来源：http://hz.aizwys.cn/gtgfkjfbiy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.quarkkingdee.top/gtkzraccjt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.mhx1999.top/gthvdubxgg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxuanxn.top/gttvjjzjtn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shzxlz.cn/gtrudklbff.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jinqigufen.top/gtbilwrouw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.316326.xyz/gtfaiedeiv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.52xcode.cn/gtcavhhinx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hnxiangtu.top/gtvvnzygha.html

[C10] 变量作用域
来源：http://hz.shangyingyoupin.top/gtgzktmlwj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tian-w.cn/gtpdtfkttd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhongyouzk.top/gtrrnqsyhc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sweek.top/gtwczxrtee.html

TS:   同 JS
来源：http://hz.meibo888.top/gteapnudul.html

Java: 方法内为块级作用域
来源：http://hz.zhixingplan.top/gtdjcbpdvl.html

Go:   花括号块级作用域
来源：http://hz.shanyushiyangkeji.top/gtigxpbcwu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.dianchejie.cn/gtfnaizsjc.html

C#:   块级作用域
来源：http://hz.cdnleiting.top/gtdqzqlvht.html

[C11] 模块导入与导出
来源：http://hz.cucudq.cn/gtobcowimt.html

Py:   from module import func
来源：http://hz.yonumen.top/gtvtaxnkvc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sxryk.cn/gtneclvvso.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.52xcode.cn/gtrfvzkuqb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.kuanghao11.cn/gtaehoubij.html

Java: import java.util.List;
来源：http://hz.shuidangran.top/gtapmomurn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cdnleiting.top/gtghfakklp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ydzc1.top/gtneulymun.html

C#:   using System.Text;
来源：http://hz.andypj.xyz/gtiopdguzk.html

[C12] 立即执行函数 IIFE
来源：http://hz.yuanzhike.top/gtyrlbuygy.html

Py:   (lambda: print("run"))()
来源：http://hz.redwolf501.top/gtkvjvqkfz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxinkj.top/gtvkbzkurs.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jqgufenzy.top/gtaradcvjs.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hywenlv.cn/gtruonvzed.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.smart0.xyz/gtmxksllvm.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sweek.top/gtcmextitz.html

Ruby: -> { puts "run" }.call
来源：http://hz.aibaodan.cn/gtletmkxog.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xingfuxueyuan.xyz/gtnljaujhy.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhixingplan.top/gtytdvckhe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guowangkeji.top/gtcvvlczqh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnqzz.top/gtdtfjpifa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hnxiangtu.top/gtxqmtskvz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hammf.cn/gtdvlsewto.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtzmtbpwsf.html

Go:   func add(a, b int) int
来源：http://hz.sweek.top/gtoxbuupkg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuxming.cn/gtfgikexip.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cashguo.top/gtikgtegfj.html

[C14] 泛型函数
来源：http://hz.xylfe.cn/gtymgwcirz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hammf.cn/gtbrpbyimw.html

PHP:  // 无泛型
来源：http://hz.yuanzhike.top/gtonhtbjnh.html

JS:   // 无泛型
来源：http://hz.zdqjudy.top/gtlnytfxzh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shangyingyoupin.top/gtjxdppxze.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hfpthk.cn/gtvpyrzebd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenjidiqi.icu/gtjcikqamo.html

Ruby: # 无泛型
来源：http://hz.xuanzx.com/gtnmqdnygo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhijiandao.cn/gtpfsbjsmn.html

[C15] 解构 / 展开参数
来源：http://hz.gotoacloud.top/gtnkmmacly.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ivvv.top/gtnyobwpaj.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj20258888.top/gtkkofqqdp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gtxucqeyed.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yuanzhike.top/gtpxqgmchi.html

Java: // 无解构
来源：http://hz.yuanzhike.top/gtfhdlkdja.html

Go:   // 无解构
来源：http://hz.yangfankeji.com/gtykavjejo.html

Ruby: a, b = pair
来源：http://hz.birdmap.top/gtzwobpvfu.html

C#:   var (a, b) = pair;
来源：http://hz.dianchejie.cn/gtaxonjtht.html

[C16] 函数 / 方法重载
来源：http://hz.feifeiyinyue.top/gtlvrspzxd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xylfe.cn/gtzkjfyudx.html

PHP:  // 无重载
来源：http://hz.jyoumei.cn/gtkibmvljq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gzhubu.top/gttjjzixmc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.vqdsnc.cn/gtcqzxizig.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.svipenyu.cn/gtoxvkylah.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgufenzy.top/gthymzfmia.html

Ruby: # 无重载：靠动态参数
来源：http://hz.aizwys.cn/gtrumeipux.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ivvv.top/gtjilmtcvp.html

================================================================================
来源：http://hz.gotoacloud.top/gtghepuerb.html

D. 数组 / 列表 / 集合
来源：http://hz.0kj1m.cn/gtkuurgqvn.html

================================================================================
来源：http://hz.c1oappe.top/gtjvbnuczk.html

[D01] 创建数组 / 列表
来源：http://hz.yangfankeji.com/gtjvkmprrp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ybcxt.top/gtyonwdzpo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xinyue.icu/gtbczzanig.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jqgfzy.top/gtdkzftpmx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sweek.top/gtaksssszn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xuetiantiany.cn/gtlopalxrn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yuxming.cn/gtxxaewnnl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhijiandao.cn/gtkibedqgk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj20258.top/gtwtcczhjg.html

[D02] 追加元素到末尾
来源：http://hz.zhixingplan.top/gtgzcnhgoe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.316326.xyz/gtzsjdyprr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.52xcode.cn/gtsaotakaf.html

JS:   arr.push(4);
来源：http://hz.aibaodan.cn/gtbtlbfgzm.html

TS:   arr.push(4);
来源：http://hz.yueranfly.top/gtzwqqlyjj.html

Java: list.add(4);
来源：http://hz.snrcjt.cn/gtemfofhep.html

Go:   arr = append(arr, 4)
来源：http://hz.hfpthk.cn/gttxcrdmov.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cashguo.top/gtturgprgk.html

C#:   list.Add(4);
来源：http://hz.dashuyun.cn/gtkqvmazao.html

[D03] 在指定位置插入元素
来源：http://hz.tian-w.cn/gtwussvaav.html

Py:   arr.insert(0, 0)
来源：http://hz.zhijiandao.cn/gtmlymabrt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sweek.top/gtxucfassx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jqgfzy.top/gteqtsgoty.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ppjwa.cn/gtqgpvwzkc.html

Java: list.add(0, 0);
来源：http://hz.quarkkingdee.top/gttpwcqnok.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhengqikj.top/gtsxlcbuxu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hammf.cn/gtfozbzvsu.html

C#:   list.Insert(0, 0);
来源：http://hz.ybcxt.top/gtzibcqhoa.html

[D04] 删除元素
来源：http://hz.jinghuilouyu.cn/gtnsixreqe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuanzx.com/gtmauwzjcp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cucudq.cn/gtlejjamxg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.0kj1m.cn/gtkttwlzfo.html

TS:   arr.splice(0, 1);
来源：http://hz.andypj.xyz/gtfrhfvqzz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangdashe.top/gtskzbrjnp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.pengpengdd.cyou/gtqxtzqhcz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangtech.top/gtxbihvmls.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.mhx1999.top/gtaavaposd.html

[D05] 访问与修改元素
来源：http://hz.yonumen.top/gtmwrcxwwd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtbvccfzip.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gaohongyu789.top/gtjdnxesuq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jianghu66.top/gtrgkuhnqm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hnxiangtu.top/gtgzdfyvik.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zdqjudy.top/gttubhcqtt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gttplaffnh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xylfe.cn/gtpnwonnfd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtnlzscfiw.html

[D06] 数组长度
来源：http://hz.yvedp.cn/gtbigyehrm.html

Py:   len(arr)
来源：http://hz.cdnleiting.top/gtkcgdvkjm.html

PHP:  count($arr);
来源：http://hz.xuanzx.com/gtwnoknada.html

JS:   arr.length
来源：http://hz.aizwys.cn/gtogtlniay.html

TS:   arr.length
来源：http://hz.meibo888.top/gtcfffejfo.html

Java: list.size();
来源：http://hz.sweek.top/gthahkouil.html

Go:   len(arr)
来源：http://hz.yangfankeji.com/gtjohpcbha.html

Ruby: arr.length; arr.size
来源：http://hz.andypj.xyz/gtporsmfpe.html

C#:   list.Count;
来源：http://hz.ppjwa.cn/gtxybjnjpg.html

[D07] 切片 / 取子数组
来源：http://hz.jlsjyb.cn/gtwchmtooa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cashguo.top/gtsuflrmtl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.guannengcc.top/gtbguhvpte.html

JS:   arr.slice(1, 4);
来源：http://hz.ybcxt.top/gtisxxphsa.html

TS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtnxfcoqpg.html

Java: list.subList(1, 4);
来源：http://hz.zhongyouzk.top/gtnpedkygm.html

Go:   arr[1:4]
来源：http://hz.cdnleiting.top/gtxxozrxex.html

Ruby: arr[1, 3]
来源：http://hz.snrcjt.cn/gtjupsqiir.html

C#:   list.GetRange(1, 3);
来源：http://hz.aizwys.cn/gtxoywbhjz.html

[D08] 合并两个数组
来源：http://hz.sweek.top/gtcupxyzja.html

Py:   a + b;  a.extend(b)
来源：http://hz.hywenlv.cn/gtxiaqkrhk.html

PHP:  array_merge($a, $b);
来源：http://hz.52xcode.cn/gtaeomnwfe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gaohongyu789.top/gtmusgimdc.html

TS:   [...a, ...b];
来源：http://hz.birdmap.top/gtjfmezrbw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hongshengwenyu.top/gtvsoparok.html

Go:   append(a, b...)
来源：http://hz.vqdsnc.cn/gtirfjprim.html

Ruby: a + b;  a.concat(b)
来源：http://hz.daria6918.cn/gtssxspazs.html

C#:   a.Concat(b).ToList()
来源：http://hz.gzhubu.top/gtvvpltvbi.html

[D09] 排序（升序）
来源：http://hz.hnxiangtu.top/gtfjvdbxxc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.quarkkingdee.top/gtflslsnew.html

PHP:  sort($arr);
来源：http://hz.shzxlz.cn/gtgofzcyka.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gzhubu.top/gtvytmjzkm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.c1oappe.top/gterxjbtft.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xuetiantiany.cn/gthtzleocz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydjk.org.cn/gtttujpopa.html

Ruby: arr.sort
来源：http://hz.tian-w.cn/gtvgpsexcm.html

C#:   list.Sort();
来源：http://hz.feifeiyinyue.top/gtcxalmobw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.fzhhl.top/gtepvkomzl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ehwqpu.com/gtfzqhmhij.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zycfv.cn/gtzjcnpgqy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nwbrower.top/gtcudjvfvy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhixingplan.top/gtyumzwnds.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yvedp.cn/gtarpqfnfp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.pengpengdd.cyou/gtyiwxtntu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj20258.top/gtqbgncnbk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jiagoushi.top/gtiaranhub.html

[D11] 反转数组
来源：http://hz.redwolf501.top/gtinezrygb.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.bjfxy.top/gtysdxaqab.html

PHP:  array_reverse($arr);
来源：http://hz.sxryk.cn/gtyhvxzoek.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yueranfly.top/gtkpsqtzxg.html

TS:   [...arr].reverse();
来源：http://hz.gotoacloud.top/gtgqjkfpzx.html

Java: Collections.reverse(list);
来源：http://hz.yongpay.top/gtspfcqioe.html

Go:   slices.Reverse(arr)
来源：http://hz.jlsjyb.cn/gteaesprca.html

Ruby: arr.reverse
来源：http://hz.snrcjt.cn/gtkenpxnjw.html

C#:   list.Reverse();
来源：http://hz.guannengcc.top/gtfljfbago.html

[D12] 查找元素下标
来源：http://hz.xuanzx.com/gtowkcednr.html

Py:   arr.index(x);  x in arr
来源：http://hz.sxryk.cn/gtgkdozkma.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xingfuxueyuan.xyz/gthwhpaadj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.andypj.xyz/gtjayekgzs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hammf.cn/gthwgsjbsw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ehwqpu.com/gtuzoijptl.html

Go:   slices.Index(arr, x)
来源：http://hz.yj20258888.top/gtuhlcjdmx.html

Ruby: arr.index(x)
来源：http://hz.hnqzz.top/gtkomvnbwd.html

C#:   list.IndexOf(x);
来源：http://hz.0kj1m.cn/gtxqxpwwmz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ywan-chungtsiang.top/gtazqwhhmm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.meibo888.top/gtblgteapx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.52xcode.cn/gtvpxebjoa.html

JS:   arr.filter(x => x > 3)
来源：http://hz.mhx1999.top/gtnzqqmooe.html

TS:   arr.filter(x => x > 3)
来源：http://hz.birdmap.top/gtlzeeqeuy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yonumen.top/gtogrsiosp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.nanxinkj.top/gtmszkcaie.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.c1oappe.top/gtltucpffp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yj20258.top/gtvhayhhrx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dashuyun.cn/gtnjomtele.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhoulong.xyz/gtdyohlidy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.wangshuangyany.cn/gtnlnhnuuw.html

JS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gthefutpgc.html

TS:   arr.map(x => x * 2)
来源：http://hz.dashuyun.cn/gtjddpmxlb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ydzc1.top/gtinyrbxzl.html

Go:   // 手写循环
来源：http://hz.redwolf501.top/gtrgstjndz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ivvv.top/gthnqwynvi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuanzhike.top/gtiywngwaa.html

[D15] 去重
来源：http://hz.nanxinkj.top/gtwnbdepuh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cashguo.top/gtppezlwpa.html

PHP:  array_unique($arr);
来源：http://hz.jinqigufen.top/gthroalgkj.html

JS:   [...new Set(arr)]
来源：http://hz.jiagoushi.top/gtqbmyrmll.html

TS:   [...new Set(arr)]
来源：http://hz.jinyuanbaomall.cn/gtnssvagwn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.meibo888.top/gtxshlvxay.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.birdmap.top/gtpcjudssm.html

Ruby: arr.uniq
来源：http://hz.cqqwz.cn/gtngyigosy.html

C#:   list.Distinct().ToList()
来源：http://hz.ppjwa.cn/gtsdflgcgf.html

[D16] 求和与平均值
来源：http://hz.smart0.xyz/gtmnemihxv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yangfankeji.com/gtefrudnjx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.andypj.xyz/gtnlzjfipm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cucudq.cn/gtluwhcwnc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yongpay.top/gtjpvuznky.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.birdmap.top/gturjeyezw.html

Go:   // 手写循环累加
来源：http://hz.sufxvd.cn/gtzzlzkvwv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydzc1.top/gtfgkernwl.html

C#:   list.Sum();  list.Average()
来源：http://hz.yangfankeji.com/gtbklihuah.html

[D17] 最大值与最小值
来源：http://hz.svipenyu.cn/gtzrakfyrp.html

Py:   max(arr);  min(arr)
来源：http://hz.ywan-chungtsiang.top/gtgcmeqdpr.html

PHP:  max($arr);  min($arr);
来源：http://hz.jianghu66.top/gtdmqdgzqj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hnxiangtu.top/gtypipthgq.html

TS:   Math.max(...arr);
来源：http://hz.ivvv.top/gtjlzmawad.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ywan-chungtsiang.top/gtrijoypsi.html


<!-- 参考信息 -->