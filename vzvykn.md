代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jqgfzy.top/gtfmrjdyso.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhiwuduotai.top/gtxbdxylxa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ywan-chungtsiang.top/gtswomngmk.html

Ruby: def greet(name = "World") = name
来源：http://hz.gaohongyu789.top/gtbzroomaz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.fzhhl.top/gtoomwgsxn.html

[C03] 可变参数
来源：http://hz.birdmap.top/gtqpddgkmr.html

Py:   def total(*args): return sum(args)
来源：http://hz.tanke756.top/gtyqxwxvex.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yongpay.top/gtydoufmua.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhijiandao.cn/gtuthatutj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cheryme.top/gtamgcnkks.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.nanxuanxn.top/gtnrhumzyi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ppjwa.cn/gtavwwevrf.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinqigfzy.top/gtvdqjsrrq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hysaishi.cn/gtykylifdw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ehwqpu.com/gtbfrjhjcp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.guowangkeji.top/gtuaybpdjh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jqgfzy.top/gtrjrkpwdh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.feifeiyinyue.top/gtpimhyeht.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hongshengwenyu.top/gtmmanvzxw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xingfuxueyuan.xyz/gtkyazvqxe.html

Go:   // 无：用配置结构体参数
来源：http://hz.jiagoushi.top/gtgccxuhtz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtzqzgqzpu.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinqigfzy.top/gtlrivjpdv.html

[C05] 返回多个值
来源：http://hz.wangshuangyany.cn/gtujhbhery.html

Py:   return a, b
来源：http://hz.9152youxi.cn/gtgqljngjb.html

PHP:  return [$a, $b];
来源：http://hz.yuxming.cn/gtnrjjjanc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jqgfzy.top/gtyxbqdbrw.html

TS:   return { a, b };
来源：http://hz.ppjwa.cn/gtqtdxbfxx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ydzc1.top/gtrljvhwkp.html

Go:   return a, b
来源：http://hz.cqqwz.cn/gtosuitane.html

Ruby: return a, b
来源：http://hz.meibo888.top/gtfsqmbrhw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dianchejie.cn/gtrxoigtwg.html

[C06] 匿名函数 / lambda
来源：http://hz.dashuyun.cn/gtsgueiauv.html

Py:   square = lambda x: x * x
来源：http://hz.cdnleiting.top/gtxtfdxkic.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.sysykeji.top/gtdylrxugb.html

JS:   const square = x => x * x;
来源：http://hz.ybcxt.top/gtfkaxecdu.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gogol.net.cn/gttcudwmps.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.mhx1999.top/gtezgqlgwu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tanke756.top/gtayfbnstb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.sxryk.cn/gtrrqhupyt.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuetiantiany.cn/gtlwpbqngs.html

[C07] 把函数作为参数传入
来源：http://hz.jqgfzy.top/gtrmykbpmr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cashguo.top/gttfqivyof.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.fzhhl.top/gttrzwziwi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.redwolf501.top/gtfturzazn.html

TS:   arr.map(String)
来源：http://hz.sweek.top/gtpfiiybfb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgufenzy.top/gttioziejw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhengqikj.top/gtbvnrfggb.html

Ruby: arr.map(&:upcase)
来源：http://hz.jianghu66.top/gtxjomkmer.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhixingplan.top/gtaeasfylf.html

[C08] 闭包
来源：http://hz.haohaochexian.top/gtwbktacdv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.iojbl.cn/gttvyukwxo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yvedp.cn/gthqtonqol.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinqigufen.top/gttxeuasyi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hammf.cn/gtfvzsupdo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jlsjyb.cn/gtvvexoeaw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.fzhhl.top/gtaegfddyc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yvedp.cn/gtdskciodq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtqbnodbgs.html

[C09] 递归
来源：http://hz.sxryk.cn/gtostgqvku.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.iojbl.cn/gtucfpcxjv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cucudq.cn/gtojzscwqd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shangyingyoupin.top/gtdjevseth.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinyuanbaomall.cn/gtyxzdslnr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gzhubu.top/gteolgpwjg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ehwqpu.com/gtmwhruwtb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ehwqpu.com/gttfpoixqd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.aibaodan.cn/gtupypsvks.html

