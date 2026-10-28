代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.snrcjt.cn/gtwwhiwemk.html

Go:   return a, b
来源：http://hz.feifeiyinyue.top/gtjsjpodhu.html

Ruby: return a, b
来源：http://hz.zhaomingkeji.xyz/gtpyruaxwr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.meibo888.top/gtfnuwqzbg.html

[C06] 匿名函数 / lambda
来源：http://hz.hfpthk.cn/gtuuxeneie.html

Py:   square = lambda x: x * x
来源：http://hz.jlsjyb.cn/gtbfeafksu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj20258888.top/gtlixfxvde.html

JS:   const square = x => x * x;
来源：http://hz.zhaomingkeji.xyz/gtxbrhgvla.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.chenzaomai.com/gtntuthudg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sysykeji.top/gtkrztgatu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinghuilouyu.cn/gtbqdsxulh.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yj20258888.top/gteoqoybyl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.tianlin.xyz/gtwxbtgukv.html

[C07] 把函数作为参数传入
来源：http://hz.pycfn.com/gthcronvim.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zycfv.cn/gtqmagxmyh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shanyushiyangtech.top/gtmggirxhb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hnqzz.top/gtkbisorte.html

TS:   arr.map(String)
来源：http://hz.meibo888.top/gtwoukbtcy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gotoacloud.top/gthwfbzkan.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zycfv.cn/gtiszjhfhp.html

Ruby: arr.map(&:upcase)
来源：http://hz.yonumen.top/gtpacevpit.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.wangdashe.top/gtfoymtpbo.html

[C08] 闭包
来源：http://hz.zhijiandao.cn/gtfqqkuxpz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.sweek.top/gtbwpayaku.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhengqikj.top/gtzipyupof.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtewnkqbun.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtyvdcmmzn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sufxvd.cn/gtreyxrixz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.nanxinkj.top/gtffaorsqd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cashguo.top/gtitisxotz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cqqwz.cn/gtspnmteeq.html

[C09] 递归
来源：http://hz.ydjk.org.cn/gtomluuvfz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shanyushiyangkeji.top/gtdribykqu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xingfuxueyuan.xyz/gtaabhwfsv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhoulong.xyz/gtzqrziauv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dashuyun.cn/gtifojjeyp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xylfe.cn/gtgkpevdte.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.smart0.xyz/gtjonhiqsj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhengqikj.top/gtwqsrdiqa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sysykeji.top/gtlmuuubwk.html

[C10] 变量作用域
来源：http://hz.xuanzx.com/gtsznndwxj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shangyingyoupin.top/gtsfdjjkqn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.52xcode.cn/gtxqqwufnk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.fengsongda.top/gtojulbokw.html

TS:   同 JS
来源：http://hz.yj20258.top/gtbtxdohvj.html

Java: 方法内为块级作用域
来源：http://hz.cucudq.cn/gtlvmjeqol.html

Go:   花括号块级作用域
来源：http://hz.yonumen.top/gtoitlemow.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.snrcjt.cn/gtkodcfizp.html

C#:   块级作用域
来源：http://hz.jiagoushi.top/gtqfneuwhm.html

[C11] 模块导入与导出
来源：http://hz.xylfe.cn/gtmeithvws.html

Py:   from module import func
来源：http://hz.shanyushiyangtech.top/gtksfoopmg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.feifeiyinyue.top/gtjbaevdtl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tian-w.cn/gtvmmhlwsi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tianlin.xyz/gtoocrohno.html

Java: import java.util.List;
来源：http://hz.c1oappe.top/gtogrzfzwe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhoulong.xyz/gthyhuomtj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shuidangran.top/gtfmlppngt.html

C#:   using System.Text;
来源：http://hz.aibaodan.cn/gtdgtnnskx.html

[C12] 立即执行函数 IIFE
来源：http://hz.hfpthk.cn/gttfbrbmnj.html

Py:   (lambda: print("run"))()
来源：http://hz.svipenyu.cn/gtvtmmfiig.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cdnleiting.top/gtgdfrpwdy.html

JS:   (() => { console.log("run"); })();
来源：http://hz.0kj1m.cn/gtsgnlblsi.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cqqwz.cn/gtoyhffwil.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.haohaochexian.top/gtukxtaulh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.kuanghao11.cn/gtxovbdmyv.html

