代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.mhx1999.top/gtpbchvvrj.html

Go:   return a, b
来源：http://hz.fzhhl.top/gtqolpnkkg.html

Ruby: return a, b
来源：http://hz.ywan-chungtsiang.top/gthfyblqkv.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.pycfn.com/gtzekmylwh.html

[C06] 匿名函数 / lambda
来源：http://hz.ywan-chungtsiang.top/gtzxcicsax.html

Py:   square = lambda x: x * x
来源：http://hz.hysaishi.cn/gtulknwwsn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jiagoushi.top/gtnvayxmzc.html

JS:   const square = x => x * x;
来源：http://hz.xinyue.icu/gtuqutzxnk.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yvedp.cn/gtnecgckkt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gotoacloud.top/gtbubydcfm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gotoacloud.top/gtrponddmv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.9152youxi.cn/gtwndywddf.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hammf.cn/gtgadzsnqh.html

[C07] 把函数作为参数传入
来源：http://hz.hammf.cn/gtjniulxhi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.birdmap.top/gtjpobrfha.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xuetiantiany.cn/gtujfpuqiy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.52xcode.cn/gtmctagjpk.html

TS:   arr.map(String)
来源：http://hz.shuidangran.top/gtusfybtpj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.sxryk.cn/gtqppgkrfj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.svipenyu.cn/gtthaqngya.html

Ruby: arr.map(&:upcase)
来源：http://hz.meibo888.top/gttrvhvjlt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xylfe.cn/gtghgvuyni.html

[C08] 闭包
来源：http://hz.havefunace.top/gtnksrbeud.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.andypj.xyz/gtxnggpcri.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.chenzaomai.com/gtyeukfnll.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tianlin.xyz/gtiegjtocf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gtpkuewmpa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.tian-w.cn/gtldcudadv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.0kj1m.cn/gtkmxlkrax.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yvedp.cn/gtgshhgobx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gtvhrelqdx.html

[C09] 递归
来源：http://hz.ybcxt.top/gtmimovhuq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.fzhhl.top/gtrpxmwyos.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yvedp.cn/gtskjbhtiz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jlsjyb.cn/gtpzyfnnfv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yueranfly.top/gtrkexwida.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yongpay.top/gtyrnmmnkd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shangyingyoupin.top/gtdvimdvmy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhengqikj.top/gtqugezqgl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.svipenyu.cn/gtistruqsx.html

[C10] 变量作用域
来源：http://hz.c1oappe.top/gtgbttyxpj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shzxlz.cn/gtogwxbigd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.dianchejie.cn/gtkdjsmvqf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhixingplan.top/gtyllmtsgp.html

TS:   同 JS
来源：http://hz.dashuyun.cn/gtbfovyyhi.html

Java: 方法内为块级作用域
来源：http://hz.gogol.net.cn/gtllbhriib.html

Go:   花括号块级作用域
来源：http://hz.zhiwuduotai.top/gtrsyginrw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.feifeiyinyue.top/gtalsbjesf.html

C#:   块级作用域
来源：http://hz.ybcxt.top/gtfsnzdbfo.html

[C11] 模块导入与导出
来源：http://hz.chenjidiqi.icu/gtwjuhyqsp.html

Py:   from module import func
来源：http://hz.ppjwa.cn/gtjuzdcdwl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shuidangran.top/gtlwowvtoy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hysaishi.cn/gtncqfvnnz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tianlin.xyz/gtiwicglwi.html

Java: import java.util.List;
来源：http://hz.aibaodan.cn/gtggducpgx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.daxiang520.top/gtcqmfnmze.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daxiang520.top/gtexlpdbsj.html

C#:   using System.Text;
来源：http://hz.guowangkeji.top/gtwigkhylh.html

[C12] 立即执行函数 IIFE
来源：http://hz.jqgfzy.top/gtjypdoyzu.html

Py:   (lambda: print("run"))()
来源：http://hz.vqdsnc.cn/gtknjfwwik.html

PHP:  (function () { echo "run"; })();
来源：http://hz.fzhhl.top/gtuafamwmo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cucudq.cn/gtqyizqjze.html

TS:   (() => { console.log("run"); })();
来源：http://hz.redwolf501.top/gtyoroiyco.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hammf.cn/gtxtponfer.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.havefunace.top/gtsdzwdhby.html

