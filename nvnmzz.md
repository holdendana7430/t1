代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.guowangkeji.top/gtaypbjlfg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.nanxuanxn.top/gtbabeidly.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.daxiang520.top/gtttiglzcy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.tianlin.xyz/gtliznhgka.html

Go:   // 无：用配置结构体参数
来源：http://hz.yj20258.top/gtrhriiybu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shanyushiyangkeji.top/gtxukohsfg.html

C#:   f(a: 1, b: 2)
来源：http://hz.quarkkingdee.top/gtocphotbc.html

[C05] 返回多个值
来源：http://hz.smart0.xyz/gttrtjgfwk.html

Py:   return a, b
来源：http://hz.yanxiufei.cn/gtjscvyslb.html

PHP:  return [$a, $b];
来源：http://hz.yuanzhike.top/gtyuiaandt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cucudq.cn/gtestjzcby.html

TS:   return { a, b };
来源：http://hz.sysykeji.top/gtdsymbuuf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.daria6918.cn/gtyvftuuxr.html

Go:   return a, b
来源：http://hz.shuidangran.top/gtdyoemncw.html

Ruby: return a, b
来源：http://hz.jlsjyb.cn/gtsqespvws.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhijiandao.cn/gtrrvdemqa.html

[C06] 匿名函数 / lambda
来源：http://hz.zhiwuduotai.top/gtrzeiwzpf.html

Py:   square = lambda x: x * x
来源：http://hz.andypj.xyz/gtljxtcazf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.c1oappe.top/gtltcnqqxo.html

JS:   const square = x => x * x;
来源：http://hz.sufxvd.cn/gtjfshmgxh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yuanzhike.top/gtqyaeuwtm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yangfankeji.com/gtzqnqwqka.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.chenzaomai.com/gtqriucjtu.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yueranfly.top/gtcyaqddkp.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.dashuyun.cn/gtqmwheknu.html

[C07] 把函数作为参数传入
来源：http://hz.pycfn.com/gtxvampbny.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yueranfly.top/gtealmlkaa.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ybcxt.top/gtmefgflec.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hfpthk.cn/gtmhyotccj.html

TS:   arr.map(String)
来源：http://hz.zhoulong.xyz/gtdgbykwkm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ydzc1.top/gttwmxjntu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ybcxt.top/gtiqpmjmpb.html

Ruby: arr.map(&:upcase)
来源：http://hz.chenlongwang.top/gtoveilrxx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.birdmap.top/gtvvlbvivz.html

[C08] 闭包
来源：http://hz.chenjidiqi.icu/gtckavrhul.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.snrcjt.cn/gtlfnlilfn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.dianchejie.cn/gtngzwyhpj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtjhskhuzo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.nanxuanxn.top/gtbqgklwcb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hysaishi.cn/gtdxnfxdrf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gzhubu.top/gtiluhqknm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sysykeji.top/gtojufhzhy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtftgtcden.html

[C09] 递归
来源：http://hz.aizwys.cn/gtptkpigzq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ehwqpu.com/gtexxawiwj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.daxiang520.top/gtzbgrnyre.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxinkj.top/gtrrjatxjv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hongshengwenyu.top/gtpyqacpct.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenlongwang.top/gtzfqilgwg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.aibaodan.cn/gtmfkefzed.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.birdmap.top/gtgtvyfxwp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yj20258.top/gtwdwbgdgs.html

[C10] 变量作用域
来源：http://hz.hfpthk.cn/gtvfmlojhg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shanyushiyangtech.top/gtwbsbyeeg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.c1oappe.top/gtqcbocgjs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhijiandao.cn/gtxlpgpadq.html

TS:   同 JS
来源：http://hz.haohaochexian.top/gttugkmnyk.html

Java: 方法内为块级作用域
来源：http://hz.iojbl.cn/gteuzqcvfu.html

Go:   花括号块级作用域
来源：http://hz.yvedp.cn/gtqtzhxrfr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ywan-chungtsiang.top/gtssjzkbch.html

C#:   块级作用域
来源：http://hz.yuanzhike.top/gtszqxgkya.html

[C11] 模块导入与导出
来源：http://hz.zhengqikj.top/gtnvsvtitc.html

