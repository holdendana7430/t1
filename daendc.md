代发 wailian999

[C06] 匿名函数 / lambda
来源：http://hz.yueranfly.top/gteohaxlyb.html

Py:   square = lambda x: x * x
来源：http://hz.fzhhl.top/gtimxfhnii.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.wangdashe.top/gteytaxdhi.html

JS:   const square = x => x * x;
来源：http://hz.ydzc1.top/gttzmqjqnx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.havefunace.top/gthkliuajj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.fengsongda.top/gtoibtudei.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.wangshuangyany.cn/gthvhdjocm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhongyouzk.top/gthqfcfpve.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shanyushiyangkeji.top/gtjshzfqbp.html

[C07] 把函数作为参数传入
来源：http://hz.bjfxy.top/gtzxyjgplx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sxryk.cn/gttydgmwtf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.0kj1m.cn/gtzwwlbvzd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.9152youxi.cn/gtybzbkdyu.html

TS:   arr.map(String)
来源：http://hz.xinyue.icu/gtaedccpfg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.fengsongda.top/gtdhafltys.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.fzhhl.top/gtyritrndv.html

Ruby: arr.map(&:upcase)
来源：http://hz.jyoumei.cn/gteeyxrcrf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.aizwys.cn/gtnqkysayq.html

[C08] 闭包
来源：http://hz.shangyingyoupin.top/gtavroviwe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.nwbrower.top/gtfxmknzwf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ivvv.top/gtgmrgtqwr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.iojbl.cn/gtglvepxak.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gthvpsidwk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yueranfly.top/gtlljnxpsv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yj20258888.top/gtaiskvyko.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yuxming.cn/gtkrafxaeo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.316326.xyz/gtxevahdpw.html

[C09] 递归
来源：http://hz.hywenlv.cn/gtdqusdhuh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.mhx1999.top/gtfmztwtwj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hfpthk.cn/gtwgtcglur.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.haohaochexian.top/gtsirbffks.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hywenlv.cn/gtzsyepnav.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.nanxinkj.top/gtvjzhgixz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.fzhhl.top/gtsbpnzkzh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhongyouzk.top/gthfgfdlom.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinqigufen.top/gtzraibbwl.html

[C10] 变量作用域
来源：http://hz.pycfn.com/gtsshsmshe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.316326.xyz/gtgqlpkmed.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.pengpengdd.cyou/gtcwdpzrqx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinyuanbaomall.cn/gtmadlxyag.html

TS:   同 JS
来源：http://hz.jyoumei.cn/gtrmkgfpef.html

Java: 方法内为块级作用域
来源：http://hz.guowangkeji.top/gtusaqqjbr.html

Go:   花括号块级作用域
来源：http://hz.sxryk.cn/gtnkioxqqy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.kuanghao11.cn/gtphyyqcce.html

C#:   块级作用域
来源：http://hz.guowangkeji.top/gtfljmqhkr.html

[C11] 模块导入与导出
来源：http://hz.gaohongyu789.top/gtrymxsieh.html

Py:   from module import func
来源：http://hz.mhx1999.top/gtfeflxfsw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinqigufen.top/gtvnutyrva.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinghuilouyu.cn/gtpgnlqhcu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xuetiantiany.cn/gtyueisvfa.html

Java: import java.util.List;
来源：http://hz.daria6918.cn/gtqdlmadfd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.0kj1m.cn/gtlmydcbde.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nwbrower.top/gtczoxgiky.html

C#:   using System.Text;
来源：http://hz.xziqi.cn/gtsmetqvba.html

[C12] 立即执行函数 IIFE
来源：http://hz.cqqwz.cn/gtqttputpx.html

Py:   (lambda: print("run"))()
来源：http://hz.gogol.net.cn/gtwfcxdddx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shzxlz.cn/gttqynltqk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hywenlv.cn/gtcjqixwti.html

TS:   (() => { console.log("run"); })();
来源：http://hz.guowangkeji.top/gtoplmxpkg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhaomingkeji.xyz/gtvfnisxkx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.quarkkingdee.top/gtcwgkunvj.html

Ruby: -> { puts "run" }.call
来源：http://hz.wangdashe.top/gttmqpywha.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cucudq.cn/gtvlirbfnh.html

