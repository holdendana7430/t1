代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ydzc1.top/gtoseedfgv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shanyushiyangkeji.top/gtlejiupsu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.bjfxy.top/gtiqxmtmea.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.pengpengdd.cyou/gtzgiogkma.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.tanke756.top/gtwjuhuxgp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.aizwys.cn/gtskzvwbnn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gtrdgohkgm.html

[C09] 递归
来源：http://hz.hfpthk.cn/gtvwxcwyst.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.dashuyun.cn/gtjzkyxinc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinqigfzy.top/gtnsvajkdh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yanxiufei.cn/gttzpdmlof.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ppjwa.cn/gteqafszcc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yj20258.top/gtbkknnceu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.pengpengdd.cyou/gtcaplypwx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dashuyun.cn/gtyqdjhcff.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gaohongyu789.top/gtqdmjbftt.html

[C10] 变量作用域
来源：http://hz.9152youxi.cn/gtaxkxcvlc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aizwys.cn/gtgdjuhxvo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shanyushiyangkeji.top/gtbkcieqrz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.andypj.xyz/gtbvmhafqm.html

TS:   同 JS
来源：http://hz.shanyushiyangtech.top/gttjggdeqs.html

Java: 方法内为块级作用域
来源：http://hz.zdqjudy.top/gtayzqgbpw.html

Go:   花括号块级作用域
来源：http://hz.shangyingyoupin.top/gtancrghhr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhengqikj.top/gtrxlinegi.html

C#:   块级作用域
来源：http://hz.ehwqpu.com/gtlcwvpwsi.html

[C11] 模块导入与导出
来源：http://hz.chenjidiqi.icu/gtocloossg.html

Py:   from module import func
来源：http://hz.zhiwuduotai.top/gtdocyhkgt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nanxuanxn.top/gtwvzesznf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jqgfzy.top/gtjwctfdqa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tian-w.cn/gtkbqvcmsc.html

Java: import java.util.List;
来源：http://hz.jqgfzy.top/gtswzrahqh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ydjk.org.cn/gtzfqiwyal.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daria6918.cn/gtvbdioyzt.html

C#:   using System.Text;
来源：http://hz.xingfuxueyuan.xyz/gtoboagqbg.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj20258.top/gtebcfvvuv.html

Py:   (lambda: print("run"))()
来源：http://hz.zhongyouzk.top/gtkewcxyaq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xziqi.cn/gtznfvntbi.html

JS:   (() => { console.log("run"); })();
来源：http://hz.vqdsnc.cn/gttpmeppsm.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtzhdryouu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.redwolf501.top/gtmrbgrjpl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cqqwz.cn/gtreedqydj.html

Ruby: -> { puts "run" }.call
来源：http://hz.chenzaomai.com/gtuyqjvnut.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ywan-chungtsiang.top/gtgeiadoxx.html

[C13] 类型声明 / 类型注解
来源：http://hz.hongshengwenyu.top/gtruxqtomo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hywenlv.cn/gtstoomjni.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gttocpsznc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xuanzx.com/gtjayvrwjb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtauuvuujo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gtjhabtcnw.html

Go:   func add(a, b int) int
来源：http://hz.sxryk.cn/gtfhbtzvsl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yueranfly.top/gtmhhtlmup.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yvedp.cn/gtchybbkdk.html

[C14] 泛型函数
来源：http://hz.tian-w.cn/gttvfkysqm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.aibaodan.cn/gtriovxatk.html

PHP:  // 无泛型
来源：http://hz.yuxming.cn/gtjiwmtttz.html

JS:   // 无泛型
来源：http://hz.jinqigufen.top/gtjitjavmy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhengqikj.top/gtsdysjpeo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.snrcjt.cn/gtkfdnbthi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zdqjudy.top/gtltyogqwa.html

Ruby: # 无泛型
来源：http://hz.mhx1999.top/gtsowbvhac.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuanzhike.top/gtbskstpgt.html

[C15] 解构 / 展开参数
来源：http://hz.shuidangran.top/gtwvrgtpvt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jiagoushi.top/gtlzptujsi.html

PHP:  [$a, $b] = $pair;
来源：http://hz.wangshuangyany.cn/gtxclpnpva.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.aibaodan.cn/gteoymxdlc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cucudq.cn/gthshkctep.html