Ruby: -> { puts "run" }.call
来源：http://hz.dashuyun.cn/gtmfojcons.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xziqi.cn/gtmnzvgqzm.html

[C13] 类型声明 / 类型注解
来源：http://hz.yuxming.cn/gtyfmafovk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.bjfxy.top/gtwnnorjin.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cdnleiting.top/gtpznbhypw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ywan-chungtsiang.top/gtrbvuhyfu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shuidangran.top/gtdcjhhocc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhijiandao.cn/gtizpticpw.html

Go:   func add(a, b int) int
来源：http://hz.cqqwz.cn/gtgwmsimbv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gzhubu.top/gtoguxkmjp.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenlongwang.top/gtvaajnnut.html

[C14] 泛型函数
来源：http://hz.fzhhl.top/gtpbdyfayu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.bjfxy.top/gtgcrczuec.html

PHP:  // 无泛型
来源：http://hz.sweek.top/gtxsodxate.html

JS:   // 无泛型
来源：http://hz.316326.xyz/gtsfaasphx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.meibo888.top/gtcnguwqog.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.birdmap.top/gtzdzpyomg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.aizwys.cn/gtwhdhhuik.html

Ruby: # 无泛型
来源：http://hz.snrcjt.cn/gtdpucuuum.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sxryk.cn/gtzfguureq.html

[C15] 解构 / 展开参数
来源：http://hz.jinyuanbaomall.cn/gtwdtrcrwi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.birdmap.top/gtjrftrktp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nwbrower.top/gtwkoqbwkr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.iojbl.cn/gtryvlnmtb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.bjfxy.top/gtwofhljsa.html

Java: // 无解构
来源：http://hz.iojbl.cn/gttesoumrq.html

Go:   // 无解构
来源：http://hz.ehwqpu.com/gtmtnvcjvo.html

Ruby: a, b = pair
来源：http://hz.birdmap.top/gtkpkgzdor.html

C#:   var (a, b) = pair;
来源：http://hz.chenzaomai.com/gtnobhtqnv.html

[C16] 函数 / 方法重载
来源：http://hz.jqgufenzy.top/gtuyypcxyg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hammf.cn/gtmmzslwrp.html

PHP:  // 无重载
来源：http://hz.zhijiandao.cn/gtjfvspgmo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hfpthk.cn/gtlyzaingx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cdnleiting.top/gtrlmeitja.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xinyue.icu/gtlgsvbpja.html

Go:   // 无重载：用不同函数名
来源：http://hz.hfpthk.cn/gtdqhsxmfg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.52xcode.cn/gtkslkuqls.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinqigfzy.top/gtpersvcxt.html

================================================================================
来源：http://hz.ehwqpu.com/gttwqttvpt.html

D. 数组 / 列表 / 集合
来源：http://hz.guannengcc.top/gtjxvlndif.html

================================================================================
来源：http://hz.jinqigufen.top/gtwpwtphdc.html

[D01] 创建数组 / 列表
来源：http://hz.aizwys.cn/gtszcpcblg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.fzhhl.top/gtmwsosoaz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yj20258.top/gtpwdxihfp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.snrcjt.cn/gtrkxgylzk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhiwuduotai.top/gtjkwaiyag.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.316326.xyz/gtikrdhzvb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.nwbrower.top/gtguyoymuo.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cheryme.top/gtzrmhrmww.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenlongwang.top/gtsuifactq.html

[D02] 追加元素到末尾
来源：http://hz.xuanzx.com/gtuumbhyml.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.iojbl.cn/gtaqrtokpm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hysaishi.cn/gtdcbxtygn.html

JS:   arr.push(4);
来源：http://hz.zhijiandao.cn/gtiqlmlybc.html

TS:   arr.push(4);
来源：http://hz.zhoulong.xyz/gtccdeqtmy.html

Java: list.add(4);
来源：http://hz.yanxiufei.cn/gtweoxsrbz.html

Go:   arr = append(arr, 4)
来源：http://hz.bjfxy.top/gtyjzcpayn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.pengpengdd.cyou/gtuoqgiwok.html

C#:   list.Add(4);
来源：http://hz.gzhubu.top/gtucbhiqdd.html