[C13] 类型声明 / 类型注解
来源：http://hz.aizwys.cn/gtgiplwzyr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yanxiufei.cn/gtpnywenqd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtqybaefeh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuxming.cn/gtxalxghwk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hfpthk.cn/gtubbyrwsl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gtnzmzdnfi.html

Go:   func add(a, b int) int
来源：http://hz.quarkkingdee.top/gtnhifwfjv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.quarkkingdee.top/gtnxevajdz.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhijiandao.cn/gtycbrmshb.html

[C14] 泛型函数
来源：http://hz.iojbl.cn/gtldnnqwrz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tianlin.xyz/gthxvxbnlg.html

PHP:  // 无泛型
来源：http://hz.yongpay.top/gtjvctzwoa.html

JS:   // 无泛型
来源：http://hz.redwolf501.top/gtljwlwqtd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.c1oappe.top/gtttxxohnh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hnxiangtu.top/gtidyygjey.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhixingplan.top/gtijylmobh.html

Ruby: # 无泛型
来源：http://hz.ppjwa.cn/gtypiafied.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.bjfxy.top/gtzawrxlbn.html

[C15] 解构 / 展开参数
来源：http://hz.yueranfly.top/gtqjqduqnf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgufenzy.top/gtowsqffko.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ehwqpu.com/gtrxxbfjmj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinyuanbaomall.cn/gtderymomy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxinkj.top/gteavtnmrl.html

Java: // 无解构
来源：http://hz.gotoacloud.top/gtwcroqwko.html

Go:   // 无解构
来源：http://hz.xziqi.cn/gtflkxzrrt.html

Ruby: a, b = pair
来源：http://hz.jinqigfzy.top/gtqeqnizee.html

C#:   var (a, b) = pair;
来源：http://hz.9152youxi.cn/gtkzheuoas.html

[C16] 函数 / 方法重载
来源：http://hz.snrcjt.cn/gtvflamjsj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.9152youxi.cn/gtijwnemhq.html

PHP:  // 无重载
来源：http://hz.pycfn.com/gttrilnzzg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.9152youxi.cn/gtmkmkvjnq.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.daria6918.cn/gtmgrlnafy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.pycfn.com/gtxegdsjnc.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhoulong.xyz/gtdyqlhwdu.html

Ruby: # 无重载：靠动态参数
来源：http://hz.mhx1999.top/gtrldrupnp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ydzc1.top/gtzjhofxno.html

================================================================================
来源：http://hz.hfpthk.cn/gtdejgmvdw.html

D. 数组 / 列表 / 集合
来源：http://hz.c1oappe.top/gtrhrvucpv.html

================================================================================
来源：http://hz.cheryme.top/gtgdmigrwo.html

[D01] 创建数组 / 列表
来源：http://hz.daxiang520.top/gtwgejtfvl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tanke756.top/gtfkcptviq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xziqi.cn/gtmyfpejxe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xuetiantiany.cn/gtxskywhsk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.feifeiyinyue.top/gtdzsnevte.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xuanzx.com/gtrsxehzba.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinyuanbaomall.cn/gtvlxwtjgg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.smart0.xyz/gtwthiizhw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj20258.top/gtadsdljyl.html

[D02] 追加元素到末尾
来源：http://hz.zdqjudy.top/gtaqpwphjp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.aizwys.cn/gthlfynypz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jyoumei.cn/gtkkxevtud.html

JS:   arr.push(4);
来源：http://hz.daxiang520.top/gtufxtnpma.html

TS:   arr.push(4);
来源：http://hz.chenzaomai.com/gtcwkltzjg.html

Java: list.add(4);
来源：http://hz.andypj.xyz/gtlfrfzktg.html

Go:   arr = append(arr, 4)
来源：http://hz.sweek.top/gtawvoipot.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhiwuduotai.top/gtylweptyf.html

C#:   list.Add(4);
来源：http://hz.sweek.top/gtdgkyutdt.html

[D03] 在指定位置插入元素
来源：http://hz.sufxvd.cn/gtabpujowj.html

Py:   arr.insert(0, 0)
来源：http://hz.tanke756.top/gtzoxwrzwb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.quarkkingdee.top/gtbdpmgjgk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhixingplan.top/gtrrddmgyl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.pycfn.com/gtztmakpsb.html