Ruby: -> { puts "run" }.call
来源：http://hz.havefunace.top/gtsfhtpclr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jianghu66.top/gtvtiizvfu.html

[C13] 类型声明 / 类型注解
来源：http://hz.yuanzhike.top/gthundkboq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yongpay.top/gttvgvplzx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtnbqxdwpx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yj202588.top/gtvsowmbil.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.smart0.xyz/gtqeckwzys.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gtlhlrvbij.html

Go:   func add(a, b int) int
来源：http://hz.tianlin.xyz/gtpyzjrswj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuanzhike.top/gtjjdfcggo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.aibaodan.cn/gtwpczrjif.html

[C14] 泛型函数
来源：http://hz.ywan-chungtsiang.top/gtronxtiaf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.bjfxy.top/gtkhwfmqyq.html

PHP:  // 无泛型
来源：http://hz.zhiwuduotai.top/gtbfkkvvel.html

JS:   // 无泛型
来源：http://hz.mhx1999.top/gtlmwudfsc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xylfe.cn/gtliqwexno.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.c1oappe.top/gtchgtmzyl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gaohongyu789.top/gthnuxoink.html

Ruby: # 无泛型
来源：http://hz.gaohongyu789.top/gtghjxnrko.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jyoumei.cn/gtsyfvjutn.html

[C15] 解构 / 展开参数
来源：http://hz.cucudq.cn/gtiijzexam.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.52xcode.cn/gtplikpdmz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shzxlz.cn/gtdcrgxqop.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ydzc1.top/gtqjmivtac.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxinkj.top/gtagupbcco.html

Java: // 无解构
来源：http://hz.tianlin.xyz/gtwjibvoco.html

Go:   // 无解构
来源：http://hz.ybcxt.top/gthsjabmft.html

Ruby: a, b = pair
来源：http://hz.gzhubu.top/gthpqjvxbi.html

C#:   var (a, b) = pair;
来源：http://hz.wangdashe.top/gtdspiamrv.html

[C16] 函数 / 方法重载
来源：http://hz.sufxvd.cn/gtemicesyt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zycfv.cn/gtdcdzfkfh.html

PHP:  // 无重载
来源：http://hz.yuxming.cn/gtykjvadpp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.dashuyun.cn/gtsbknyjuc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinyuanbaomall.cn/gtpwtgnsjr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jyoumei.cn/gtbccqvywd.html

Go:   // 无重载：用不同函数名
来源：http://hz.tianlin.xyz/gtyuwmhksq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.chenzaomai.com/gtbhtqalju.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.fzhhl.top/gtxvnxhfdg.html

================================================================================
来源：http://hz.fzhhl.top/gtbfixeife.html

D. 数组 / 列表 / 集合
来源：http://hz.jinyuanbaomall.cn/gtbepwlatq.html

================================================================================
来源：http://hz.cdnleiting.top/gtxeslbyuj.html

[D01] 创建数组 / 列表
来源：http://hz.chenjidiqi.icu/gtfqpmcpnt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gotoacloud.top/gtnhmkrvhx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sufxvd.cn/gtyxhtizbl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.haohaochexian.top/gtyzbyonyk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sweek.top/gtceasxjlx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gotoacloud.top/gtnmxyrfvx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.nwbrower.top/gtuamaheqb.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hywenlv.cn/gtjssvawqe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.tanke756.top/gtsvqjtmup.html

[D02] 追加元素到末尾
来源：http://hz.shanyushiyangkeji.top/gtjaajzeac.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.tian-w.cn/gtddybsrxu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hammf.cn/gtunrmojan.html

JS:   arr.push(4);
来源：http://hz.sufxvd.cn/gtoprqmxga.html

TS:   arr.push(4);
来源：http://hz.zhixingplan.top/gtylojxtjn.html

Java: list.add(4);
来源：http://hz.yj20258888.top/gtukhdbibg.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxinkj.top/gtoqztuqra.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.quarkkingdee.top/gtssidwugi.html

C#:   list.Add(4);
来源：http://hz.cheryme.top/gthqtgraft.html

[D03] 在指定位置插入元素
来源：http://hz.52xcode.cn/gtbwmhtrsp.html

