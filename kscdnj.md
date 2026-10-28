代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.tianlin.xyz/gtaqseycqt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.fzhhl.top/gtvctqkvof.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sweek.top/gtymaaeqzs.html

[C09] 递归
来源：http://hz.smart0.xyz/gtwkketlks.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cashguo.top/gtnxmiffxy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhongyouzk.top/gtylwrdbks.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuetiantiany.cn/gtlyhmkelv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gzhubu.top/gteyysaupb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhongyouzk.top/gtuesxjyyz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.andypj.xyz/gtjlakvgye.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tanke756.top/gtzipbmvro.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.daria6918.cn/gtapapfasf.html

[C10] 变量作用域
来源：http://hz.dianchejie.cn/gtkvvacdkc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hywenlv.cn/gtyggjpfzi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ehwqpu.com/gtqwrtpuyu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cheryme.top/gtbsyhopgo.html

TS:   同 JS
来源：http://hz.wangdashe.top/gtadsfekez.html

Java: 方法内为块级作用域
来源：http://hz.guannengcc.top/gtadhcpxbw.html

Go:   花括号块级作用域
来源：http://hz.snrcjt.cn/gtnqdieleo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jianghu66.top/gtibuukegh.html

C#:   块级作用域
来源：http://hz.yonumen.top/gtiaykiqpi.html

[C11] 模块导入与导出
来源：http://hz.chenjidiqi.icu/gtktfrdsyk.html

Py:   from module import func
来源：http://hz.c1oappe.top/gtktxsxcqy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.guannengcc.top/gtgtqdubtc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yvedp.cn/gtxzxlnjyp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gotoacloud.top/gtxadjqltp.html

Java: import java.util.List;
来源：http://hz.ivvv.top/gtentrxvjb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhixingplan.top/gttqctkcta.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.bjfxy.top/gtkmrtxygi.html

C#:   using System.Text;
来源：http://hz.smart0.xyz/gtcndfpzzb.html

[C12] 立即执行函数 IIFE
来源：http://hz.yonumen.top/gtzgsnxzbl.html

Py:   (lambda: print("run"))()
来源：http://hz.aizwys.cn/gthebosbff.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhiwuduotai.top/gtaijafokx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.aizwys.cn/gtjfzuzxik.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhixingplan.top/gtnriyxsvp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ppjwa.cn/gtewiccgnk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sufxvd.cn/gtwprvhvgv.html

Ruby: -> { puts "run" }.call
来源：http://hz.ppjwa.cn/gtmnpgxcqo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ywan-chungtsiang.top/gtoyfagiuy.html

[C13] 类型声明 / 类型注解
来源：http://hz.havefunace.top/gtqmkwxroc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.daria6918.cn/gtdhphcuyz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangdashe.top/gtovcwhvlk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ybcxt.top/gtofknajwa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hfpthk.cn/gtdpdspgmf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.c1oappe.top/gtjwsftkqx.html

Go:   func add(a, b int) int
来源：http://hz.redwolf501.top/gtsqtcxwfb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.bjfxy.top/gtkbyvoxqb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.aizwys.cn/gtqtijbvvk.html

[C14] 泛型函数
来源：http://hz.quarkkingdee.top/gtfuapyhzp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinqigufen.top/gtvjtszdbu.html

PHP:  // 无泛型
来源：http://hz.yj20258.top/gtmnjjrgro.html

JS:   // 无泛型
来源：http://hz.pycfn.com/gtfpopknvg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.andypj.xyz/gteecywvln.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gogol.net.cn/gtqgkjdrwf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.meibo888.top/gtcowyhmdz.html

Ruby: # 无泛型
来源：http://hz.yj20258888.top/gtluervfqm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zdqjudy.top/gttntlaydb.html

[C15] 解构 / 展开参数
来源：http://hz.sweek.top/gtlwlatwhx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.feifeiyinyue.top/gtdadlpwqb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.guannengcc.top/gtcsvurjdf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.52xcode.cn/gtqsujimpe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.sufxvd.cn/gtbdjrrrdm.html

Java: // 无解构
来源：http://hz.sysykeji.top/gtwodcflyj.html