[D03] 在指定位置插入元素
来源：http://hz.hysaishi.cn/gtypsemafh.html

Py:   arr.insert(0, 0)
来源：http://hz.wangdashe.top/gtwtdhimzm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.iojbl.cn/gtkzmyirmu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.andypj.xyz/gtrgjatybh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yanxiufei.cn/gtphamlssd.html

Java: list.add(0, 0);
来源：http://hz.zhiwuduotai.top/gtikttnfjq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.52xcode.cn/gtpwnovwdj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cashguo.top/gtlkitsuej.html

C#:   list.Insert(0, 0);
来源：http://hz.haohaochexian.top/gtfgvrpiwz.html

[D04] 删除元素
来源：http://hz.yj20258888.top/gtrmumyvpe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gotoacloud.top/gtwisyettc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.aibaodan.cn/gtdjwiqwdk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xinyue.icu/gtmbvmdykz.html

TS:   arr.splice(0, 1);
来源：http://hz.jqgufenzy.top/gtyrnapxqy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yueranfly.top/gtxljvjknr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yangfankeji.com/gtdbaykbvd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yj20258.top/gtfdmtjzft.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xingfuxueyuan.xyz/gtjwobkcso.html

[D05] 访问与修改元素
来源：http://hz.xylfe.cn/gtpovmwqpg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gthhswpsdb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cdnleiting.top/gtmnlkfqzm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ydjk.org.cn/gtdihcgbmh.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yueranfly.top/gtitdpleka.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhixingplan.top/gtpeyegdqz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtcviaurgi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.redwolf501.top/gtrpwtoxuj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zycfv.cn/gtzscgiapr.html

[D06] 数组长度
来源：http://hz.yuanzhike.top/gtzpshaavv.html

Py:   len(arr)
来源：http://hz.sweek.top/gtlinyhfgp.html

PHP:  count($arr);
来源：http://hz.zhongyouzk.top/gtifucslqm.html

JS:   arr.length
来源：http://hz.yj20258888.top/gtsvwxzatg.html

TS:   arr.length
来源：http://hz.ppjwa.cn/gtlykzsvlr.html

Java: list.size();
来源：http://hz.smart0.xyz/gtqljdszrr.html

Go:   len(arr)
来源：http://hz.sysykeji.top/gtmoocpipr.html

Ruby: arr.length; arr.size
来源：http://hz.aibaodan.cn/gtnqbvqjad.html

C#:   list.Count;
来源：http://hz.jqgufenzy.top/gtzuxuwbec.html

[D07] 切片 / 取子数组
来源：http://hz.ybcxt.top/gtsounnjlz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xuetiantiany.cn/gtaiyosctp.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.iojbl.cn/gtekmgafyz.html

JS:   arr.slice(1, 4);
来源：http://hz.feifeiyinyue.top/gtcfibdyje.html

TS:   arr.slice(1, 4);
来源：http://hz.wangshuangyany.cn/gtlpgpghzu.html

Java: list.subList(1, 4);
来源：http://hz.jqgfzy.top/gtdppdgrwc.html

Go:   arr[1:4]
来源：http://hz.yonumen.top/gtwscopacz.html

Ruby: arr[1, 3]
来源：http://hz.52xcode.cn/gtskbkpldm.html

C#:   list.GetRange(1, 3);
来源：http://hz.yongpay.top/gtakrpmkva.html

[D08] 合并两个数组
来源：http://hz.ivvv.top/gtzrolseei.html

Py:   a + b;  a.extend(b)
来源：http://hz.tian-w.cn/gtjriwgvxx.html

PHP:  array_merge($a, $b);
来源：http://hz.tian-w.cn/gtmlgllhcr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.chenzaomai.com/gtlxdfvwtc.html

TS:   [...a, ...b];
来源：http://hz.shzxlz.cn/gtpummlcax.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangtech.top/gtffeebzhf.html

Go:   append(a, b...)
来源：http://hz.birdmap.top/gtkqpswwcx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sufxvd.cn/gtjsnpdbgs.html

C#:   a.Concat(b).ToList()
来源：http://hz.fengsongda.top/gtrmcndkyd.html

[D09] 排序（升序）
来源：http://hz.cashguo.top/gtmzkzksmg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pycfn.com/gtgycduvjx.html