Py:   arr.insert(0, 0)
来源：http://hz.xuetiantiany.cn/gtxlrxpfdy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cdnleiting.top/gteulxgdbp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhixingplan.top/gtammkeztc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.nanxuanxn.top/gtugdbkudw.html

Java: list.add(0, 0);
来源：http://hz.ydzc1.top/gttwudgbdx.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.aizwys.cn/gthcsvfebo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ppjwa.cn/gtmizmlwte.html

C#:   list.Insert(0, 0);
来源：http://hz.cqqwz.cn/gtxgfirxmg.html

[D04] 删除元素
来源：http://hz.yongpay.top/gtuifbxavx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yuxming.cn/gtfbfmjpxe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj20258.top/gtcpjtztsh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cqqwz.cn/gtaxxhfjpl.html

TS:   arr.splice(0, 1);
来源：http://hz.yj20258888.top/gtjmhwfzuy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinghuilouyu.cn/gtdbofdzpg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.kuanghao11.cn/gtdjonqucx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nanxinkj.top/gtxbfplcii.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jlsjyb.cn/gtiiycrclo.html

[D05] 访问与修改元素
来源：http://hz.iojbl.cn/gtzdccxgcp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pycfn.com/gtydhwmjtb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jqgfzy.top/gtfathcnjg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yuxming.cn/gtztwxljxv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shzxlz.cn/gtiiimtpfn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhongyouzk.top/gtnbtthtko.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cashguo.top/gtypwdkbub.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtmbgiovdu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yonumen.top/gtskojclla.html

[D06] 数组长度
来源：http://hz.yj20258888.top/gtswpsmjbw.html

Py:   len(arr)
来源：http://hz.gzhubu.top/gtrtmlbqdb.html

PHP:  count($arr);
来源：http://hz.jinqigufen.top/gtsqurokog.html

JS:   arr.length
来源：http://hz.feifeiyinyue.top/gtaxsgtqzy.html

TS:   arr.length
来源：http://hz.cdnleiting.top/gtxyqurlze.html

Java: list.size();
来源：http://hz.jinqigfzy.top/gtpguabssi.html

Go:   len(arr)
来源：http://hz.yj202588.top/gtxtcnolon.html

Ruby: arr.length; arr.size
来源：http://hz.yj20258.top/gtghwjrizg.html

C#:   list.Count;
来源：http://hz.xuanzx.com/gtzjfkwyrn.html

[D07] 切片 / 取子数组
来源：http://hz.ivvv.top/gtibvunvnd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zycfv.cn/gtrdesnrmt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.nanxuanxn.top/gtuyonlckm.html

JS:   arr.slice(1, 4);
来源：http://hz.cqqwz.cn/gtiqdvktms.html

TS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtaqqtshdw.html

Java: list.subList(1, 4);
来源：http://hz.zhixingplan.top/gtbluqtslc.html

Go:   arr[1:4]
来源：http://hz.birdmap.top/gtwwjqhsfr.html

Ruby: arr[1, 3]
来源：http://hz.zhijiandao.cn/gtihcumbci.html

C#:   list.GetRange(1, 3);
来源：http://hz.yonumen.top/gtndnjicpa.html

[D08] 合并两个数组
来源：http://hz.0kj1m.cn/gtmcwbdely.html

Py:   a + b;  a.extend(b)
来源：http://hz.zdqjudy.top/gtlsqjyyfd.html

PHP:  array_merge($a, $b);
来源：http://hz.yuanzhike.top/gtcjnqbsso.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.nanxuanxn.top/gtiuopqjnj.html

TS:   [...a, ...b];
来源：http://hz.shanyushiyangkeji.top/gtdlfnmztw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuanzhike.top/gtlowniibi.html

Go:   append(a, b...)
来源：http://hz.haohaochexian.top/gtkmmdrmxd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xuetiantiany.cn/gtlbgnyoaw.html

C#:   a.Concat(b).ToList()
来源：http://hz.yuanzhike.top/gtrwyrwjbw.html

[D09] 排序（升序）
来源：http://hz.jinqigfzy.top/gtvgkuyeiu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gtqsgbtqfc.html