Java: // 无解构
来源：http://hz.mhx1999.top/gtansgkmiw.html

Go:   // 无解构
来源：http://hz.yuxming.cn/gtzvhpzkei.html

Ruby: a, b = pair
来源：http://hz.feifeiyinyue.top/gtgzdcrdep.html

C#:   var (a, b) = pair;
来源：http://hz.chenlongwang.top/gtdkhzgdkz.html

[C16] 函数 / 方法重载
来源：http://hz.xuanzx.com/gtjjheindj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.iojbl.cn/gtmqaqjklh.html

PHP:  // 无重载
来源：http://hz.sysykeji.top/gtebpajwsz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.daxiang520.top/gtnrrydeys.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.havefunace.top/gtlkrfimnj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cqqwz.cn/gtztqdjejg.html

Go:   // 无重载：用不同函数名
来源：http://hz.zycfv.cn/gtbobcypql.html

Ruby: # 无重载：靠动态参数
来源：http://hz.dashuyun.cn/gtczjloxsx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hywenlv.cn/gtrgpunwib.html

================================================================================
来源：http://hz.snrcjt.cn/gtnchigauf.html

D. 数组 / 列表 / 集合
来源：http://hz.yuanzhike.top/gtmyjnacet.html

================================================================================
来源：http://hz.yanxiufei.cn/gthdelulry.html

[D01] 创建数组 / 列表
来源：http://hz.fengsongda.top/gtwppsbbvw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hnqzz.top/gtvqrcustt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.pycfn.com/gtjkkvfmil.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigfzy.top/gtlsbcmtpx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.birdmap.top/gteuccexqc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.tanke756.top/gtgjulnauz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.tianlin.xyz/gtfrowkrrw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.aizwys.cn/gtsgtncyia.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jlsjyb.cn/gtqixtkewd.html

[D02] 追加元素到末尾
来源：http://hz.daxiang520.top/gtjwxdfepf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.snrcjt.cn/gtvfcfeblk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.wangshuangyany.cn/gtuduhtcdz.html

JS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtdlccywef.html

TS:   arr.push(4);
来源：http://hz.nwbrower.top/gteofknetp.html

Java: list.add(4);
来源：http://hz.tianlin.xyz/gtvjtcsxwx.html

Go:   arr = append(arr, 4)
来源：http://hz.shuidangran.top/gtzwdappzn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.pengpengdd.cyou/gtuicltyab.html

C#:   list.Add(4);
来源：http://hz.shangyingyoupin.top/gtigqewzyn.html

[D03] 在指定位置插入元素
来源：http://hz.jinghuilouyu.cn/gtnikiordv.html

Py:   arr.insert(0, 0)
来源：http://hz.pengpengdd.cyou/gtsqejvnpn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.tian-w.cn/gtijugsklc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.fengsongda.top/gtwffybnty.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ydjk.org.cn/gtscopzfwl.html

Java: list.add(0, 0);
来源：http://hz.shanyushiyangkeji.top/gthcezxwom.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.aibaodan.cn/gtfrfbodmm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yvedp.cn/gtyxfighbg.html

C#:   list.Insert(0, 0);
来源：http://hz.xziqi.cn/gtwjhwkyql.html

[D04] 删除元素
来源：http://hz.ywan-chungtsiang.top/gtxgmncdhq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.fzhhl.top/gtztlfinss.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.dianchejie.cn/gtakivxmgf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nanxuanxn.top/gtyuonqope.html

TS:   arr.splice(0, 1);
来源：http://hz.ywan-chungtsiang.top/gtarwwndbf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.kuanghao11.cn/gtrvdecssn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cheryme.top/gtkxwaumzp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinqigufen.top/gtteitkrki.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.316326.xyz/gtxuhwcony.html

[D05] 访问与修改元素
来源：http://hz.xinyue.icu/gtgzkfnayh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nwbrower.top/gtnrsmkytb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.guannengcc.top/gtqcmfjobr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tanke756.top/gttoixjozm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.dashuyun.cn/gtombwjfdb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jianghu66.top/gtpzoyxlll.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.nanxuanxn.top/gtmuhpjpdk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ywan-chungtsiang.top/gtvlqlnaey.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xuanzx.com/gthpdmgryn.html

