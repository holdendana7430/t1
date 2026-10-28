代发 wailian999

================================================================================
来源：http://hz.zhixingplan.top/gtkxsaabnp.html

C. 函数与作用域
来源：http://hz.pycfn.com/gtlvgagyeg.html

================================================================================
来源：http://hz.jiagoushi.top/gtljxilayo.html

[C01] 定义函数
来源：http://hz.meibo888.top/gtvjscpamk.html

Py:   def add(a, b): return a + b
来源：http://hz.birdmap.top/gtgfiauutk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dashuyun.cn/gtiaboznwg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.birdmap.top/gtuiijijde.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.316326.xyz/gtxishqyag.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xinyue.icu/gtsazoypkf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nanxinkj.top/gtnphebuef.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sxryk.cn/gtdvrjrsud.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtaknaztpa.html

[C02] 默认参数
来源：http://hz.jiagoushi.top/gtmgfutlni.html

Py:   def greet(name="World"): return name
来源：http://hz.zhiwuduotai.top/gtgpouhfgp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.gotoacloud.top/gtgpytozgk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.wangshuangyany.cn/gtjdnnefmt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yj202588.top/gtqprwwqsw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shuidangran.top/gtlpnsjsll.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.fzhhl.top/gttqqtamtn.html

Ruby: def greet(name = "World") = name
来源：http://hz.quarkkingdee.top/gtixyosdic.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xylfe.cn/gtifecqwai.html

[C03] 可变参数
来源：http://hz.zycfv.cn/gttqcatafj.html

Py:   def total(*args): return sum(args)
来源：http://hz.svipenyu.cn/gtxeivymcc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.smart0.xyz/gtdykdtisi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jlsjyb.cn/gtfknaovol.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgfzy.top/gtlktkkqpd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.dashuyun.cn/gttrcnppzw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jyoumei.cn/gtpldlpoyk.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ivvv.top/gtybroinem.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.fzhhl.top/gttapyfqrf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuanzhike.top/gtbacuflrd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xylfe.cn/gtuodkmhyv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jqgfzy.top/gtxxdypckz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhijiandao.cn/gtpfjdovzq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.mhx1999.top/gtctknvspj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhongyouzk.top/gtbffpwdew.html

Go:   // 无：用配置结构体参数
来源：http://hz.ivvv.top/gtgmappmuq.html

Ruby: f(a: 1, b: 2)
来源：http://hz.c1oappe.top/gtbomhnhpc.html

C#:   f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtxgcnhzvz.html

[C05] 返回多个值
来源：http://hz.meibo888.top/gtpnnayzim.html

Py:   return a, b
来源：http://hz.smart0.xyz/gttgjttadp.html

PHP:  return [$a, $b];
来源：http://hz.jyoumei.cn/gtmnzewxxe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.kuanghao11.cn/gtjnfuokes.html

TS:   return { a, b };
来源：http://hz.zdqjudy.top/gtbragiuyf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj20258.top/gtmhhgnpwp.html

Go:   return a, b
来源：http://hz.iojbl.cn/gtkyjpgawb.html

Ruby: return a, b
来源：http://hz.guannengcc.top/gtqwouupdz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.chenjidiqi.icu/gtoyhfwxon.html

[C06] 匿名函数 / lambda
来源：http://hz.zhengqikj.top/gtvkshoioz.html

Py:   square = lambda x: x * x
来源：http://hz.nanxinkj.top/gteypogtix.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.nwbrower.top/gtddtcpulz.html

JS:   const square = x => x * x;
来源：http://hz.nanxuanxn.top/gtoatwjvsa.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yuanzhike.top/gtffeyuhsd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.mhx1999.top/gtfaecmoin.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.mhx1999.top/gtdiaajkrc.html

Ruby: square = ->(x) { x * x }
来源：http://hz.52xcode.cn/gtvedtvoii.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.birdmap.top/gtoyjhnaak.html

[C07] 把函数作为参数传入
来源：http://hz.0kj1m.cn/gtkglsamht.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yvedp.cn/gtrcwttnbc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zycfv.cn/gtwtbpwqhe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.havefunace.top/gtuiudhnqd.html