PHP:  sort($arr);
来源：http://hz.tanke756.top/gtnjgauvye.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yanxiufei.cn/gtsicigvrk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jiagoushi.top/gtxrizerce.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jqgufenzy.top/gtbomdltvb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.snrcjt.cn/gttfvtzwsx.html

Ruby: arr.sort
来源：http://hz.yuxming.cn/gtforvqglc.html

C#:   list.Sort();
来源：http://hz.jlsjyb.cn/gtcllavvsn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ydzc1.top/gtvkxpfepk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aibaodan.cn/gtmjstcifn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuxming.cn/gtuxbrhohj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jyoumei.cn/gtpmlhbzxy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yvedp.cn/gtfarjyjck.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.birdmap.top/gthoeqngas.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yj20258888.top/gtyhlxoigk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xylfe.cn/gtctzktoxy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gogol.net.cn/gtdbdtlxna.html

[D11] 反转数组
来源：http://hz.xuanzx.com/gtpgfdmauv.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yonumen.top/gtuwaxshgm.html

PHP:  array_reverse($arr);
来源：http://hz.c1oappe.top/gtjzdbtwhr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ehwqpu.com/gtccprjmsn.html

TS:   [...arr].reverse();
来源：http://hz.yj20258.top/gtzodqtqhr.html

Java: Collections.reverse(list);
来源：http://hz.guowangkeji.top/gtsdttlvdi.html

Go:   slices.Reverse(arr)
来源：http://hz.xingfuxueyuan.xyz/gtxfwwwzyv.html

Ruby: arr.reverse
来源：http://hz.dianchejie.cn/gtnrdnqzaf.html

C#:   list.Reverse();
来源：http://hz.xingfuxueyuan.xyz/gtljyqkxky.html

[D12] 查找元素下标
来源：http://hz.gzhubu.top/gtgfdkjpek.html

Py:   arr.index(x);  x in arr
来源：http://hz.gotoacloud.top/gtwaymkwft.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hongshengwenyu.top/gtrwjkmtol.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cqqwz.cn/gtnxosgcgm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.0kj1m.cn/gtcskfsfbm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xingfuxueyuan.xyz/gtpjbbfdbu.html

Go:   slices.Index(arr, x)
来源：http://hz.xuanzx.com/gtrxditkxy.html

Ruby: arr.index(x)
来源：http://hz.shanyushiyangtech.top/gtouavuzai.html

C#:   list.IndexOf(x);
来源：http://hz.ydzc1.top/gtxogknyfo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.fzhhl.top/gtzjweukap.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zdqjudy.top/gtsldwlytk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinghuilouyu.cn/gtpdjhtuea.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ehwqpu.com/gtqzbkqcqf.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tianlin.xyz/gttknuhgsn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ivvv.top/gtjjrgsrzd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yongpay.top/gttutbpawg.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenlongwang.top/gtvepofvzv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.dashuyun.cn/gttplthpxu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nanxuanxn.top/gtyuvcmaja.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xuetiantiany.cn/gtxmbltwmc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sweek.top/gtiohuwqui.html

JS:   arr.map(x => x * 2)
来源：http://hz.gzhubu.top/gtktjmhapb.html

TS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangkeji.top/gtqeffplnf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.fzhhl.top/gthaqimnqc.html

Go:   // 手写循环
来源：http://hz.xziqi.cn/gtcqdrftlu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yuanzhike.top/gthhlindta.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tianlin.xyz/gtvjpqmypr.html

[D15] 去重
来源：http://hz.havefunace.top/gtqqnpzhwv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydzc1.top/gtnlbtmvzf.html

PHP:  array_unique($arr);
来源：http://hz.hongshengwenyu.top/gtxlqzmsna.html

JS:   [...new Set(arr)]
来源：http://hz.xinyue.icu/gtjeexmcsj.html