Go:   // 无解构
来源：http://hz.wangshuangyany.cn/gtgcxtlvnr.html

Ruby: a, b = pair
来源：http://hz.316326.xyz/gtvkyxofyx.html

C#:   var (a, b) = pair;
来源：http://hz.yuanzhike.top/gtvsrkyrag.html

[C16] 函数 / 方法重载
来源：http://hz.aibaodan.cn/gtoqvybuto.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yongpay.top/gtydbssvyb.html

PHP:  // 无重载
来源：http://hz.shuidangran.top/gtjkxitfmk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hywenlv.cn/gtmhuunoex.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258888.top/gtdjvnyqzr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hywenlv.cn/gtfvhhbagu.html

Go:   // 无重载：用不同函数名
来源：http://hz.xuanzx.com/gtghjefbqb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.havefunace.top/gtxkjraxyn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ehwqpu.com/gtavzurarn.html

================================================================================
来源：http://hz.andypj.xyz/gtoggimqtg.html

D. 数组 / 列表 / 集合
来源：http://hz.hongshengwenyu.top/gtmqcvxlew.html

================================================================================
来源：http://hz.mhx1999.top/gterzphxoi.html

[D01] 创建数组 / 列表
来源：http://hz.hywenlv.cn/gtvgkpqklx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hfpthk.cn/gtvwhfrhkc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shuidangran.top/gtsulzujbn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sxryk.cn/gtdvarqopz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.bjfxy.top/gtmqsravol.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.52xcode.cn/gtklokbsmn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.andypj.xyz/gtsybwnjws.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yangfankeji.com/gtmpbkjipy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhijiandao.cn/gtvpxvywcd.html

[D02] 追加元素到末尾
来源：http://hz.ppjwa.cn/gthfvxvbyk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hongshengwenyu.top/gtlmikbfhy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.aibaodan.cn/gtckgqrgve.html

JS:   arr.push(4);
来源：http://hz.yueranfly.top/gthbsymdpr.html

TS:   arr.push(4);
来源：http://hz.zdqjudy.top/gtiomntzzv.html

Java: list.add(4);
来源：http://hz.gzhubu.top/gttxinpwcf.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxuanxn.top/gtstgdsurf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.havefunace.top/gtxpvyqwci.html

C#:   list.Add(4);
来源：http://hz.jinghuilouyu.cn/gteezclato.html

[D03] 在指定位置插入元素
来源：http://hz.cheryme.top/gtpnkneogn.html

Py:   arr.insert(0, 0)
来源：http://hz.nwbrower.top/gtambbugum.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.mhx1999.top/gtchgbnrbs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ehwqpu.com/gtbuvavivs.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cashguo.top/gtecdplyvu.html

Java: list.add(0, 0);
来源：http://hz.gotoacloud.top/gtndwvrwub.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.guowangkeji.top/gthtnqnxld.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.vqdsnc.cn/gtzlxxjeas.html

C#:   list.Insert(0, 0);
来源：http://hz.ivvv.top/gthublruax.html

[D04] 删除元素
来源：http://hz.jinyuanbaomall.cn/gtbavnakkt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cdnleiting.top/gtucvpkglu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.316326.xyz/gtxdpnnyzu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenlongwang.top/gtqnnorobj.html

TS:   arr.splice(0, 1);
来源：http://hz.shzxlz.cn/gtiohryiir.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.aizwys.cn/gturgwblcv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sweek.top/gtgmsxcyyd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.andypj.xyz/gtktyvarme.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.9152youxi.cn/gtjgqetbxu.html

[D05] 访问与修改元素
来源：http://hz.yj20258.top/gtruonkymj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daria6918.cn/gtbhldzgmm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jiagoushi.top/gtgcoallzq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xylfe.cn/gtrcksazcb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ydjk.org.cn/gtttwfvysc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xylfe.cn/gteynpxlzn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtodoxkgtu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xinyue.icu/gthyoidirq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yangfankeji.com/gtqtymqoda.html

[D06] 数组长度
来源：http://hz.ybcxt.top/gtautwtzbt.html

Py:   len(arr)
来源：http://hz.yj202588.top/gtuzdoqxrd.html