TS:   arr.map(String)
来源：http://hz.shzxlz.cn/gtwzreoxff.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.meibo888.top/gtshicecaa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jianghu66.top/gtccppqdsu.html

Ruby: arr.map(&:upcase)
来源：http://hz.yj202588.top/gtwecvjhqo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.daxiang520.top/gtsxppcsec.html

[C08] 闭包
来源：http://hz.yanxiufei.cn/gtmreqgpgr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gzhubu.top/gtkpwqukxm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.fengsongda.top/gtppbqutku.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.birdmap.top/gtwalghsgt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xziqi.cn/gtyovzorly.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ivvv.top/gtjxjfecoq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.guannengcc.top/gtqlotntjv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yvedp.cn/gtfamgfyfw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtqelaapjc.html

[C09] 递归
来源：http://hz.zhongyouzk.top/gtzqqsjwpl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yvedp.cn/gtpenxfdxd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.sweek.top/gtfnoktdca.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gotoacloud.top/gtwvlcsilx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuanzhike.top/gtwugrouzr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yangfankeji.com/gtjvjqwnng.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.havefunace.top/gtlqlhrddx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hnxiangtu.top/gtlshgitep.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinqigufen.top/gtiwdaosts.html

[C10] 变量作用域
来源：http://hz.cashguo.top/gtoebdcpew.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yvedp.cn/gtujddodft.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.snrcjt.cn/gtrckjbpoh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gaohongyu789.top/gtopeswzof.html

TS:   同 JS
来源：http://hz.nwbrower.top/gthstxgulo.html

Java: 方法内为块级作用域
来源：http://hz.ppjwa.cn/gtyyojfcbn.html

Go:   花括号块级作用域
来源：http://hz.zhijiandao.cn/gtvvvygeux.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ybcxt.top/gtilplwpqi.html

C#:   块级作用域
来源：http://hz.pycfn.com/gtanxjxsxc.html

[C11] 模块导入与导出
来源：http://hz.316326.xyz/gtmqjbuhxn.html

Py:   from module import func
来源：http://hz.yuxming.cn/gtvuhzekoj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xuetiantiany.cn/gtmakomkjt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.guowangkeji.top/gtyvsjujou.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jlsjyb.cn/gtcwwqkbzk.html

Java: import java.util.List;
来源：http://hz.gotoacloud.top/gtrptmheou.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sufxvd.cn/gtciifqzjh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.vqdsnc.cn/gthmpemlas.html

C#:   using System.Text;
来源：http://hz.svipenyu.cn/gtazkaadhw.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinqigufen.top/gtfjqxyybz.html

Py:   (lambda: print("run"))()
来源：http://hz.smart0.xyz/gtaubgfidp.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhongyouzk.top/gtjphmqsmi.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cdnleiting.top/gtmnfgierr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigfzy.top/gtscqnosfd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.9152youxi.cn/gtqyqzwflt.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.dashuyun.cn/gtxhmtbziq.html

Ruby: -> { puts "run" }.call
来源：http://hz.shanyushiyangtech.top/gtatvqpmbv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yonumen.top/gtsnwinlum.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhijiandao.cn/gtefhvczmk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhiwuduotai.top/gtuoqcybsj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtfcyirvwb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.fzhhl.top/gtzjlkfjjq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fengsongda.top/gteoiplher.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhixingplan.top/gtbarcrujp.html

Go:   func add(a, b int) int
来源：http://hz.jqgfzy.top/gtrtjhwkqb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hnxiangtu.top/gtlqowzqel.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenzaomai.com/gtcqawfsbh.html

[C14] 泛型函数
来源：http://hz.sufxvd.cn/gtrallcnwr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xylfe.cn/gtfdviuijq.html

PHP:  // 无泛型
来源：http://hz.chenjidiqi.icu/gtbuqziznn.html

JS:   // 无泛型
来源：http://hz.nanxuanxn.top/gtnkjzjzzr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.pengpengdd.cyou/gtskwwbfuo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.haohaochexian.top/gtyhlkuqga.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yuanzhike.top/gtdfnaqqiv.html