[C10] 变量作用域
来源：http://hz.wangshuangyany.cn/gtiaattwft.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zycfv.cn/gtaoklfdoe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shanyushiyangtech.top/gtazopqarf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ydjk.org.cn/gtsjjuhvnz.html

TS:   同 JS
来源：http://hz.jlsjyb.cn/gtkzpiivot.html

Java: 方法内为块级作用域
来源：http://hz.hammf.cn/gtmvpvqagz.html

Go:   花括号块级作用域
来源：http://hz.shzxlz.cn/gtuulcafuv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cheryme.top/gtjoujircf.html

C#:   块级作用域
来源：http://hz.gotoacloud.top/gtzubbltso.html

[C11] 模块导入与导出
来源：http://hz.aizwys.cn/gtafwntaho.html

Py:   from module import func
来源：http://hz.birdmap.top/gtdlanrhan.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.9152youxi.cn/gtggcvkkjc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jlsjyb.cn/gtfbynbnnu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.pycfn.com/gtlcrjasfv.html

Java: import java.util.List;
来源：http://hz.gotoacloud.top/gtfdhygztm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.dianchejie.cn/gtrahggvxx.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.aizwys.cn/gtrahgylnl.html

C#:   using System.Text;
来源：http://hz.birdmap.top/gtfrhsumlq.html

[C12] 立即执行函数 IIFE
来源：http://hz.yuxming.cn/gtdnwyrftz.html

Py:   (lambda: print("run"))()
来源：http://hz.aizwys.cn/gtpxdqfuda.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shanyushiyangtech.top/gtimxxtcao.html

JS:   (() => { console.log("run"); })();
来源：http://hz.nwbrower.top/gtovvmfwwa.html

TS:   (() => { console.log("run"); })();
来源：http://hz.havefunace.top/gtrsfpzyjf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.vqdsnc.cn/gtuyxxqkiz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hywenlv.cn/gtymljbhlg.html

Ruby: -> { puts "run" }.call
来源：http://hz.xuanzx.com/gtfcftnpsw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cashguo.top/gtdfxjwmgb.html

[C13] 类型声明 / 类型注解
来源：http://hz.tian-w.cn/gttnyorbyw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yueranfly.top/gtdavxvuex.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnxiangtu.top/gtigtbbaij.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cashguo.top/gtmdnnimuv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.andypj.xyz/gtzyjwkuzj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtdpnfvjcm.html

Go:   func add(a, b int) int
来源：http://hz.yj20258.top/gtyigoomsa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jqgfzy.top/gtzdiynksm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.svipenyu.cn/gtemubmdsv.html

[C14] 泛型函数
来源：http://hz.jianghu66.top/gtsddtomur.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shanyushiyangtech.top/gtyxihacqw.html

PHP:  // 无泛型
来源：http://hz.cheryme.top/gtcwppetub.html

JS:   // 无泛型
来源：http://hz.nanxinkj.top/gtydngogui.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.svipenyu.cn/gtrgxlzall.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xingfuxueyuan.xyz/gttvncthkw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhongyouzk.top/gtrdlnwmkw.html

Ruby: # 无泛型
来源：http://hz.zhengqikj.top/gtktynxgvt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hfpthk.cn/gtxnqhdxbj.html

[C15] 解构 / 展开参数
来源：http://hz.xylfe.cn/gthdjdnrzc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yonumen.top/gtlgcyvukv.html

PHP:  [$a, $b] = $pair;
来源：http://hz.havefunace.top/gtzslvbiwa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shanyushiyangkeji.top/gtojqefanl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xinyue.icu/gtqxfpycsz.html

Java: // 无解构
来源：http://hz.hywenlv.cn/gtpazjxwtz.html

Go:   // 无解构
来源：http://hz.xuetiantiany.cn/gtusvtoyxc.html

Ruby: a, b = pair
来源：http://hz.gogol.net.cn/gtjfsuouit.html

C#:   var (a, b) = pair;
来源：http://hz.52xcode.cn/gtjluslyvu.html

[C16] 函数 / 方法重载
来源：http://hz.daxiang520.top/gtfeslfixf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ywan-chungtsiang.top/gtkzyxtmki.html