PHP:  count($arr);
来源：http://hz.hfpthk.cn/gtalhrqcmq.html

JS:   arr.length
来源：http://hz.gogol.net.cn/gtuwyavcby.html

TS:   arr.length
来源：http://hz.zhongyouzk.top/gtbrzihosq.html

Java: list.size();
来源：http://hz.zhoulong.xyz/gtreuvlugh.html

Go:   len(arr)
来源：http://hz.yuanzhike.top/gtvbglfvyt.html

Ruby: arr.length; arr.size
来源：http://hz.birdmap.top/gtrlrecwgx.html

C#:   list.Count;
来源：http://hz.cucudq.cn/gteiccozrc.html

[D07] 切片 / 取子数组
来源：http://hz.jiagoushi.top/gtnglyqrws.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yueranfly.top/gtgrpyvvvw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhongyouzk.top/gtycjhwmkg.html

JS:   arr.slice(1, 4);
来源：http://hz.haohaochexian.top/gtignykucx.html

TS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gtxjympbvd.html

Java: list.subList(1, 4);
来源：http://hz.quarkkingdee.top/gtvhvhinlk.html

Go:   arr[1:4]
来源：http://hz.birdmap.top/gtgfmsjajq.html

Ruby: arr[1, 3]
来源：http://hz.jinyuanbaomall.cn/gthpegyxto.html

C#:   list.GetRange(1, 3);
来源：http://hz.yuanzhike.top/gtubvjzbda.html

[D08] 合并两个数组
来源：http://hz.shuidangran.top/gtcmgrptbs.html

Py:   a + b;  a.extend(b)
来源：http://hz.9152youxi.cn/gtokwglhww.html

PHP:  array_merge($a, $b);
来源：http://hz.jinqigfzy.top/gtsrmlotaz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jianghu66.top/gtdshopuvp.html

TS:   [...a, ...b];
来源：http://hz.yongpay.top/gtmgrrnsrx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yongpay.top/gtkqqspape.html

Go:   append(a, b...)
来源：http://hz.gzhubu.top/gtapnimcce.html

Ruby: a + b;  a.concat(b)
来源：http://hz.snrcjt.cn/gtuewhrjxt.html

C#:   a.Concat(b).ToList()
来源：http://hz.andypj.xyz/gtlgcnjcpk.html

[D09] 排序（升序）
来源：http://hz.52xcode.cn/gtyxiopgwf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtaefpwuoq.html

PHP:  sort($arr);
来源：http://hz.dashuyun.cn/gtsegzknmo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj20258.top/gtqoromkhh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yuxming.cn/gtfninowud.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj20258.top/gtnaqwtyiw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yvedp.cn/gtuhjzoequ.html

Ruby: arr.sort
来源：http://hz.iojbl.cn/gtltiavlpu.html

C#:   list.Sort();
来源：http://hz.gotoacloud.top/gtgpaorlcp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jqgufenzy.top/gtpnhjrofu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.snrcjt.cn/gtskhvaupk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gtwwttruul.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangkeji.top/gtfvgmtlui.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sweek.top/gtxarzhfqd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj20258.top/gtftfxiaqi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.haohaochexian.top/gtldrxwiuu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yonumen.top/gtzfiqrens.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.mhx1999.top/gtudickgbs.html

[D11] 反转数组
来源：http://hz.zycfv.cn/gtywkbjnod.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhongyouzk.top/gtxbjpwqhr.html

PHP:  array_reverse($arr);
来源：http://hz.wangshuangyany.cn/gtktqnjpnh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhengqikj.top/gtgbjyfpmg.html

TS:   [...arr].reverse();
来源：http://hz.yuanzhike.top/gtdelqzhga.html

Java: Collections.reverse(list);
来源：http://hz.nwbrower.top/gtbdbdipae.html

Go:   slices.Reverse(arr)
来源：http://hz.hnxiangtu.top/gtjplqijph.html

Ruby: arr.reverse
来源：http://hz.yuxming.cn/gtiyapanbd.html

C#:   list.Reverse();
来源：http://hz.gogol.net.cn/gtzzzuatjf.html

[D12] 查找元素下标
来源：http://hz.cheryme.top/gtpjcdjtxd.html