Ruby: # 无泛型
来源：http://hz.jiagoushi.top/gtaeekcmqc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cqqwz.cn/gteybiacso.html

[C15] 解构 / 展开参数
来源：http://hz.hfpthk.cn/gtvgsztqip.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.andypj.xyz/gtxmmrlxqq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj20258888.top/gtvxopmqtu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtdaefqvrk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.sysykeji.top/gtxhoibtrm.html

Java: // 无解构
来源：http://hz.iojbl.cn/gtvzpzdnmf.html

Go:   // 无解构
来源：http://hz.daria6918.cn/gtvdmaexld.html

Ruby: a, b = pair
来源：http://hz.tanke756.top/gtlnfjezuk.html

C#:   var (a, b) = pair;
来源：http://hz.yj202588.top/gtqdjerygf.html

[C16] 函数 / 方法重载
来源：http://hz.ydzc1.top/gtiubohniz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sxryk.cn/gtalparlup.html

PHP:  // 无重载
来源：http://hz.zhaomingkeji.xyz/gtnfohqlns.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hysaishi.cn/gtkelupqci.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.guowangkeji.top/gtnskumcpa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.smart0.xyz/gtiktdfrdt.html

Go:   // 无重载：用不同函数名
来源：http://hz.sweek.top/gtaxugswmn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xziqi.cn/gtvhphalmu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xylfe.cn/gtiyadbfcs.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtpeirsdop.html

D. 数组 / 列表 / 集合
来源：http://hz.kuanghao11.cn/gtyyjdswyn.html

================================================================================
来源：http://hz.ybcxt.top/gtrouzvong.html

[D01] 创建数组 / 列表
来源：http://hz.zhixingplan.top/gtncgiuzpq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.wangshuangyany.cn/gtspldjkte.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sweek.top/gtumjbaqqx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sufxvd.cn/gtwfikgdoz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ydzc1.top/gtshxsulvm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.tian-w.cn/gtvuyfiegb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gaohongyu789.top/gtrzafkuqt.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jyoumei.cn/gtdozxawdq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.dianchejie.cn/gtmyuhpael.html

[D02] 追加元素到末尾
来源：http://hz.sufxvd.cn/gtwknumufs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cheryme.top/gtqywaptjy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.dashuyun.cn/gtzathxand.html

JS:   arr.push(4);
来源：http://hz.shzxlz.cn/gtitcxlugh.html

TS:   arr.push(4);
来源：http://hz.ydzc1.top/gtjbmnybya.html

Java: list.add(4);
来源：http://hz.havefunace.top/gtrjcglywp.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxuanxn.top/gtpefcnlvu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yueranfly.top/gtkchxzaaf.html

C#:   list.Add(4);
来源：http://hz.hysaishi.cn/gtgabuckgl.html

[D03] 在指定位置插入元素
来源：http://hz.ehwqpu.com/gtcrvstnrs.html

Py:   arr.insert(0, 0)
来源：http://hz.nanxinkj.top/gtfooywzld.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.haohaochexian.top/gtgciejvjp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yuxming.cn/gtrgbgwzsd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hongshengwenyu.top/gtgfhrvpuw.html

Java: list.add(0, 0);
来源：http://hz.ehwqpu.com/gtixkhizob.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sysykeji.top/gtptdeykco.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.52xcode.cn/gtfwasexqq.html

C#:   list.Insert(0, 0);
来源：http://hz.tanke756.top/gtwoepxqzg.html

[D04] 删除元素
来源：http://hz.yuxming.cn/gtyfvcyvtg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yongpay.top/gtoygfyhax.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhijiandao.cn/gtarhhisge.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shanyushiyangtech.top/gtbvrprowy.html

TS:   arr.splice(0, 1);
来源：http://hz.wangdashe.top/gtawtoaaoc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.aizwys.cn/gtqyhqwjcq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.chenlongwang.top/gtvngejwbl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jyoumei.cn/gtyppeyvtf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jyoumei.cn/gtjlhuqrmf.html