[D06] 数组长度
来源：http://hz.shzxlz.cn/gtxfipfgcu.html

Py:   len(arr)
来源：http://hz.jqgufenzy.top/gtodpopufb.html

PHP:  count($arr);
来源：http://hz.jyoumei.cn/gtxdwdxqer.html

JS:   arr.length
来源：http://hz.yj20258888.top/gtemidrhms.html

TS:   arr.length
来源：http://hz.zhijiandao.cn/gtrkitfqdm.html

Java: list.size();
来源：http://hz.ehwqpu.com/gtyolswsbo.html

Go:   len(arr)
来源：http://hz.sxryk.cn/gttnzfhbju.html

Ruby: arr.length; arr.size
来源：http://hz.hnxiangtu.top/gtomscqcsn.html

C#:   list.Count;
来源：http://hz.zhijiandao.cn/gtikmytjmq.html

[D07] 切片 / 取子数组
来源：http://hz.snrcjt.cn/gtpxiwoukg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yonumen.top/gtymuhenoj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.pycfn.com/gttfyqjzny.html

JS:   arr.slice(1, 4);
来源：http://hz.shangyingyoupin.top/gtdzlydwfv.html

TS:   arr.slice(1, 4);
来源：http://hz.hysaishi.cn/gtagjcgycm.html

Java: list.subList(1, 4);
来源：http://hz.cdnleiting.top/gtzieotcsn.html

Go:   arr[1:4]
来源：http://hz.aizwys.cn/gtoulgnpar.html

Ruby: arr[1, 3]
来源：http://hz.zhixingplan.top/gtvnumpmux.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangkeji.top/gtjeisksbi.html

[D08] 合并两个数组
来源：http://hz.pengpengdd.cyou/gtddqfkrma.html

Py:   a + b;  a.extend(b)
来源：http://hz.cqqwz.cn/gtgyimctev.html

PHP:  array_merge($a, $b);
来源：http://hz.xziqi.cn/gthkmufnsj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yueranfly.top/gtbqimagsm.html

TS:   [...a, ...b];
来源：http://hz.havefunace.top/gtixbflyzq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.haohaochexian.top/gtknecwlyq.html

Go:   append(a, b...)
来源：http://hz.ybcxt.top/gtniwwtnet.html

Ruby: a + b;  a.concat(b)
来源：http://hz.haohaochexian.top/gtrixhmins.html

C#:   a.Concat(b).ToList()
来源：http://hz.havefunace.top/gtmwzfkees.html

[D09] 排序（升序）
来源：http://hz.daria6918.cn/gtopyntsej.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.vqdsnc.cn/gtnroeufdo.html

PHP:  sort($arr);
来源：http://hz.cashguo.top/gtjwhqtmms.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hysaishi.cn/gtiblxusvc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.guowangkeji.top/gtizdktqik.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gzhubu.top/gtpbtsuasm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hywenlv.cn/gtwgmtvmww.html

Ruby: arr.sort
来源：http://hz.zhongyouzk.top/gtirlgrdnz.html

C#:   list.Sort();
来源：http://hz.chenzaomai.com/gtdqofpuog.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.316326.xyz/gttmrebmit.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sweek.top/gtxbxoeofc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gthhtbrmvc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aibaodan.cn/gtzgqryotl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xinyue.icu/gtmfwfipzj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhaomingkeji.xyz/gteqsqtpis.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhixingplan.top/gtktouinqm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nanxinkj.top/gtkdkrfyrm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj20258888.top/gtlmvfiquf.html

[D11] 反转数组
来源：http://hz.yanxiufei.cn/gtktgadidj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.tian-w.cn/gtpuefddjy.html

PHP:  array_reverse($arr);
来源：http://hz.tian-w.cn/gtyqijoznd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.sufxvd.cn/gtqfdasqdk.html

TS:   [...arr].reverse();
来源：http://hz.c1oappe.top/gtstnndhal.html

Java: Collections.reverse(list);
来源：http://hz.andypj.xyz/gtkftnxhvw.html

Go:   slices.Reverse(arr)
来源：http://hz.fzhhl.top/gtpulrbvvp.html

Ruby: arr.reverse
来源：http://hz.wangshuangyany.cn/gtaozqqcnw.html

C#:   list.Reverse();
来源：http://hz.guowangkeji.top/gtistdgbjv.html