Py:   arr.index(x);  x in arr
来源：http://hz.ivvv.top/gtjghwmruf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgufenzy.top/gtyeejuqfx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shangyingyoupin.top/gtmstesrbu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xinyue.icu/gtiipvfcsd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jqgfzy.top/gtwcabxffo.html

Go:   slices.Index(arr, x)
来源：http://hz.zdqjudy.top/gtddvsjvpm.html

Ruby: arr.index(x)
来源：http://hz.zdqjudy.top/gtgcvedoou.html

C#:   list.IndexOf(x);
来源：http://hz.jqgufenzy.top/gtsulkaslj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.wangdashe.top/gtcedstwrg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.smart0.xyz/gtsdkiejdk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xylfe.cn/gtxajurxpp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gtxrgcnvvi.html

TS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gtylplwoji.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zycfv.cn/gtyczaraex.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hysaishi.cn/gtdjipbopr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenlongwang.top/gtdprtxwoy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.bjfxy.top/gtisydveff.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jqgufenzy.top/gtnqlhnyhx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ivvv.top/gtqxobvagi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ywan-chungtsiang.top/gtehcgozvo.html

JS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtmfdhxkjc.html

TS:   arr.map(x => x * 2)
来源：http://hz.snrcjt.cn/gtqpawxuzv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.iojbl.cn/gtdumykkgk.html

Go:   // 手写循环
来源：http://hz.aibaodan.cn/gtpuznmrag.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.0kj1m.cn/gtawwwqfqa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jlsjyb.cn/gtrjiqnufx.html

[D15] 去重
来源：http://hz.ppjwa.cn/gthtekboov.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yongpay.top/gtiwlztijl.html

PHP:  array_unique($arr);
来源：http://hz.0kj1m.cn/gtzjdgicdw.html