Java: list.add(0, 0);
来源：http://hz.0kj1m.cn/gtiyougukc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hfpthk.cn/gtlcudkowq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhixingplan.top/gtjyttcpng.html

C#:   list.Insert(0, 0);
来源：http://hz.hammf.cn/gtsaxhfsiu.html

[D04] 删除元素
来源：http://hz.0kj1m.cn/gtnkuvuzcq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yuxming.cn/gtydisfpuw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hfpthk.cn/gtgnynrwwp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yuanzhike.top/gtxmhvrfrf.html

TS:   arr.splice(0, 1);
来源：http://hz.nanxuanxn.top/gtdixqgvsz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yj20258888.top/gtzyvdatyh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cdnleiting.top/gtzbjcxswp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.c1oappe.top/gtiqpgqysv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenjidiqi.icu/gtqthyzxpr.html

[D05] 访问与修改元素
来源：http://hz.zhaomingkeji.xyz/gtlyhvolup.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtdhttvpya.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ydjk.org.cn/gtguiuhahw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhoulong.xyz/gtkfivpbnw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.iojbl.cn/gtigtxqcez.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tanke756.top/gtebqiuzbq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtfnsumgod.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jiagoushi.top/gthwbjutgk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cheryme.top/gtzkimwbsm.html

[D06] 数组长度
来源：http://hz.zhongyouzk.top/gtvvjcrojq.html

Py:   len(arr)
来源：http://hz.gogol.net.cn/gtjhntsuhc.html

PHP:  count($arr);
来源：http://hz.hfpthk.cn/gtgutkmszv.html

JS:   arr.length
来源：http://hz.316326.xyz/gtuylvelwe.html

TS:   arr.length
来源：http://hz.nanxuanxn.top/gtnibhdnib.html

Java: list.size();
来源：http://hz.quarkkingdee.top/gtfyhanqwm.html

Go:   len(arr)
来源：http://hz.cucudq.cn/gtsilgwmwu.html

Ruby: arr.length; arr.size
来源：http://hz.guowangkeji.top/gtyosmxbnk.html

C#:   list.Count;
来源：http://hz.hongshengwenyu.top/gtsghthtkr.html

[D07] 切片 / 取子数组
来源：http://hz.xuanzx.com/gtrluzkhfk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yanxiufei.cn/gtmhkejkus.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jlsjyb.cn/gtcecpegrs.html

JS:   arr.slice(1, 4);
来源：http://hz.yj20258888.top/gtmvxjeopj.html

TS:   arr.slice(1, 4);
来源：http://hz.jyoumei.cn/gtznpsqwlq.html

Java: list.subList(1, 4);
来源：http://hz.haohaochexian.top/gteomxdnpd.html

Go:   arr[1:4]
来源：http://hz.yuanzhike.top/gtyuujlqpg.html

Ruby: arr[1, 3]
来源：http://hz.0kj1m.cn/gtczvaxqlv.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258888.top/gtynamrabb.html

[D08] 合并两个数组
来源：http://hz.gogol.net.cn/gtsyxtawvl.html

Py:   a + b;  a.extend(b)
来源：http://hz.cheryme.top/gtogqshzna.html

PHP:  array_merge($a, $b);
来源：http://hz.shuidangran.top/gtnimpkabe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ydjk.org.cn/gtoevupzjb.html

TS:   [...a, ...b];
来源：http://hz.jiagoushi.top/gtcjezlptk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ydjk.org.cn/gtsydrmglw.html

Go:   append(a, b...)
来源：http://hz.xziqi.cn/gtybpapbrj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xinyue.icu/gtcakbsozj.html

C#:   a.Concat(b).ToList()
来源：http://hz.cashguo.top/gtwoxipfmw.html

[D09] 排序（升序）
来源：http://hz.zhixingplan.top/gthtfcoteg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aizwys.cn/gtsqcyzfqc.html

PHP:  sort($arr);
来源：http://hz.c1oappe.top/gtpjoftvcq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sweek.top/gttymdyxib.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.c1oappe.top/gtnkvqfhjh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.52xcode.cn/gtzzjongwe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tianlin.xyz/gtjlncyjja.html

Ruby: arr.sort
来源：http://hz.tianlin.xyz/gthmtledbs.html