Py:   from module import func
来源：http://hz.jiagoushi.top/gthkveinmv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hnxiangtu.top/gtrxsxlaax.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinghuilouyu.cn/gtbimqznis.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhongyouzk.top/gtjuznrteg.html

Java: import java.util.List;
来源：http://hz.gzhubu.top/gtmyfcvbbr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jiagoushi.top/gtgmyrllkn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhijiandao.cn/gtbuigqjrq.html

C#:   using System.Text;
来源：http://hz.chenzaomai.com/gtefozexnb.html

[C12] 立即执行函数 IIFE
来源：http://hz.guowangkeji.top/gtmakjvzcx.html

Py:   (lambda: print("run"))()
来源：http://hz.zhongyouzk.top/gtndoyzddi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.gaohongyu789.top/gtekevsulb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.pengpengdd.cyou/gtuauwegnl.html

TS:   (() => { console.log("run"); })();
来源：http://hz.pycfn.com/gtvcgqmgsy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.svipenyu.cn/gtwyuhnnfl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xuanzx.com/gthylaanid.html

Ruby: -> { puts "run" }.call
来源：http://hz.redwolf501.top/gtftzeodsf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hysaishi.cn/gtxwfqwmde.html

[C13] 类型声明 / 类型注解
来源：http://hz.0kj1m.cn/gttxzbecvm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jyoumei.cn/gtjbkbrcom.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinyuanbaomall.cn/gtqkbifwrj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shanyushiyangkeji.top/gtlruggxyn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guannengcc.top/gtanvzrhgz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtvhzztsse.html

Go:   func add(a, b int) int
来源：http://hz.vqdsnc.cn/gtklowidbd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shangyingyoupin.top/gtvbmulhyc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ydjk.org.cn/gtkiqvaeiq.html

[C14] 泛型函数
来源：http://hz.zycfv.cn/gtjmozmted.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gttdsxxgxe.html

PHP:  // 无泛型
来源：http://hz.sweek.top/gtpvvxsaow.html

JS:   // 无泛型
来源：http://hz.c1oappe.top/gtajbqtlka.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shanyushiyangkeji.top/gtyvuoxkwj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.vqdsnc.cn/gtfilvqwiq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sysykeji.top/gtqpkehjbg.html

Ruby: # 无泛型
来源：http://hz.chenzaomai.com/gtyibvlzis.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shangyingyoupin.top/gtmannubgr.html

[C15] 解构 / 展开参数
来源：http://hz.ybcxt.top/gtvwheaask.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.316326.xyz/gtejnbvqbn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jinyuanbaomall.cn/gtpfmtvtna.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ybcxt.top/gtjznlfvvs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.svipenyu.cn/gtmskyefzk.html

Java: // 无解构
来源：http://hz.tianlin.xyz/gtvkoksgyu.html

Go:   // 无解构
来源：http://hz.meibo888.top/gtfmfpllhk.html

Ruby: a, b = pair
来源：http://hz.sysykeji.top/gtgpfocjje.html

C#:   var (a, b) = pair;
来源：http://hz.jiagoushi.top/gtoikoxiyt.html

[C16] 函数 / 方法重载
来源：http://hz.shanyushiyangkeji.top/gtgbcpsxwm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.birdmap.top/gtobwzlwua.html

PHP:  // 无重载
来源：http://hz.tanke756.top/gtvzxeqzeo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.9152youxi.cn/gtrhggamew.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xuanzx.com/gtdvtlmsio.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tanke756.top/gtwmitzboj.html

Go:   // 无重载：用不同函数名
来源：http://hz.snrcjt.cn/gtaffovjhr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.smart0.xyz/gtosbmizyy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yvedp.cn/gtxkvahqwl.html

================================================================================
来源：http://hz.52xcode.cn/gtrhucgbyt.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258888.top/gtopjaobmh.html

================================================================================
来源：http://hz.wangdashe.top/gtjsxthrix.html

[D01] 创建数组 / 列表
来源：http://hz.chenzaomai.com/gtogqtqgxz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ppjwa.cn/gtenhzefew.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guowangkeji.top/gtkdyubdbf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj20258.top/gtxksxawpv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hfpthk.cn/gtexsckmam.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.birdmap.top/gtsowzfmzz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yueranfly.top/gtfdkqzpdu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yongpay.top/gthymxtsyi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ybcxt.top/gtejlwxjer.html