PHP:  sort($arr);
来源：http://hz.zhengqikj.top/gtktydrlxp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj20258.top/gtpvelyxfw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sysykeji.top/gtimolwntl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xuanzx.com/gtpitstexs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.svipenyu.cn/gtzssvodxl.html

Ruby: arr.sort
来源：http://hz.andypj.xyz/gtdaunjzha.html

C#:   list.Sort();
来源：http://hz.ybcxt.top/gtqtlrbutz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gotoacloud.top/gtyjchlvix.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.pengpengdd.cyou/gteilbdeoi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuanzhike.top/gtfihiwxlh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.havefunace.top/gtyyhboyov.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gtkpgrosbl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.fzhhl.top/gtbufvrwld.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sysykeji.top/gttwkptrop.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shanyushiyangkeji.top/gtheeadrhs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhongyouzk.top/gtkzqrzzyc.html

[D11] 反转数组
来源：http://hz.yueranfly.top/gtvemhfvwp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shuidangran.top/gtkbvwoqpt.html

PHP:  array_reverse($arr);
来源：http://hz.hnqzz.top/gtnximktlv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ybcxt.top/gtsjicgclf.html

TS:   [...arr].reverse();
来源：http://hz.smart0.xyz/gtnvxymfmw.html

Java: Collections.reverse(list);
来源：http://hz.sweek.top/gtjqkahjhk.html

Go:   slices.Reverse(arr)
来源：http://hz.yuanzhike.top/gtgcrrsrua.html

Ruby: arr.reverse
来源：http://hz.guannengcc.top/gtpawjbtdu.html

C#:   list.Reverse();
来源：http://hz.xziqi.cn/gtkcpecnrm.html

[D12] 查找元素下标
来源：http://hz.xinyue.icu/gtzljxsbbf.html

Py:   arr.index(x);  x in arr
来源：http://hz.pengpengdd.cyou/gtojiqulom.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gotoacloud.top/gtwitujetp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuanzhike.top/gtyebicjvk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigufen.top/gtyontmrqy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.guannengcc.top/gtjpbjefva.html

Go:   slices.Index(arr, x)
来源：http://hz.birdmap.top/gtmzlgncni.html

Ruby: arr.index(x)
来源：http://hz.guowangkeji.top/gtgrlnwqra.html

C#:   list.IndexOf(x);
来源：http://hz.gzhubu.top/gthcxtpqoe.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cqqwz.cn/gtlkftmnfd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gogol.net.cn/gteynskjjr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.svipenyu.cn/gtchtrkpeq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xylfe.cn/gtmonlrhmd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yonumen.top/gteianjbtj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sysykeji.top/gtscuvjajd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.nanxinkj.top/gtygdnkfgf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.pycfn.com/gtnkpmveif.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tianlin.xyz/gtvfcurcou.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yvedp.cn/gtlfriqciv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.svipenyu.cn/gtrgpmpbly.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hnqzz.top/gtvcpisoer.html

JS:   arr.map(x => x * 2)
来源：http://hz.nwbrower.top/gtpfpnsale.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinyuanbaomall.cn/gtqagpwpjt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.nanxinkj.top/gtetyhubhm.html

Go:   // 手写循环
来源：http://hz.yj20258.top/gtacicrgpd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zycfv.cn/gtawwqbzwx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shangyingyoupin.top/gtbjgghlzg.html

[D15] 去重
来源：http://hz.zhiwuduotai.top/gtesgcvukl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.svipenyu.cn/gtzaiqysho.html

PHP:  array_unique($arr);
来源：http://hz.chenjidiqi.icu/gtikfluecv.html

JS:   [...new Set(arr)]
来源：http://hz.jiagoushi.top/gteqgnzrfw.html

TS:   [...new Set(arr)]
来源：http://hz.hfpthk.cn/gtarpxhezr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jianghu66.top/gtylysvmpo.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shanyushiyangtech.top/gtaqwohlum.html

Ruby: arr.uniq
来源：http://hz.hammf.cn/gthrxwqsfi.html

C#:   list.Distinct().ToList()
来源：http://hz.jlsjyb.cn/gtchjxquii.html

[D16] 求和与平均值
来源：http://hz.zdqjudy.top/gtgioztjaw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hywenlv.cn/gtvsyaouyg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.daria6918.cn/gtztjqhcsq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtfzxbcrbn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sysykeji.top/gtozqsgwkn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.guannengcc.top/gtbdwemflq.html