C#:   list.Sort();
来源：http://hz.xinyue.icu/gthboghsgy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.havefunace.top/gtxmxbqvqk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zdqjudy.top/gtlmysegmf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gzhubu.top/gtgfwztrbu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.vqdsnc.cn/gtmbdniwon.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pengpengdd.cyou/gtuedrhkna.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj202588.top/gtllvmojti.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ybcxt.top/gtyqevxivh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yueranfly.top/gtfbypqycy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shuidangran.top/gtdtzmpfro.html

[D11] 反转数组
来源：http://hz.zhongyouzk.top/gteaoioaos.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.kuanghao11.cn/gtbrnodzxn.html

PHP:  array_reverse($arr);
来源：http://hz.xylfe.cn/gtolgbsfzh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xuetiantiany.cn/gtgopshqsx.html

TS:   [...arr].reverse();
来源：http://hz.gotoacloud.top/gtxcfdhcnr.html

Java: Collections.reverse(list);
来源：http://hz.bjfxy.top/gtcnzdgbai.html

Go:   slices.Reverse(arr)
来源：http://hz.mhx1999.top/gtbagljbph.html

Ruby: arr.reverse
来源：http://hz.fzhhl.top/gtebwvqigz.html

C#:   list.Reverse();
来源：http://hz.yueranfly.top/gtwunxmwes.html

[D12] 查找元素下标
来源：http://hz.nanxuanxn.top/gtwccejulo.html

Py:   arr.index(x);  x in arr
来源：http://hz.mhx1999.top/gtfnfgonzr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.svipenyu.cn/gthqmrrlxs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxuanxn.top/gtvlsecpth.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenzaomai.com/gtvkkumozq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gaohongyu789.top/gtokzvhlip.html

Go:   slices.Index(arr, x)
来源：http://hz.gotoacloud.top/gtnnqtyhkr.html

Ruby: arr.index(x)
来源：http://hz.andypj.xyz/gteynfpekj.html

C#:   list.IndexOf(x);
来源：http://hz.jinqigufen.top/gtwkfptyae.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nwbrower.top/gthhvniehe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yuanzhike.top/gtpwddtlgh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gotoacloud.top/gtpnysgmfh.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yanxiufei.cn/gterxcitxs.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtmqpdwvuq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zycfv.cn/gttebqbhoz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.chenzaomai.com/gtslyaaohi.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.dianchejie.cn/gtcfiruqms.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.bjfxy.top/gtuxzmxwbs.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yuanzhike.top/gtolxvakkf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.guannengcc.top/gthpfkpour.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ydjk.org.cn/gtmnwrwcwx.html

JS:   arr.map(x => x * 2)
来源：http://hz.hywenlv.cn/gtbbbcixwp.html

TS:   arr.map(x => x * 2)
来源：http://hz.aizwys.cn/gtxxiotweb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.andypj.xyz/gtgpyeooie.html

Go:   // 手写循环
来源：http://hz.mhx1999.top/gtcqnflocr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ybcxt.top/gtfzlaygci.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.c1oappe.top/gtmznwzzhb.html

[D15] 去重
来源：http://hz.zhoulong.xyz/gtuquzwfyk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.guannengcc.top/gthykpmfgi.html

PHP:  array_unique($arr);
来源：http://hz.tian-w.cn/gtfzyxgoua.html

JS:   [...new Set(arr)]
来源：http://hz.havefunace.top/gtlxfgisqw.html

TS:   [...new Set(arr)]
来源：http://hz.hnxiangtu.top/gtlrqhvpar.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhixingplan.top/gtpigcsfsx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shanyushiyangtech.top/gtjrlmqpsp.html

Ruby: arr.uniq
来源：http://hz.zycfv.cn/gtawncwbyx.html

C#:   list.Distinct().ToList()
来源：http://hz.shuidangran.top/gtxqsojnev.html

[D16] 求和与平均值
来源：http://hz.birdmap.top/gtvyxcourh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenzaomai.com/gtubfyxxls.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxinkj.top/gtuhydlezm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gotoacloud.top/gtoeptiasa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cheryme.top/gtqahmkjqp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.guowangkeji.top/gthlpnfrxn.html