[D02] 追加元素到末尾
来源：http://hz.jinqigfzy.top/gtkqnaeuec.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.vqdsnc.cn/gtgpjwqudj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.dianchejie.cn/gtbursncoi.html

JS:   arr.push(4);
来源：http://hz.zdqjudy.top/gtfhqyoblb.html

TS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gthanltobh.html

Java: list.add(4);
来源：http://hz.bjfxy.top/gtfvxfbqga.html

Go:   arr = append(arr, 4)
来源：http://hz.birdmap.top/gtfrnnedsl.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tian-w.cn/gtbxcipszj.html

C#:   list.Add(4);
来源：http://hz.svipenyu.cn/gtaqcdqmtt.html

[D03] 在指定位置插入元素
来源：http://hz.shanyushiyangtech.top/gtogwfpqyy.html

Py:   arr.insert(0, 0)
来源：http://hz.jqgfzy.top/gtkkxewfzi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sysykeji.top/gthbxztxen.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.andypj.xyz/gtecoymfjj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.feifeiyinyue.top/gtsackflbz.html

Java: list.add(0, 0);
来源：http://hz.ehwqpu.com/gtcybaisoy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shangyingyoupin.top/gttylzffjm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shzxlz.cn/gtmuywxiht.html

C#:   list.Insert(0, 0);
来源：http://hz.shanyushiyangtech.top/gtyzkkvvun.html

[D04] 删除元素
来源：http://hz.jinghuilouyu.cn/gttnvnmall.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinghuilouyu.cn/gtkyekplqw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.havefunace.top/gttyrqdnpl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xylfe.cn/gtcopiaelw.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigufen.top/gtrtcipiya.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.guowangkeji.top/gtifkajfrg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jianghu66.top/gtskxmvnmk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.pycfn.com/gtlobzuzhv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yvedp.cn/gtekqwsood.html

[D05] 访问与修改元素
来源：http://hz.mhx1999.top/gtzstzkpfs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtjhiurmgy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jqgfzy.top/gtqfryomvd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.chenlongwang.top/gtkyyvgckh.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gotoacloud.top/gtdaondwms.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tanke756.top/gtrwnwzztz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gtbbxdruhp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gtblafffwi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zdqjudy.top/gtalwnunds.html

[D06] 数组长度
来源：http://hz.ehwqpu.com/gtzqlrigsf.html

Py:   len(arr)
来源：http://hz.aizwys.cn/gtarywbnhj.html

PHP:  count($arr);
来源：http://hz.yanxiufei.cn/gttzixuxhb.html

JS:   arr.length
来源：http://hz.yj202588.top/gtznithueo.html

TS:   arr.length
来源：http://hz.hfpthk.cn/gtbhfahcpr.html

Java: list.size();
来源：http://hz.feifeiyinyue.top/gtrcwxqmfs.html

Go:   len(arr)
来源：http://hz.316326.xyz/gtbzkanyoa.html

Ruby: arr.length; arr.size
来源：http://hz.andypj.xyz/gtdorjqqfg.html

C#:   list.Count;
来源：http://hz.fzhhl.top/gtmczjvvub.html

[D07] 切片 / 取子数组
来源：http://hz.yj20258888.top/gteqyhazzs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.havefunace.top/gtilagiihi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jianghu66.top/gtbjwwmtad.html

JS:   arr.slice(1, 4);
来源：http://hz.hfpthk.cn/gtpdwwokgg.html

TS:   arr.slice(1, 4);
来源：http://hz.yangfankeji.com/gtwhzyazas.html

Java: list.subList(1, 4);
来源：http://hz.xuanzx.com/gtcgzylvvu.html

Go:   arr[1:4]
来源：http://hz.yj20258888.top/gtyradhvwn.html

Ruby: arr[1, 3]
来源：http://hz.0kj1m.cn/gtqxrgcfho.html

C#:   list.GetRange(1, 3);
来源：http://hz.sufxvd.cn/gtgztatdzj.html

[D08] 合并两个数组
来源：http://hz.jinyuanbaomall.cn/gtcixmjahc.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj202588.top/gtshacpadz.html