[D05] 访问与修改元素
来源：http://hz.hammf.cn/gtczxgyrfj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtwkklevbz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yanxiufei.cn/gtkusrsmqa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sufxvd.cn/gtrlhnxufa.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zycfv.cn/gtsayinolh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shanyushiyangtech.top/gtiagzbmtw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gtyzyhizzq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtbdsocyxo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yuxming.cn/gtdxggomtl.html

[D06] 数组长度
来源：http://hz.sysykeji.top/gtpjyujqlv.html

Py:   len(arr)
来源：http://hz.jlsjyb.cn/gtehypsxjf.html

PHP:  count($arr);
来源：http://hz.pengpengdd.cyou/gtwmigyfza.html

JS:   arr.length
来源：http://hz.chenlongwang.top/gtgiylqrry.html

TS:   arr.length
来源：http://hz.zhoulong.xyz/gtjgdicarr.html

Java: list.size();
来源：http://hz.hnqzz.top/gtuzildkug.html

Go:   len(arr)
来源：http://hz.wangdashe.top/gtpolbjqdn.html

Ruby: arr.length; arr.size
来源：http://hz.cashguo.top/gtykbwkktg.html

C#:   list.Count;
来源：http://hz.ywan-chungtsiang.top/gtpknmamwc.html

[D07] 切片 / 取子数组
来源：http://hz.zhoulong.xyz/gtjostloqq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.redwolf501.top/gtfbvzkodu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yj20258.top/gthyasuayf.html

JS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gtyyrnzusg.html

TS:   arr.slice(1, 4);
来源：http://hz.tanke756.top/gtsliuvkdv.html

Java: list.subList(1, 4);
来源：http://hz.sufxvd.cn/gtsctoxzww.html

Go:   arr[1:4]
来源：http://hz.yonumen.top/gtiueirbdq.html

Ruby: arr[1, 3]
来源：http://hz.iojbl.cn/gtgsbbqfro.html

C#:   list.GetRange(1, 3);
来源：http://hz.daria6918.cn/gtvlxnxtxh.html

[D08] 合并两个数组
来源：http://hz.jianghu66.top/gtxozcodec.html

Py:   a + b;  a.extend(b)
来源：http://hz.tianlin.xyz/gtjmgwnqlf.html

PHP:  array_merge($a, $b);
来源：http://hz.meibo888.top/gtdjtmdxyx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xuanzx.com/gtnjhvrydg.html

TS:   [...a, ...b];
来源：http://hz.fengsongda.top/gtcbzdzscb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ehwqpu.com/gtnojehxis.html

Go:   append(a, b...)
来源：http://hz.sxryk.cn/gtkqeahcjh.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhiwuduotai.top/gtkwtqdpyl.html

C#:   a.Concat(b).ToList()
来源：http://hz.sufxvd.cn/gtufmrcfzr.html

[D09] 排序（升序）
来源：http://hz.smart0.xyz/gtqaprvzpr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shzxlz.cn/gthxzglyfr.html

PHP:  sort($arr);
来源：http://hz.chenjidiqi.icu/gtszcdjktx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhongyouzk.top/gtfwtbouxd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zycfv.cn/gttkytpnoy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hysaishi.cn/gtklmjdcjo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.aizwys.cn/gtalszdcrg.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gtbmxwjozm.html

C#:   list.Sort();
来源：http://hz.gogol.net.cn/gttcycjxaz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yvedp.cn/gthovjezgm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gotoacloud.top/gtdhkmuibp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangtech.top/gtnhqufhqq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ivvv.top/gtviyfkymo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.meibo888.top/gtpsnxpizf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgufenzy.top/gtbryjvltp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ydzc1.top/gtuscqlxfe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.dashuyun.cn/gtyieoptye.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hongshengwenyu.top/gtpffptdvk.html

[D11] 反转数组
来源：http://hz.haohaochexian.top/gtxczmqpvb.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hysaishi.cn/gtbucbeert.html

PHP:  array_reverse($arr);
来源：http://hz.tianlin.xyz/gtsoyunpgv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ivvv.top/gtkwdzmuea.html

TS:   [...arr].reverse();
来源：http://hz.jqgufenzy.top/gtdcrekvak.html