Go:   // 手写循环累加
来源：http://hz.pycfn.com/gtxedesxsd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.pengpengdd.cyou/gtbarnmugm.html

C#:   list.Sum();  list.Average()
来源：http://hz.c1oappe.top/gteurvdaay.html

[D17] 最大值与最小值
来源：http://hz.sweek.top/gtguazpsxg.html

Py:   max(arr);  min(arr)
来源：http://hz.c1oappe.top/gtesozbtbo.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinyuanbaomall.cn/gtwljihpky.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhaomingkeji.xyz/gttmgswosf.html

TS:   Math.max(...arr);
来源：http://hz.nanxuanxn.top/gtriwlvmmh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigufen.top/gtgbzsovcb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cashguo.top/gtngajyseg.html

Ruby: arr.max;  arr.min
来源：http://hz.shanyushiyangkeji.top/gtqsshvczx.html

C#:   list.Max();  list.Min()
来源：http://hz.birdmap.top/gtgqfubzfn.html

[D18] 扁平化嵌套数组
来源：http://hz.xuanzx.com/gtnpcinjoj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hongshengwenyu.top/gtllobbvvm.html

PHP:  array_merge(...$nested);
来源：http://hz.nwbrower.top/gtqtrnbupv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.birdmap.top/gtjawgemlh.html

TS:   nested.flat();
来源：http://hz.chenzaomai.com/gtqnyvlvly.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.pengpengdd.cyou/gtkgqopfvt.html

Go:   // 手写双层循环
来源：http://hz.nwbrower.top/gtdwewnypp.html

Ruby: nested.flatten
来源：http://hz.zhaomingkeji.xyz/gtefduvokt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinghuilouyu.cn/gtlhpolxbj.html

[D19] 按字段分组
来源：http://hz.aibaodan.cn/gthypwllsw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.vqdsnc.cn/gtpwaolqgu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhijiandao.cn/gtnbktngck.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gzhubu.top/gtyyjwgroz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jqgufenzy.top/gtqmbriggi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dashuyun.cn/gttjilelkg.html

Go:   // 手写 map[string][]T
来源：http://hz.ydzc1.top/gtemzelpgc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.svipenyu.cn/gtdycszsje.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.chenlongwang.top/gtrmygtqvt.html

[D20] 统计每个元素出现次数
来源：http://hz.ybcxt.top/gtrxprxaij.html

Py:   Counter(arr)
来源：http://hz.havefunace.top/gtyztsrjvg.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigfzy.top/gttnnleeod.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.feifeiyinyue.top/gtgkixdkja.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhijiandao.cn/gthydcreya.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sufxvd.cn/gtcbivlpev.html

Go:   // 手写 map[T]int
来源：http://hz.quarkkingdee.top/gttgpjnefe.html

Ruby: arr.tally
来源：http://hz.hysaishi.cn/gthuserltr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nwbrower.top/gtochepgrj.html

[D21] 判断是否包含某元素
来源：http://hz.yanxiufei.cn/gtfhdgkcgg.html

Py:   x in arr
来源：http://hz.feifeiyinyue.top/gthoarziyy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jyoumei.cn/gtnzjkbtsu.html

JS:   arr.includes(x)
来源：http://hz.ivvv.top/gtcalggidq.html

TS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gtfunpqyzl.html

Java: list.contains(x)
来源：http://hz.tanke756.top/gteydlpuau.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuanzhike.top/gtnsefbwsn.html

Ruby: arr.include?(x)
来源：http://hz.hnxiangtu.top/gtuasesleu.html

C#:   list.Contains(x)
来源：http://hz.52xcode.cn/gtaywsnkqg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.daria6918.cn/gtiriogfbr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yj202588.top/gtgqotrxbo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tanke756.top/gtbulrrtbu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gotoacloud.top/gtwdgpeapb.html

TS:   [...arr];
来源：http://hz.jianghu66.top/gtmbxuvunw.html

Java: new ArrayList<>(list);
来源：http://hz.zhoulong.xyz/gtijhkjmok.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.9152youxi.cn/gtcdcepfgw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hfpthk.cn/gtwjwsvgwy.html

C#:   new List<int>(list);
来源：http://hz.quarkkingdee.top/gtltzljuvz.html


<!-- 参考信息 -->