PHP:  array_merge($a, $b);
来源：http://hz.0kj1m.cn/gtwpwhjbkr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xuetiantiany.cn/gtfznrgusc.html

TS:   [...a, ...b];
来源：http://hz.gzhubu.top/gtyvhnsepf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hnqzz.top/gtzqteyqvv.html

Go:   append(a, b...)
来源：http://hz.mhx1999.top/gtmbnluqoi.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj202588.top/gtxdjiljof.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenlongwang.top/gtifoefsmg.html

[D09] 排序（升序）
来源：http://hz.chenjidiqi.icu/gtfdcuvije.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.316326.xyz/gtyoaeyzcu.html

PHP:  sort($arr);
来源：http://hz.quarkkingdee.top/gthwfawjzy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj20258888.top/gtcgqeszcw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ppjwa.cn/gtmjgulniz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shangyingyoupin.top/gtqifjmhuy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jyoumei.cn/gtyrgzdiiz.html

Ruby: arr.sort
来源：http://hz.feifeiyinyue.top/gtehhfbvqk.html

C#:   list.Sort();
来源：http://hz.zhongyouzk.top/gtpagdhlfw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shanyushiyangtech.top/gtvucqqoot.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhijiandao.cn/gtgrxxbrbi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.smart0.xyz/gtjqquqjmn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sxryk.cn/gtjnoufjfz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hongshengwenyu.top/gtlinmemyh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sysykeji.top/gtgcagzsas.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ehwqpu.com/gtvyjmoaho.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ybcxt.top/gtzfkssdrt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.wangshuangyany.cn/gtgygxoawp.html

[D11] 反转数组
来源：http://hz.nanxinkj.top/gtmvblggen.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ydjk.org.cn/gtjjxombch.html

PHP:  array_reverse($arr);
来源：http://hz.redwolf501.top/gtopqppdpm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhengqikj.top/gtohpwnmoj.html

TS:   [...arr].reverse();
来源：http://hz.haohaochexian.top/gtrycxrdiy.html

Java: Collections.reverse(list);
来源：http://hz.sufxvd.cn/gtjqmpphoc.html

Go:   slices.Reverse(arr)
来源：http://hz.gaohongyu789.top/gtkthjorth.html

Ruby: arr.reverse
来源：http://hz.yvedp.cn/gtwpczzzbm.html

C#:   list.Reverse();
来源：http://hz.xziqi.cn/gtkvjqfcbt.html

[D12] 查找元素下标
来源：http://hz.gotoacloud.top/gtltisxdfw.html

Py:   arr.index(x);  x in arr
来源：http://hz.nwbrower.top/gthdkgvphq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhongyouzk.top/gtlecmwulr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tanke756.top/gtrnjngipj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tanke756.top/gtixhwrdep.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xziqi.cn/gtqbazupcb.html

Go:   slices.Index(arr, x)
来源：http://hz.zdqjudy.top/gttlhptltq.html

Ruby: arr.index(x)
来源：http://hz.ydjk.org.cn/gtbvwzkptd.html

C#:   list.IndexOf(x);
来源：http://hz.havefunace.top/gtvsjubyhw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yueranfly.top/gtyvdzwtlt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ivvv.top/gtzpgtyksv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhijiandao.cn/gtkgjqryge.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yanxiufei.cn/gtobcwycza.html

TS:   arr.filter(x => x > 3)
来源：http://hz.dianchejie.cn/gtkqrgnnka.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.mhx1999.top/gtoztbmxsy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xylfe.cn/gtkruxtloa.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yj202588.top/gtzmdnccaw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.quarkkingdee.top/gtnwlazjos.html

[D14] 映射转换（每个元素变形）
来源：http://hz.quarkkingdee.top/gtrvmfnlxw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.redwolf501.top/gtnceermkh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hongshengwenyu.top/gtgvhihoii.html

JS:   arr.map(x => x * 2)
来源：http://hz.sweek.top/gtrlzbzhxi.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinqigfzy.top/gtmimxktln.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cdnleiting.top/gttmbitqwz.html

Go:   // 手写循环
来源：http://hz.cqqwz.cn/gtudfcqwjf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sxryk.cn/gtytrnhcqe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.52xcode.cn/gtcoqgfcms.html