Java: Collections.reverse(list);
来源：http://hz.cqqwz.cn/gttpsexgtk.html

Go:   slices.Reverse(arr)
来源：http://hz.jyoumei.cn/gtqrrjvayw.html

Ruby: arr.reverse
来源：http://hz.sysykeji.top/gttpzthsxs.html

C#:   list.Reverse();
来源：http://hz.aibaodan.cn/gtwwqkkvzt.html

[D12] 查找元素下标
来源：http://hz.nanxuanxn.top/gtfpxbxwhh.html

Py:   arr.index(x);  x in arr
来源：http://hz.dashuyun.cn/gtycmmzyvh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shangyingyoupin.top/gtopezzyhb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gotoacloud.top/gtngpmybfi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cashguo.top/gtnxuyivrt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xylfe.cn/gtuhnbuxif.html

Go:   slices.Index(arr, x)
来源：http://hz.yuanzhike.top/gtcivwsyoz.html

Ruby: arr.index(x)
来源：http://hz.jlsjyb.cn/gtcilmjubw.html

C#:   list.IndexOf(x);
来源：http://hz.gogol.net.cn/gtjshlvtkf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhoulong.xyz/gtzeoglbbg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cucudq.cn/gtlxhyboom.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hysaishi.cn/gtarmszohm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.meibo888.top/gtowmxeecc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.316326.xyz/gtcfhohgla.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinqigufen.top/gtiedyxmiv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.dianchejie.cn/gtvyhjcoxp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cashguo.top/gthatpudex.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.0kj1m.cn/gtzuztxllp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shanyushiyangtech.top/gtcokjzerl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tianlin.xyz/gtimvdbywh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xingfuxueyuan.xyz/gtbkprhutd.html

JS:   arr.map(x => x * 2)
来源：http://hz.shuidangran.top/gtrzdhmkaf.html

TS:   arr.map(x => x * 2)
来源：http://hz.ydjk.org.cn/gtkoyaymmb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ybcxt.top/gtvusihylo.html

Go:   // 手写循环
来源：http://hz.jianghu66.top/gtgcgpigwb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yj20258888.top/gtpelqvmez.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.svipenyu.cn/gtjhofolqt.html

[D15] 去重
来源：http://hz.dashuyun.cn/gtyzxfykmj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sufxvd.cn/gtphpecmrn.html

PHP:  array_unique($arr);
来源：http://hz.jinyuanbaomall.cn/gtpvbxfvwp.html

JS:   [...new Set(arr)]
来源：http://hz.tanke756.top/gtpbhpcxto.html

TS:   [...new Set(arr)]
来源：http://hz.52xcode.cn/gtrouvuwaf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guannengcc.top/gtiqgthjzo.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jqgufenzy.top/gtqgbpaacw.html

Ruby: arr.uniq
来源：http://hz.xziqi.cn/gtchszdkjm.html

C#:   list.Distinct().ToList()
来源：http://hz.tianlin.xyz/gtrupncgjf.html

[D16] 求和与平均值
来源：http://hz.yangfankeji.com/gteyfwffdn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.meibo888.top/gtdgmyrniv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fzhhl.top/gtewubjvah.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.birdmap.top/gttnzruvdi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yueranfly.top/gthphxupbv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sxryk.cn/gtvjdmqnpi.html

Go:   // 手写循环累加
来源：http://hz.zycfv.cn/gtnbvloqqg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xziqi.cn/gtbmomhibc.html

C#:   list.Sum();  list.Average()
来源：http://hz.ybcxt.top/gtpldivnaf.html

[D17] 最大值与最小值
来源：http://hz.tian-w.cn/gteyhonetm.html

Py:   max(arr);  min(arr)
来源：http://hz.jinghuilouyu.cn/gthxooffhd.html

PHP:  max($arr);  min($arr);
来源：http://hz.iojbl.cn/gtjmbsyzgw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.fengsongda.top/gtvzpcmyot.html

TS:   Math.max(...arr);
来源：http://hz.zhijiandao.cn/gtsxkbclbs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hysaishi.cn/gtkusknjmf.html


<!-- 参考信息 -->