[D12] 查找元素下标
来源：http://hz.cqqwz.cn/gtldjdxrya.html

Py:   arr.index(x);  x in arr
来源：http://hz.shanyushiyangtech.top/gtaytmsgcc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nanxuanxn.top/gtoxffppec.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtqaqgsmjl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenlongwang.top/gtxbryfwsl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tanke756.top/gtauwcaeby.html

Go:   slices.Index(arr, x)
来源：http://hz.jqgfzy.top/gtlrpbdrnm.html

Ruby: arr.index(x)
来源：http://hz.zycfv.cn/gthxcqsfub.html

C#:   list.IndexOf(x);
来源：http://hz.ydjk.org.cn/gtpjegtrvr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.guowangkeji.top/gtribvxfac.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hammf.cn/gtjlfschur.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ivvv.top/gtaihzqcck.html

JS:   arr.filter(x => x > 3)
来源：http://hz.dianchejie.cn/gtarlbztbs.html

TS:   arr.filter(x => x > 3)
来源：http://hz.chenjidiqi.icu/gtswnjanox.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xuetiantiany.cn/gthtnqdtzs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.svipenyu.cn/gtplaegulz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shuidangran.top/gtismklobo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cucudq.cn/gtxbaavgku.html

[D14] 映射转换（每个元素变形）
来源：http://hz.kuanghao11.cn/gtqklpvfhi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tian-w.cn/gtrizreftn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yj20258.top/gtietvondz.html

JS:   arr.map(x => x * 2)
来源：http://hz.tanke756.top/gtcffkccfj.html

TS:   arr.map(x => x * 2)
来源：http://hz.hysaishi.cn/gthvasrgsh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jlsjyb.cn/gtgoeqlsnw.html

Go:   // 手写循环
来源：http://hz.shangyingyoupin.top/gtocoudmmc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhengqikj.top/gtdzohpydi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dashuyun.cn/gtzdaoqluz.html

[D15] 去重
来源：http://hz.xuanzx.com/gtczscjxfm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cashguo.top/gtlpzoehhn.html

PHP:  array_unique($arr);
来源：http://hz.zhengqikj.top/gtoltmgbrc.html

JS:   [...new Set(arr)]
来源：http://hz.chenlongwang.top/gtqkkvsane.html

TS:   [...new Set(arr)]
来源：http://hz.yanxiufei.cn/gtkwpeawll.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yuxming.cn/gtbnnfagri.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.sxryk.cn/gtvowutwdk.html

Ruby: arr.uniq
来源：http://hz.birdmap.top/gtmfmxgnav.html

C#:   list.Distinct().ToList()
来源：http://hz.yanxiufei.cn/gtdkbroakr.html

[D16] 求和与平均值
来源：http://hz.cdnleiting.top/gtqdbqmuua.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cdnleiting.top/gtxaghiyfm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hfpthk.cn/gtlitujapn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cdnleiting.top/gtpthvcmep.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.bjfxy.top/gtxoitfnvs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj20258.top/gtybqudyqu.html

Go:   // 手写循环累加
来源：http://hz.sxryk.cn/gtquoyzvjf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.redwolf501.top/gtrfilndyb.html

C#:   list.Sum();  list.Average()
来源：http://hz.wangshuangyany.cn/gtcvogkkel.html

[D17] 最大值与最小值
来源：http://hz.chenzaomai.com/gtenajmojl.html

Py:   max(arr);  min(arr)
来源：http://hz.chenzaomai.com/gtwyhpxlqy.html

PHP:  max($arr);  min($arr);
来源：http://hz.pycfn.com/gtisoobdtb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yanxiufei.cn/gthrkvvvah.html

TS:   Math.max(...arr);
来源：http://hz.fzhhl.top/gthjfnryeg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yanxiufei.cn/gthaawwdnn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.52xcode.cn/gtmykicwae.html

Ruby: arr.max;  arr.min
来源：http://hz.shanyushiyangkeji.top/gtoahhyupy.html

C#:   list.Max();  list.Min()
来源：http://hz.cucudq.cn/gtocfvrtiu.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangtech.top/gttykqoams.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sufxvd.cn/gtcaeyzylm.html

PHP:  array_merge(...$nested);
来源：http://hz.jianghu66.top/gtojvuklhn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.aibaodan.cn/gtezwbptsp.html