JS:   [...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gtyigxxjzj.html

TS:   [...new Set(arr)]
来源：http://hz.andypj.xyz/gtyiwcxvid.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.birdmap.top/gtnlqvzxqj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinqigufen.top/gtsugsumqc.html

Ruby: arr.uniq
来源：http://hz.chenzaomai.com/gtbvyodwnt.html

C#:   list.Distinct().ToList()
来源：http://hz.xuanzx.com/gteepqjtlx.html

[D16] 求和与平均值
来源：http://hz.ydjk.org.cn/gtsgulallt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cqqwz.cn/gtneqhwuqv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinyuanbaomall.cn/gtdocqpnfv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sxryk.cn/gtfjovmsij.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hammf.cn/gtjfvzztgt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenjidiqi.icu/gtlhmqrcyz.html

Go:   // 手写循环累加
来源：http://hz.zhengqikj.top/gtbvejhink.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xuanzx.com/gtarjsdbpn.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj202588.top/gtaxpngnju.html

[D17] 最大值与最小值
来源：http://hz.zhengqikj.top/gtqhtpjfax.html

Py:   max(arr);  min(arr)
来源：http://hz.cucudq.cn/gtmqwfzxlm.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenlongwang.top/gtcnnxfelk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ywan-chungtsiang.top/gtfcrpvgnu.html

TS:   Math.max(...arr);
来源：http://hz.zhixingplan.top/gtpdddkvvl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.redwolf501.top/gtzukvunbh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.birdmap.top/gtftrhwpdy.html

Ruby: arr.max;  arr.min
来源：http://hz.ydzc1.top/gtcgjpwltm.html

C#:   list.Max();  list.Min()
来源：http://hz.yj20258.top/gtydbonnox.html

[D18] 扁平化嵌套数组
来源：http://hz.jlsjyb.cn/gturwoaicc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shuidangran.top/gttevuxftw.html

PHP:  array_merge(...$nested);
来源：http://hz.meibo888.top/gtczdhmhro.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.birdmap.top/gtlhrgymlx.html

TS:   nested.flat();
来源：http://hz.meibo888.top/gtjystjjpg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.fzhhl.top/gtkdwnwrbe.html

Go:   // 手写双层循环
来源：http://hz.ydzc1.top/gtoziljwgm.html

Ruby: nested.flatten
来源：http://hz.kuanghao11.cn/gtiswevkot.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cqqwz.cn/gtkmqfgxww.html

[D19] 按字段分组
来源：http://hz.0kj1m.cn/gtfvstvdqg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cheryme.top/gtkfadhpvq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.kuanghao11.cn/gtdofavhmq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gotoacloud.top/gtnlrjlusa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.haohaochexian.top/gtbueadeqi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.andypj.xyz/gtciowznab.html

Go:   // 手写 map[string][]T
来源：http://hz.jyoumei.cn/gtwhcuovbs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.9152youxi.cn/gttdgwqulr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.dianchejie.cn/gtirzszlmy.html

[D20] 统计每个元素出现次数
来源：http://hz.jyoumei.cn/gtsyfdlksa.html

Py:   Counter(arr)
来源：http://hz.shangyingyoupin.top/gttqnpvcct.html

PHP:  array_count_values($arr);
来源：http://hz.hammf.cn/gtwqwqwiar.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangdashe.top/gtbjgwapsw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cucudq.cn/gtklkcslmc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zdqjudy.top/gtbzxpaqgd.html

Go:   // 手写 map[T]int
来源：http://hz.zycfv.cn/gtabbxmxqr.html

Ruby: arr.tally
来源：http://hz.gogol.net.cn/gtjywnpxjh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhongyouzk.top/gtvwtqawbi.html

[D21] 判断是否包含某元素
来源：http://hz.zdqjudy.top/gtaohjlkcy.html

Py:   x in arr
来源：http://hz.cqqwz.cn/gtncnzmmtd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.bjfxy.top/gtzxgmonyz.html

JS:   arr.includes(x)
来源：http://hz.gzhubu.top/gtqsgdxmpw.html

TS:   arr.includes(x)
来源：http://hz.ybcxt.top/gtncnhvsqe.html

Java: list.contains(x)
来源：http://hz.yuxming.cn/gtgdxelfse.html

Go:   slices.Contains(arr, x)
来源：http://hz.tian-w.cn/gtnrcfqufa.html

Ruby: arr.include?(x)
来源：http://hz.ydzc1.top/gtzkaokrdu.html

C#:   list.Contains(x)
来源：http://hz.xinyue.icu/gtijzkokik.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yvedp.cn/gtlheoofav.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shanyushiyangtech.top/gteuxorqrl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aibaodan.cn/gtbuohnpes.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hongshengwenyu.top/gtgxoxhioz.html

TS:   [...arr];
来源：http://hz.pycfn.com/gtcqwfyaik.html

Java: new ArrayList<>(list);
来源：http://hz.shuidangran.top/gtcmpdvhkt.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.mhx1999.top/gtgxjqbubx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenjidiqi.icu/gtrrnfwqys.html

C#:   new List<int>(list);
来源：http://hz.ybcxt.top/gtjkcutthk.html

[D23] reduce 累积计算
来源：http://hz.sysykeji.top/gtffpcuakg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yanxiufei.cn/gtwyzshmvv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yanxiufei.cn/gteibamjwq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangkeji.top/gtzjmfmubz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cheryme.top/gtxrrtxbns.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.snrcjt.cn/gtmznzqmdj.html

Go:   // 手写循环
来源：http://hz.chenlongwang.top/gteiaydukp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenzaomai.com/gtgcjarboo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinghuilouyu.cn/gtyhkaytkg.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxinkj.top/gtofodpdyp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xylfe.cn/gtnavmkvrf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xuanzx.com/gtlumnovnz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.daria6918.cn/gtxgavoqnt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xylfe.cn/gtrihngmll.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hnqzz.top/gtsveribrh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hnxiangtu.top/gtujntdndv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sysykeji.top/gtuujpgfsg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cheryme.top/gthkfihupl.html

[D25] Set 集合去重与交并差
来源：http://hz.hnqzz.top/gtogfrvcik.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhaomingkeji.xyz/gtypmoqyrf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yj20258888.top/gtsoazibbs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhixingplan.top/gtotioitbb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shuidangran.top/gtsmuqkesi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gogol.net.cn/gtyohlqwlp.html


<!-- 参考信息 -->