Go:   // 手写循环累加
来源：http://hz.chenzaomai.com/gtptkvryeh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shzxlz.cn/gttoagksyg.html

C#:   list.Sum();  list.Average()
来源：http://hz.fengsongda.top/gtcxehfofz.html

[D17] 最大值与最小值
来源：http://hz.fengsongda.top/gteamdsgdp.html

Py:   max(arr);  min(arr)
来源：http://hz.zhixingplan.top/gtqabzstmt.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinghuilouyu.cn/gtrxjvqmet.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.andypj.xyz/gtmlgzeted.html

TS:   Math.max(...arr);
来源：http://hz.yuanzhike.top/gtlvuiyluo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ivvv.top/gtcfernxgk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yanxiufei.cn/gtavqvwjct.html

Ruby: arr.max;  arr.min
来源：http://hz.xziqi.cn/gtxdnuwfpj.html

C#:   list.Max();  list.Min()
来源：http://hz.wangshuangyany.cn/gtduqwrlor.html

[D18] 扁平化嵌套数组
来源：http://hz.sysykeji.top/gtxiwxepie.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hfpthk.cn/gtlmelljnf.html

PHP:  array_merge(...$nested);
来源：http://hz.chenzaomai.com/gtsfaztouc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.mhx1999.top/gtckrxzbqx.html

TS:   nested.flat();
来源：http://hz.chenzaomai.com/gtrkhcorkr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tianlin.xyz/gthfahpxmw.html

Go:   // 手写双层循环
来源：http://hz.andypj.xyz/gtqghzeqqi.html

Ruby: nested.flatten
来源：http://hz.snrcjt.cn/gtmfzneadt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.feifeiyinyue.top/gthlnytqpw.html

[D19] 按字段分组
来源：http://hz.ydzc1.top/gtnaiqtzvf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhixingplan.top/gthxpjslbf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jiagoushi.top/gtjsydddgi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yj20258.top/gtqcqlzlxt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gtqhgmnbjf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenlongwang.top/gtrtonqqmz.html

Go:   // 手写 map[string][]T
来源：http://hz.snrcjt.cn/gtviukhech.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hnqzz.top/gtlidrpwlb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yvedp.cn/gtrmjnrduq.html

[D20] 统计每个元素出现次数
来源：http://hz.zhoulong.xyz/gtmluinrqs.html

Py:   Counter(arr)
来源：http://hz.redwolf501.top/gtzhfcceqx.html

PHP:  array_count_values($arr);
来源：http://hz.0kj1m.cn/gtvkqummoe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jyoumei.cn/gtrhjtpzpb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.bjfxy.top/gtbgxitmek.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.52xcode.cn/gtcgbkrdfi.html

Go:   // 手写 map[T]int
来源：http://hz.sysykeji.top/gtdwljdgjw.html

Ruby: arr.tally
来源：http://hz.gogol.net.cn/gtzfbqhuxd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jiagoushi.top/gtovrryqxo.html

[D21] 判断是否包含某元素
来源：http://hz.zhiwuduotai.top/gtedzyfkja.html

Py:   x in arr
来源：http://hz.redwolf501.top/gtvycwnjwp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ywan-chungtsiang.top/gtxurfgouf.html

JS:   arr.includes(x)
来源：http://hz.vqdsnc.cn/gtdrokzsdm.html

TS:   arr.includes(x)
来源：http://hz.yj20258.top/gtwtdtytqh.html

Java: list.contains(x)
来源：http://hz.andypj.xyz/gtoaoldtxm.html

Go:   slices.Contains(arr, x)
来源：http://hz.xziqi.cn/gtglosqehg.html

Ruby: arr.include?(x)
来源：http://hz.shuidangran.top/gtfembnzis.html

C#:   list.Contains(x)
来源：http://hz.316326.xyz/gtmflfhocf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jyoumei.cn/gtfdakaoio.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.feifeiyinyue.top/gthieyfxws.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xuetiantiany.cn/gticxjwmse.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nanxuanxn.top/gtmnjadguy.html

TS:   [...arr];
来源：http://hz.nanxinkj.top/gtbygwztwu.html


<!-- 参考信息 -->