PHP:  // 无重载
来源：http://hz.nanxuanxn.top/gtkdssnbap.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jqgufenzy.top/gtjycptutb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gzhubu.top/gtqnljgmhk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tian-w.cn/gtnysrxbyt.html

Go:   // 无重载：用不同函数名
来源：http://hz.shangyingyoupin.top/gthnwxajwa.html

Ruby: # 无重载：靠动态参数
来源：http://hz.kuanghao11.cn/gtozewzvan.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xingfuxueyuan.xyz/gtxxwtzauj.html

================================================================================
来源：http://hz.316326.xyz/gtnxvxjcxz.html

D. 数组 / 列表 / 集合
来源：http://hz.havefunace.top/gtiufrslgc.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtikqihzdw.html

[D01] 创建数组 / 列表
来源：http://hz.andypj.xyz/gtwgreirpc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xuetiantiany.cn/gtckpcrzdg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhoulong.xyz/gtilaucaag.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hysaishi.cn/gtnqfeuoje.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sufxvd.cn/gthwfzjrow.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.snrcjt.cn/gttkwxocbp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shuidangran.top/gtppggwzbt.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nanxinkj.top/gthymrwqyz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.nwbrower.top/gtlgakbvxa.html

[D02] 追加元素到末尾
来源：http://hz.nanxuanxn.top/gtkywwhvak.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.andypj.xyz/gtwjfxgoia.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinqigfzy.top/gteokfgoaf.html

JS:   arr.push(4);
来源：http://hz.ydzc1.top/gtrdsnlpok.html

TS:   arr.push(4);
来源：http://hz.sufxvd.cn/gtlfojsnvi.html

Java: list.add(4);
来源：http://hz.ydjk.org.cn/gtusqcuwja.html

Go:   arr = append(arr, 4)
来源：http://hz.shanyushiyangkeji.top/gtvfdxyblh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yj20258888.top/gtagrmztfr.html

C#:   list.Add(4);
来源：http://hz.snrcjt.cn/gthhhfhcrt.html

[D03] 在指定位置插入元素
来源：http://hz.wangdashe.top/gtohpgtltf.html

Py:   arr.insert(0, 0)
来源：http://hz.hnqzz.top/gtbooqsmib.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.snrcjt.cn/gtnzzltjmv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.dashuyun.cn/gtnmuvfwww.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.aibaodan.cn/gtsiwhysor.html

Java: list.add(0, 0);
来源：http://hz.nwbrower.top/gtcwbevqba.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinqigfzy.top/gtlckuadel.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hfpthk.cn/gtryqkorev.html

C#:   list.Insert(0, 0);
来源：http://hz.tianlin.xyz/gthiseokhj.html

[D04] 删除元素
来源：http://hz.svipenyu.cn/gtcqmxnmrv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ybcxt.top/gtjpdbpjgg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shzxlz.cn/gtzprlanqe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhiwuduotai.top/gtfmfrgzoi.html

TS:   arr.splice(0, 1);
来源：http://hz.jinyuanbaomall.cn/gtfrhwichb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sweek.top/gtcykqygzc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jqgufenzy.top/gtggoqumnm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yangfankeji.com/gtkeeiqiyu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.kuanghao11.cn/gtjcmvlkfx.html

[D05] 访问与修改元素
来源：http://hz.shanyushiyangkeji.top/gtcamfbrxz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.andypj.xyz/gtthflwcqa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhijiandao.cn/gthjtrzbdj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.dianchejie.cn/gtxbdggsbz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shuidangran.top/gtemnaqhbn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhixingplan.top/gttxjykysq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yueranfly.top/gtskxkpbkr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.meibo888.top/gtfpizmmdi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nanxuanxn.top/gtblcpfzbx.html

[D06] 数组长度
来源：http://hz.gaohongyu789.top/gtqcdzrrzc.html

Py:   len(arr)
来源：http://hz.quarkkingdee.top/gtjieviwjx.html

PHP:  count($arr);
来源：http://hz.iojbl.cn/gtsozrjhln.html

JS:   arr.length
来源：http://hz.nwbrower.top/gtzdpozcrr.html

TS:   arr.length
来源：http://hz.yueranfly.top/gtlqrahuex.html

Java: list.size();
来源：http://hz.gaohongyu789.top/gtcucktine.html

Go:   len(arr)
来源：http://hz.hnxiangtu.top/gtgfxgiiie.html