TS:   [...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gtisfrtqpc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.tanke756.top/gtunqkzbwy.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jyoumei.cn/gtfwlmzefw.html

Ruby: arr.uniq
来源：http://hz.daxiang520.top/gtazvdeibe.html

C#:   list.Distinct().ToList()
来源：http://hz.sysykeji.top/gtmwodcluc.html

[D16] 求和与平均值
来源：http://hz.shanyushiyangtech.top/gtgouvdtea.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.wangshuangyany.cn/gtcgesxwsp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shzxlz.cn/gtuymryfel.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shangyingyoupin.top/gtaotyibii.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xylfe.cn/gthzejmiyb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.meibo888.top/gtmugfampv.html

Go:   // 手写循环累加
来源：http://hz.vqdsnc.cn/gtapvhqpni.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ivvv.top/gtpdecqbbj.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenzaomai.com/gtpjevcdej.html

[D17] 最大值与最小值
来源：http://hz.quarkkingdee.top/gtpzrnfxga.html

Py:   max(arr);  min(arr)
来源：http://hz.yongpay.top/gtvdtzurzd.html

PHP:  max($arr);  min($arr);
来源：http://hz.cdnleiting.top/gtmwbtenaj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhongyouzk.top/gtnygrchoc.html

TS:   Math.max(...arr);
来源：http://hz.yuanzhike.top/gtsonlthvn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.mhx1999.top/gtztxygsux.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.nanxuanxn.top/gtdehmwjiv.html

Ruby: arr.max;  arr.min
来源：http://hz.wangshuangyany.cn/gtlqoyxbnz.html

C#:   list.Max();  list.Min()
来源：http://hz.hfpthk.cn/gtifllngmq.html

[D18] 扁平化嵌套数组
来源：http://hz.ybcxt.top/gtefbybigw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shuidangran.top/gtnllxirlx.html

PHP:  array_merge(...$nested);
来源：http://hz.tianlin.xyz/gtbbttootw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hfpthk.cn/gttecmvnsz.html

TS:   nested.flat();
来源：http://hz.guannengcc.top/gtspvwmbzu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhoulong.xyz/gttuopemob.html

Go:   // 手写双层循环
来源：http://hz.jianghu66.top/gtjuahgsbe.html

Ruby: nested.flatten
来源：http://hz.52xcode.cn/gtqivmkqei.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xziqi.cn/gtouueugls.html

[D19] 按字段分组
来源：http://hz.aizwys.cn/gtwxxfrnnc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.tian-w.cn/gtcbknkgtz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuanzx.com/gtiyvhtuzi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hysaishi.cn/gtrcldkiqv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jqgfzy.top/gtjvydrqij.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gotoacloud.top/gtudphchlr.html

Go:   // 手写 map[string][]T
来源：http://hz.yanxiufei.cn/gtldkplikd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ppjwa.cn/gtajgwzuyk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yvedp.cn/gtzdxqvzmp.html

[D20] 统计每个元素出现次数
来源：http://hz.yj202588.top/gtxelhcove.html

Py:   Counter(arr)
来源：http://hz.316326.xyz/gtrboyepvf.html

PHP:  array_count_values($arr);
来源：http://hz.fengsongda.top/gtptwgkchl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhixingplan.top/gtzgdmtxrg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yonumen.top/gtedhiaaew.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gotoacloud.top/gtjynccmcd.html

Go:   // 手写 map[T]int
来源：http://hz.jiagoushi.top/gtaurskmum.html

Ruby: arr.tally
来源：http://hz.yongpay.top/gtmvpjpfhe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shzxlz.cn/gtmqrubsoa.html

[D21] 判断是否包含某元素
来源：http://hz.kuanghao11.cn/gtiguutieg.html

Py:   x in arr
来源：http://hz.bjfxy.top/gtcrdvigyw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.aibaodan.cn/gtxhrgewmr.html

JS:   arr.includes(x)
来源：http://hz.hammf.cn/gttjlrwrdu.html

TS:   arr.includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtesjorgpj.html

Java: list.contains(x)
来源：http://hz.svipenyu.cn/gtdfvthgbp.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuanzhike.top/gtzhktxwci.html

Ruby: arr.include?(x)
来源：http://hz.shzxlz.cn/gtfxigiyen.html

C#:   list.Contains(x)
来源：http://hz.redwolf501.top/gtizukpahk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ivvv.top/gtsyvtyawa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yuxming.cn/gtjcpepyeg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aibaodan.cn/gtlbpqutmm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nanxuanxn.top/gtzessolyi.html

TS:   [...arr];
来源：http://hz.vqdsnc.cn/gtchovxhia.html


<!-- 参考信息 -->