TS:   nested.flat();
来源：http://hz.tanke756.top/gtwibzaskv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gogol.net.cn/gtbnhpkaea.html

Go:   // 手写双层循环
来源：http://hz.zhaomingkeji.xyz/gtjmixfnww.html

Ruby: nested.flatten
来源：http://hz.pengpengdd.cyou/gtafekvavw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jqgfzy.top/gtpquoojsj.html

[D19] 按字段分组
来源：http://hz.shangyingyoupin.top/gthsttcvry.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ywan-chungtsiang.top/gtnlcuegjo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.gzhubu.top/gtzhqrgchx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jiagoushi.top/gtmzmwulrh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gtcrujudlo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zycfv.cn/gtjpzakttx.html

Go:   // 手写 map[string][]T
来源：http://hz.ydjk.org.cn/gttbmlqfmg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.svipenyu.cn/gtgqrainqr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yongpay.top/gtnekpkvdi.html

[D20] 统计每个元素出现次数
来源：http://hz.jinghuilouyu.cn/gtigaalqoh.html

Py:   Counter(arr)
来源：http://hz.jinghuilouyu.cn/gtsilwoylw.html

PHP:  array_count_values($arr);
来源：http://hz.316326.xyz/gtgxeubnja.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.52xcode.cn/gtvtndzstm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gtdhiqepdf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.chenzaomai.com/gtavmrsewh.html

Go:   // 手写 map[T]int
来源：http://hz.ydzc1.top/gtsjxbwbwj.html

Ruby: arr.tally
来源：http://hz.yj20258.top/gtaykeprvz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.havefunace.top/gtwwoqziwu.html

[D21] 判断是否包含某元素
来源：http://hz.jianghu66.top/gtyeupklar.html

Py:   x in arr
来源：http://hz.aibaodan.cn/gtfvolrdmt.html

PHP:  in_array($x, $arr, true);
来源：http://hz.wangshuangyany.cn/gtobnpcrij.html

JS:   arr.includes(x)
来源：http://hz.hfpthk.cn/gtjhfwuisn.html

TS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtsgziobtw.html

Java: list.contains(x)
来源：http://hz.birdmap.top/gtzvnrvfxr.html

Go:   slices.Contains(arr, x)
来源：http://hz.sufxvd.cn/gtczprmzik.html

Ruby: arr.include?(x)
来源：http://hz.cdnleiting.top/gtwcsupqup.html

C#:   list.Contains(x)
来源：http://hz.52xcode.cn/gtprxdmxyo.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhijiandao.cn/gtrrnzczty.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hammf.cn/gtsutjtjxv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tianlin.xyz/gthmcpqgcg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.guowangkeji.top/gtdgpooxpx.html

TS:   [...arr];
来源：http://hz.ivvv.top/gtszpjpscu.html

Java: new ArrayList<>(list);
来源：http://hz.xuetiantiany.cn/gtimggycam.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.wangdashe.top/gtmnkfdufs.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinghuilouyu.cn/gtcqyzrljg.html

C#:   new List<int>(list);
来源：http://hz.guowangkeji.top/gtodqhseem.html

[D23] reduce 累积计算
来源：http://hz.daxiang520.top/gtqqolcjnl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.wangshuangyany.cn/gttdvllqzc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hnqzz.top/gtpomfelhl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.quarkkingdee.top/gtjbzhwsja.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydzc1.top/gtppktnvnh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ppjwa.cn/gtmetrcfrf.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gtoindtokz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sweek.top/gtmxvtqhqq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenlongwang.top/gtvmfnkygr.html

[D24] 字典 / Map 基本操作
来源：http://hz.guannengcc.top/gtihwrgeld.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aibaodan.cn/gtdgeofonv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangkeji.top/gtywzztxjn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xinyue.icu/gtyydbiyuu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.fengsongda.top/gtkanxojxq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cheryme.top/gtywfczroz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xylfe.cn/gtewrtmgsl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydjk.org.cn/gtxolvwuih.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hnxiangtu.top/gteifzjvsr.html

[D25] Set 集合去重与交并差
来源：http://hz.quarkkingdee.top/gtmsbfkgkc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.nanxinkj.top/gthggxxdmx.html


<!-- 参考信息 -->