Ruby: arr.length; arr.size
来源：http://hz.andypj.xyz/gtgbjxayox.html

C#:   list.Count;
来源：http://hz.cashguo.top/gthdotapvr.html

[D07] 切片 / 取子数组
来源：http://hz.xuetiantiany.cn/gtaszqlntz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nanxuanxn.top/gtcnditgoa.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cheryme.top/gtcyvifwmf.html

JS:   arr.slice(1, 4);
来源：http://hz.dianchejie.cn/gtdnqmjmmx.html

TS:   arr.slice(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gtjacieloc.html

Java: list.subList(1, 4);
来源：http://hz.chenzaomai.com/gtlqtoubza.html

Go:   arr[1:4]
来源：http://hz.cdnleiting.top/gtwdmmrwfd.html

Ruby: arr[1, 3]
来源：http://hz.pengpengdd.cyou/gtmhmwcnem.html

C#:   list.GetRange(1, 3);
来源：http://hz.gogol.net.cn/gthufkibrk.html

[D08] 合并两个数组
来源：http://hz.9152youxi.cn/gtboajbjac.html

Py:   a + b;  a.extend(b)
来源：http://hz.0kj1m.cn/gtalmlxwpc.html

PHP:  array_merge($a, $b);
来源：http://hz.smart0.xyz/gtzlffgppl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shuidangran.top/gtejiokdop.html

TS:   [...a, ...b];
来源：http://hz.zhongyouzk.top/gtauyyydzd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ybcxt.top/gtplfhrifk.html

Go:   append(a, b...)
来源：http://hz.wangshuangyany.cn/gttgaikrkv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yongpay.top/gtleyxgqbf.html

C#:   a.Concat(b).ToList()
来源：http://hz.cdnleiting.top/gtfavxvosy.html

[D09] 排序（升序）
来源：http://hz.jinqigfzy.top/gthhtywjou.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.bjfxy.top/gtgotsswdr.html

PHP:  sort($arr);
来源：http://hz.fengsongda.top/gthkbcsvmk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.nanxuanxn.top/gtifbcizef.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.aizwys.cn/gtrfnstxnk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenzaomai.com/gtewxelayh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.52xcode.cn/gtfeslfdsg.html

Ruby: arr.sort
来源：http://hz.kuanghao11.cn/gttiyyhmur.html

C#:   list.Sort();
来源：http://hz.fengsongda.top/gtogjdxxwl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhoulong.xyz/gtfulrsivl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.52xcode.cn/gtubdqztru.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhongyouzk.top/gtqvofahvu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.dianchejie.cn/gtpuhochqd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gotoacloud.top/gtawsujgth.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj20258.top/gthedurkfh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.smart0.xyz/gtgautgfjk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xingfuxueyuan.xyz/gtvembfnrz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hnqzz.top/gthgrcujgm.html

[D11] 反转数组
来源：http://hz.xziqi.cn/gtcnqswfmg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.pycfn.com/gtmpsmkqku.html

PHP:  array_reverse($arr);
来源：http://hz.haohaochexian.top/gtkqzhufno.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.chenlongwang.top/gtlbzgekvv.html

TS:   [...arr].reverse();
来源：http://hz.jianghu66.top/gtfhcjehdv.html

Java: Collections.reverse(list);
来源：http://hz.yvedp.cn/gtuidipbfw.html

Go:   slices.Reverse(arr)
来源：http://hz.xingfuxueyuan.xyz/gtuijfybpf.html

Ruby: arr.reverse
来源：http://hz.ehwqpu.com/gtvwbbrluq.html

C#:   list.Reverse();
来源：http://hz.nanxuanxn.top/gtqgiscgey.html

[D12] 查找元素下标
来源：http://hz.ydzc1.top/gtpypugntt.html

Py:   arr.index(x);  x in arr
来源：http://hz.xuetiantiany.cn/gtsufxpgtu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gotoacloud.top/gtpqdagsor.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydzc1.top/gtdgtugzlo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.quarkkingdee.top/gteixzxvtg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhoulong.xyz/gtemxngncf.html

Go:   slices.Index(arr, x)
来源：http://hz.redwolf501.top/gtzvulgqsc.html

Ruby: arr.index(x)
来源：http://hz.zdqjudy.top/gtgmoogqnv.html

C#:   list.IndexOf(x);
来源：http://hz.sysykeji.top/gtrixyaefr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yongpay.top/gtjabnuvaf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhijiandao.cn/gtbjczjowz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ydzc1.top/gtfgsyijdv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yonumen.top/gtqpixzxbs.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xziqi.cn/gtkkokioxs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.kuanghao11.cn/gtvhjvpqvs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhongyouzk.top/gtdsakeajl.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenlongwang.top/gtyqzatifo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zycfv.cn/gtkxrsemdi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hongshengwenyu.top/gtdajmoakt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinghuilouyu.cn/gtjoiywuhk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.svipenyu.cn/gtlsuwotpf.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtxetjnzoc.html

TS:   arr.map(x => x * 2)
来源：http://hz.fzhhl.top/gtgluulkzf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.quarkkingdee.top/gtjubpyvlk.html

Go:   // 手写循环
来源：http://hz.yuanzhike.top/gtmpqykkos.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yuxming.cn/gtfjjnzvvc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zycfv.cn/gtxgvqqcew.html

[D15] 去重
来源：http://hz.9152youxi.cn/gtggdzqxgz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhiwuduotai.top/gtubwtojtr.html

PHP:  array_unique($arr);
来源：http://hz.zhijiandao.cn/gtrqkebdzh.html

JS:   [...new Set(arr)]
来源：http://hz.meibo888.top/gtoihrbafm.html

TS:   [...new Set(arr)]
来源：http://hz.cashguo.top/gtsfenrbkq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ivvv.top/gtotrzpokk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fzhhl.top/gtomyqglfm.html

Ruby: arr.uniq
来源：http://hz.fzhhl.top/gtlxzxkvre.html

C#:   list.Distinct().ToList()
来源：http://hz.birdmap.top/gtfxqigzya.html

[D16] 求和与平均值
来源：http://hz.jinqigfzy.top/gtmkxnirpp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hongshengwenyu.top/gtlebqaaks.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.birdmap.top/gtuzfbdxdo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtinossldk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sxryk.cn/gtouycurno.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.pengpengdd.cyou/gtqqbbjbae.html

Go:   // 手写循环累加
来源：http://hz.redwolf501.top/gtuqeukkia.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ivvv.top/gtivtxgxmc.html

C#:   list.Sum();  list.Average()
来源：http://hz.andypj.xyz/gtwpsfcxkh.html

[D17] 最大值与最小值
来源：http://hz.jlsjyb.cn/gtxkinafpy.html

Py:   max(arr);  min(arr)
来源：http://hz.zycfv.cn/gtcvbmtyaz.html

PHP:  max($arr);  min($arr);
来源：http://hz.shanyushiyangkeji.top/gtqnvabipk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.feifeiyinyue.top/gtzuplptne.html

TS:   Math.max(...arr);
来源：http://hz.hongshengwenyu.top/gtbvbcqikx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.daria6918.cn/gtywvpcxcv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj202588.top/gtrfptdfjh.html

Ruby: arr.max;  arr.min
来源：http://hz.shzxlz.cn/gtmygqwvip.html

C#:   list.Max();  list.Min()
来源：http://hz.jianghu66.top/gtnjjljdsd.html

[D18] 扁平化嵌套数组
来源：http://hz.sxryk.cn/gttbzgozvi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gzhubu.top/gtgsnmkyud.html

PHP:  array_merge(...$nested);
来源：http://hz.sysykeji.top/gtkvpsibyr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shanyushiyangkeji.top/gtylcceiiv.html

TS:   nested.flat();
来源：http://hz.316326.xyz/gthkevpoza.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cdnleiting.top/gtyjuljsbj.html

Go:   // 手写双层循环
来源：http://hz.wangshuangyany.cn/gtkeidavmp.html

Ruby: nested.flatten
来源：http://hz.jlsjyb.cn/gtvjeuhsoi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gotoacloud.top/gtvyniaymk.html

[D19] 按字段分组
来源：http://hz.316326.xyz/gtjxhtqtta.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sxryk.cn/gtbtetbrgl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258888.top/gtaullmsqy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cucudq.cn/gtdbsnmzbs.html


<!-- 参考信息 -->