[D15] 去重
来源：http://hz.cheryme.top/gtrjkaqxmt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gtkhujdylw.html

PHP:  array_unique($arr);
来源：http://hz.jlsjyb.cn/gtslpneita.html

JS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gtrjscmadg.html

TS:   [...new Set(arr)]
来源：http://hz.yuxming.cn/gtroivioli.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.tian-w.cn/gtqxsqnbci.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.havefunace.top/gtveksbyfj.html

Ruby: arr.uniq
来源：http://hz.yvedp.cn/gtdqotwtaj.html

C#:   list.Distinct().ToList()
来源：http://hz.cucudq.cn/gtojlvcjaw.html

[D16] 求和与平均值
来源：http://hz.ppjwa.cn/gtugkxiopx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhaomingkeji.xyz/gtfqhmwhhs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jianghu66.top/gtuhaievei.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nwbrower.top/gtofotqxhh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangdashe.top/gtyaggxtap.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jiagoushi.top/gtdqqiaxsv.html

Go:   // 手写循环累加
来源：http://hz.jqgfzy.top/gtvaaensqf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.kuanghao11.cn/gtumsogggn.html

C#:   list.Sum();  list.Average()
来源：http://hz.fengsongda.top/gtaotfpdam.html

[D17] 最大值与最小值
来源：http://hz.ehwqpu.com/gtxlvamydt.html

Py:   max(arr);  min(arr)
来源：http://hz.jlsjyb.cn/gtjswtxzzr.html

PHP:  max($arr);  min($arr);
来源：http://hz.svipenyu.cn/gtisajxnhn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hysaishi.cn/gtqvwavivy.html

TS:   Math.max(...arr);
来源：http://hz.gaohongyu789.top/gtjcrjtvgl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.vqdsnc.cn/gtwrlquhds.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.haohaochexian.top/gtoicbcmfx.html

Ruby: arr.max;  arr.min
来源：http://hz.feifeiyinyue.top/gtrgjjvrrz.html

C#:   list.Max();  list.Min()
来源：http://hz.pycfn.com/gtvpilaxfk.html

[D18] 扁平化嵌套数组
来源：http://hz.andypj.xyz/gtyreppyte.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.aibaodan.cn/gtfgqslxln.html

PHP:  array_merge(...$nested);
来源：http://hz.wangdashe.top/gtuictvwip.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guannengcc.top/gtrlyjhglw.html

TS:   nested.flat();
来源：http://hz.chenlongwang.top/gttwryhehb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zycfv.cn/gtgaeaejka.html

Go:   // 手写双层循环
来源：http://hz.zhengqikj.top/gtwtbtoxyl.html

Ruby: nested.flatten
来源：http://hz.ivvv.top/gtonwzsojx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hnqzz.top/gtolhnmxlk.html

[D19] 按字段分组
来源：http://hz.hnxiangtu.top/gtgzdafqbf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.redwolf501.top/gtikgbryob.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yangfankeji.com/gtjeajzcpc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shangyingyoupin.top/gttkbfwebs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gotoacloud.top/gtqiapjzsb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dashuyun.cn/gtaburiaxi.html

Go:   // 手写 map[string][]T
来源：http://hz.dashuyun.cn/gtdomaedka.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shanyushiyangtech.top/gtqtbakgbx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yongpay.top/gtbokpluha.html

[D20] 统计每个元素出现次数
来源：http://hz.0kj1m.cn/gtietkhfwu.html

Py:   Counter(arr)
来源：http://hz.chenjidiqi.icu/gtufxsqnwm.html

PHP:  array_count_values($arr);
来源：http://hz.haohaochexian.top/gtcacojvtr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtefoofrti.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhaomingkeji.xyz/gthzlnlobo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhoulong.xyz/gtvwgawlxk.html

Go:   // 手写 map[T]int
来源：http://hz.chenjidiqi.icu/gtrnyyfppt.html

Ruby: arr.tally
来源：http://hz.xuanzx.com/gtmjiwijvd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.guannengcc.top/gtzplcsovr.html

[D21] 判断是否包含某元素
来源：http://hz.cheryme.top/gtnvhjomcx.html

Py:   x in arr
来源：http://hz.hfpthk.cn/gtwblktfeq.html


<!-- 参考信息 -->