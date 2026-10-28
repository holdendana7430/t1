代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yueranfly.top/gtsvycxelb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hywenlv.cn/gtbwpwawnz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gotoacloud.top/gtsasnknxb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.fengsongda.top/gtrqaipfln.html

Go:   // 无：用配置结构体参数
来源：http://hz.pengpengdd.cyou/gtegjeefaq.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtsvwjouqo.html

C#:   f(a: 1, b: 2)
来源：http://hz.svipenyu.cn/gtqsycsllu.html

[C05] 返回多个值
来源：http://hz.hywenlv.cn/gtsonsjiiu.html

Py:   return a, b
来源：http://hz.zhongyouzk.top/gtrqqetszb.html

PHP:  return [$a, $b];
来源：http://hz.ivvv.top/gtsurnyybh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hywenlv.cn/gtyafucqdv.html

TS:   return { a, b };
来源：http://hz.yangfankeji.com/gtjoclufiq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhoulong.xyz/gtwhvlgdvb.html

Go:   return a, b
来源：http://hz.jlsjyb.cn/gtploenjin.html

Ruby: return a, b
来源：http://hz.52xcode.cn/gtdghdcfsc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj202588.top/gtqjnklxxm.html

[C06] 匿名函数 / lambda
来源：http://hz.wangdashe.top/gthvymbdbn.html

Py:   square = lambda x: x * x
来源：http://hz.dianchejie.cn/gtsomycucc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shangyingyoupin.top/gthdjnxcsl.html

JS:   const square = x => x * x;
来源：http://hz.cheryme.top/gtlcvixifl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.fzhhl.top/gtqaembnmr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhaomingkeji.xyz/gtpgupsilq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xziqi.cn/gttlgpaiiy.html

Ruby: square = ->(x) { x * x }
来源：http://hz.wangshuangyany.cn/gtggbbnjpk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cdnleiting.top/gtwuzgujrt.html

[C07] 把函数作为参数传入
来源：http://hz.bjfxy.top/gtujnmfnyw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yuanzhike.top/gtahscxskh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guannengcc.top/gtdwobpbdr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.gotoacloud.top/gtwdwyycag.html

TS:   arr.map(String)
来源：http://hz.meibo888.top/gtrgpykfsb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nanxuanxn.top/gtdxefzfnb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cqqwz.cn/gtlmyrtitx.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhongyouzk.top/gtutneypqj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.wangshuangyany.cn/gtaqpayssc.html

[C08] 闭包
来源：http://hz.hongshengwenyu.top/gtgbxqoaqm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.dashuyun.cn/gttpwrcoba.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yuxming.cn/gtchuymffo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yj202588.top/gtfpexkbkb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.fzhhl.top/gtnmffhsod.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.316326.xyz/gtukyvwsvk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hysaishi.cn/gtqwqjmbmr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.gotoacloud.top/gtvxtmmdeg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj20258888.top/gtzvfjjcjt.html

[C09] 递归
来源：http://hz.snrcjt.cn/gttrmnujfy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.aibaodan.cn/gtahmblqyg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.mhx1999.top/gtnvndfduk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnqzz.top/gtgcmfgiux.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhiwuduotai.top/gtsdqhwcso.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hywenlv.cn/gtaxouwuwo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenzaomai.com/gtvpacxjig.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.mhx1999.top/gtnzfkjifd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxinkj.top/gtqiuuotjd.html

[C10] 变量作用域
来源：http://hz.jianghu66.top/gteacebxoo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yvedp.cn/gtixqfoiwf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ppjwa.cn/gtshuyicss.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hywenlv.cn/gtbssiqckw.html

TS:   同 JS
来源：http://hz.haohaochexian.top/gtqdvgnahj.html

Java: 方法内为块级作用域
来源：http://hz.gzhubu.top/gtvebshdif.html

Go:   花括号块级作用域
来源：http://hz.tian-w.cn/gtwufzrsax.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nwbrower.top/gtivkpixwj.html

C#:   块级作用域
来源：http://hz.shangyingyoupin.top/gtxfqkmkqo.html

[C11] 模块导入与导出
来源：http://hz.kuanghao11.cn/gtlskhmoww.html

Py:   from module import func
来源：http://hz.yj202588.top/gtfdxapyqy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cheryme.top/gtvmrshmrf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ydzc1.top/gtwazzfvna.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shangyingyoupin.top/gtplhqlegc.html

Java: import java.util.List;
来源：http://hz.yanxiufei.cn/gtelqcvdxt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ivvv.top/gteymqxrvy.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yanxiufei.cn/gtfpklbolj.html

C#:   using System.Text;
来源：http://hz.jinyuanbaomall.cn/gtwzguqkby.html

[C12] 立即执行函数 IIFE
来源：http://hz.ehwqpu.com/gtviknnxio.html

Py:   (lambda: print("run"))()
来源：http://hz.yj202588.top/gtjikztjwh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yonumen.top/gtvrqpxlos.html

JS:   (() => { console.log("run"); })();
来源：http://hz.wangshuangyany.cn/gtsydknwev.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tianlin.xyz/gtxexipftl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nwbrower.top/gtyvibigem.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.chenlongwang.top/gtipmvxrbf.html

Ruby: -> { puts "run" }.call
来源：http://hz.chenlongwang.top/gticyhywwu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ywan-chungtsiang.top/gtqzyzbpky.html

[C13] 类型声明 / 类型注解
来源：http://hz.sysykeji.top/gtkayizxkx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.bjfxy.top/gtlviyaxnf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuxming.cn/gtjcnaxcli.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.tanke756.top/gtlytfewzp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gotoacloud.top/gteklcnoey.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.dashuyun.cn/gtecpjjtnf.html

Go:   func add(a, b int) int
来源：http://hz.xinyue.icu/gttidycikp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.tianlin.xyz/gtqznepaun.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yuxming.cn/gtmactmjcg.html

[C14] 泛型函数
来源：http://hz.c1oappe.top/gtimrwzqkp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.bjfxy.top/gtyozqnjyr.html

PHP:  // 无泛型
来源：http://hz.yongpay.top/gtshdbyzhh.html

JS:   // 无泛型
来源：http://hz.bjfxy.top/gtrtobfsmx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tian-w.cn/gtvmslyblz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.0kj1m.cn/gtjqzdmvdu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenjidiqi.icu/gtlxfetplk.html

Ruby: # 无泛型
来源：http://hz.tanke756.top/gturxoynzr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.0kj1m.cn/gtvzxwatxc.html

[C15] 解构 / 展开参数
来源：http://hz.316326.xyz/gtcmqnbdyh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cdnleiting.top/gtlylqqwsh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yuanzhike.top/gtxezmiukf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinyuanbaomall.cn/gttcdyyfhn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.meibo888.top/gtudjvxdbq.html

Java: // 无解构
来源：http://hz.zdqjudy.top/gtcstedzic.html

Go:   // 无解构
来源：http://hz.fengsongda.top/gtbbcciygj.html

Ruby: a, b = pair
来源：http://hz.shzxlz.cn/gtpljntpsd.html

C#:   var (a, b) = pair;
来源：http://hz.jqgufenzy.top/gtlowxknmk.html

[C16] 函数 / 方法重载
来源：http://hz.nanxinkj.top/gtuvnptiqe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hnqzz.top/gttqbwvdhw.html

PHP:  // 无重载
来源：http://hz.gotoacloud.top/gtwomppkod.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sxryk.cn/gtkryaahzm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shangyingyoupin.top/gttydpbaxd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xuanzx.com/gtwmbtgpjd.html

Go:   // 无重载：用不同函数名
来源：http://hz.daxiang520.top/gtfbwjuhtn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ybcxt.top/gtgsohsiqj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zdqjudy.top/gtaxrarbet.html

================================================================================
来源：http://hz.yuxming.cn/gtyutmegme.html

D. 数组 / 列表 / 集合
来源：http://hz.pycfn.com/gtjflnoxrk.html

================================================================================
来源：http://hz.meibo888.top/gtdpkqjsll.html

[D01] 创建数组 / 列表
来源：http://hz.jinyuanbaomall.cn/gtzbxyuuag.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ehwqpu.com/gtcffcjdgq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuanzhike.top/gtynqcmpsb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hammf.cn/gtccmdqybq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj202588.top/gthucwlgzp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ppjwa.cn/gtusuzcgbo.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hysaishi.cn/gtrgxdcedy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangtech.top/gtaduwhgzv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.bjfxy.top/gtmhybcdzp.html

[D02] 追加元素到末尾
来源：http://hz.haohaochexian.top/gtzpsbauuz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yj20258888.top/gtucchxyll.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yuxming.cn/gtfjeqszkq.html

JS:   arr.push(4);
来源：http://hz.quarkkingdee.top/gtmplqkihx.html

TS:   arr.push(4);
来源：http://hz.jinghuilouyu.cn/gtbfpacsxa.html

Java: list.add(4);
来源：http://hz.daria6918.cn/gtvloiovdt.html

Go:   arr = append(arr, 4)
来源：http://hz.aizwys.cn/gtyenkpces.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.meibo888.top/gtsqkfywoq.html

C#:   list.Add(4);
来源：http://hz.yj20258888.top/gtkerfrqga.html

[D03] 在指定位置插入元素
来源：http://hz.guannengcc.top/gtjmwqxpmz.html

Py:   arr.insert(0, 0)
来源：http://hz.316326.xyz/gtypeaeqwg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xingfuxueyuan.xyz/gtekaoxale.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yueranfly.top/gtcirngwjf.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.mhx1999.top/gtbhzcufmp.html

Java: list.add(0, 0);
来源：http://hz.hysaishi.cn/gtzgvarcpj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cqqwz.cn/gtvjekjycz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jqgufenzy.top/gtrqottcoe.html

C#:   list.Insert(0, 0);
来源：http://hz.zhijiandao.cn/gtoibeqgew.html

[D04] 删除元素
来源：http://hz.xziqi.cn/gtgszetytb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.nwbrower.top/gtsokhgkgw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenzaomai.com/gtgjmaxqcx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.snrcjt.cn/gtaorssyhp.html

TS:   arr.splice(0, 1);
来源：http://hz.gzhubu.top/gtzcrobdyx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhixingplan.top/gteskpqiee.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gzhubu.top/gtxysepjip.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.haohaochexian.top/gtddntdowg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhaomingkeji.xyz/gtsewcbxhx.html

[D05] 访问与修改元素
来源：http://hz.sweek.top/gtasrixcrc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuanzx.com/gtikvmzphs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xziqi.cn/gtifchvucj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yonumen.top/gtwgiiroqn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.meibo888.top/gtiibjsxpe.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nanxinkj.top/gtkhaqeqqd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtbsqhxdfx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guannengcc.top/gtzslffome.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xuanzx.com/gtcewcyjlk.html

[D06] 数组长度
来源：http://hz.shanyushiyangtech.top/gtludzzgyb.html

Py:   len(arr)
来源：http://hz.feifeiyinyue.top/gtnpfgtyxf.html

PHP:  count($arr);
来源：http://hz.cdnleiting.top/gtdleewmvh.html

JS:   arr.length
来源：http://hz.hnxiangtu.top/gtddfvxpvk.html

TS:   arr.length
来源：http://hz.tian-w.cn/gtwsubtmvw.html

Java: list.size();
来源：http://hz.xingfuxueyuan.xyz/gtnsrkcfha.html

Go:   len(arr)
来源：http://hz.hnqzz.top/gtiozsnsun.html

Ruby: arr.length; arr.size
来源：http://hz.daria6918.cn/gtwoutksbz.html

C#:   list.Count;
来源：http://hz.jianghu66.top/gtdoctyjmb.html

[D07] 切片 / 取子数组
来源：http://hz.andypj.xyz/gtaehcigrb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hfpthk.cn/gthjqjoruc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.c1oappe.top/gturjfgqny.html

JS:   arr.slice(1, 4);
来源：http://hz.wangshuangyany.cn/gtfdkvofgs.html

TS:   arr.slice(1, 4);
来源：http://hz.havefunace.top/gtbkyaehrx.html

Java: list.subList(1, 4);
来源：http://hz.svipenyu.cn/gtmcmijxnf.html

Go:   arr[1:4]
来源：http://hz.xingfuxueyuan.xyz/gtoqsowidr.html

Ruby: arr[1, 3]
来源：http://hz.shanyushiyangkeji.top/gtlqnehtin.html

C#:   list.GetRange(1, 3);
来源：http://hz.meibo888.top/gtgalbjtxu.html

[D08] 合并两个数组
来源：http://hz.andypj.xyz/gtrrnpkkye.html

Py:   a + b;  a.extend(b)
来源：http://hz.wangshuangyany.cn/gtsqbmgxzq.html

PHP:  array_merge($a, $b);
来源：http://hz.yuanzhike.top/gtbymtldbn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ybcxt.top/gtzaehanjh.html

TS:   [...a, ...b];
来源：http://hz.zhixingplan.top/gtrblbvsia.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuanzhike.top/gtnbgbxurh.html

Go:   append(a, b...)
来源：http://hz.fengsongda.top/gtuyjqbzsc.html

Ruby: a + b;  a.concat(b)
来源：http://hz.aibaodan.cn/gtupsfridn.html

C#:   a.Concat(b).ToList()
来源：http://hz.gzhubu.top/gtenhnbcbr.html

[D09] 排序（升序）
来源：http://hz.dashuyun.cn/gtwhgciehh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yanxiufei.cn/gtstovqfiy.html

PHP:  sort($arr);
来源：http://hz.hysaishi.cn/gtahtwnris.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.dianchejie.cn/gtbpgufbxl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.haohaochexian.top/gtkyuneiko.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj202588.top/gtzmekoeec.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yangfankeji.com/gttfzjfmgv.html

Ruby: arr.sort
来源：http://hz.gogol.net.cn/gtwwrnykle.html

C#:   list.Sort();
来源：http://hz.zhiwuduotai.top/gtvscfjfeh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hammf.cn/gtqgcppazy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.iojbl.cn/gtdnqxsmwh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.birdmap.top/gtxroambgo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cucudq.cn/gtcghkxabp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnxiangtu.top/gtemqhqjdo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.wangdashe.top/gtuplihrzh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hnqzz.top/gttvqyfmmc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ivvv.top/gtetqimhwf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.fengsongda.top/gtuzzoexqe.html

[D11] 反转数组
来源：http://hz.gzhubu.top/gthcvqjbvk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ydzc1.top/gtpneqadkp.html

PHP:  array_reverse($arr);
来源：http://hz.meibo888.top/gtxxfehsyj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.smart0.xyz/gtshheeofp.html

TS:   [...arr].reverse();
来源：http://hz.haohaochexian.top/gtcfbakccx.html

Java: Collections.reverse(list);
来源：http://hz.meibo888.top/gtqjvinroa.html

Go:   slices.Reverse(arr)
来源：http://hz.cashguo.top/gtyadnmgmi.html

Ruby: arr.reverse
来源：http://hz.ivvv.top/gtyhoazbcc.html

C#:   list.Reverse();
来源：http://hz.gotoacloud.top/gtucqkpvsw.html

[D12] 查找元素下标
来源：http://hz.chenlongwang.top/gthpyvihnl.html

Py:   arr.index(x);  x in arr
来源：http://hz.xuetiantiany.cn/gtadddybkr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nanxuanxn.top/gtuardjgyt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.vqdsnc.cn/gtmneooytq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtdexdanln.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.snrcjt.cn/gttsidqvjw.html

Go:   slices.Index(arr, x)
来源：http://hz.hysaishi.cn/gtswaijwet.html

Ruby: arr.index(x)
来源：http://hz.xuanzx.com/gtvzlasbro.html

C#:   list.IndexOf(x);
来源：http://hz.haohaochexian.top/gtzrwljmro.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shanyushiyangtech.top/gtuacbgljt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sweek.top/gtluktzmzx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ybcxt.top/gtxxkobuwx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xingfuxueyuan.xyz/gtspcrxxdh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daria6918.cn/gtcoqtxmso.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.aizwys.cn/gtisppyrwk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.tian-w.cn/gtopetilzv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ydjk.org.cn/gtrupptecu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jianghu66.top/gtxgwutaix.html

[D14] 映射转换（每个元素变形）
来源：http://hz.316326.xyz/gtifrxlfhw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.wangshuangyany.cn/gtzqelvsxs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.birdmap.top/gtgxrfrmhc.html

JS:   arr.map(x => x * 2)
来源：http://hz.chenzaomai.com/gtxsaugdpz.html

TS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gtbfcbflcm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinqigfzy.top/gtaqkkziwy.html

Go:   // 手写循环
来源：http://hz.ivvv.top/gthtntjyft.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.0kj1m.cn/gtamjkaceh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gzhubu.top/gttgoivxfm.html

[D15] 去重
来源：http://hz.xingfuxueyuan.xyz/gtkgjhdqls.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.redwolf501.top/gteuexsqjy.html

PHP:  array_unique($arr);
来源：http://hz.dianchejie.cn/gthmwycotg.html

JS:   [...new Set(arr)]
来源：http://hz.sufxvd.cn/gtmosgogjq.html

TS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gtajlndakb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxuanxn.top/gtxcdnsglj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhengqikj.top/gtoqcizeop.html

Ruby: arr.uniq
来源：http://hz.xylfe.cn/gtpsppusxb.html

C#:   list.Distinct().ToList()
来源：http://hz.cashguo.top/gtqdokflcz.html

[D16] 求和与平均值
来源：http://hz.dashuyun.cn/gtoedzlhlu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj202588.top/gtusbumlur.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xinyue.icu/gtwsdqgdtc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jlsjyb.cn/gtzlrincul.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nwbrower.top/gtwfhwrare.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.daria6918.cn/gttjiuwmwr.html

Go:   // 手写循环累加
来源：http://hz.jinghuilouyu.cn/gtsiavjixw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cqqwz.cn/gttthbisei.html

C#:   list.Sum();  list.Average()
来源：http://hz.daxiang520.top/gtmrzqexsl.html

[D17] 最大值与最小值
来源：http://hz.yueranfly.top/gtzipctsyu.html

Py:   max(arr);  min(arr)
来源：http://hz.jinghuilouyu.cn/gtlaizprpq.html

PHP:  max($arr);  min($arr);
来源：http://hz.jlsjyb.cn/gtwpigqgwl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cucudq.cn/gtmmggwmwv.html

TS:   Math.max(...arr);
来源：http://hz.jyoumei.cn/gtvwvirqyu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ydzc1.top/gtssmerath.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jyoumei.cn/gtjwlwyofg.html

Ruby: arr.max;  arr.min
来源：http://hz.tian-w.cn/gtozclohbs.html

C#:   list.Max();  list.Min()
来源：http://hz.redwolf501.top/gtkhldbalt.html

[D18] 扁平化嵌套数组
来源：http://hz.xuanzx.com/gtyudesden.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.iojbl.cn/gttblmfrdu.html

PHP:  array_merge(...$nested);
来源：http://hz.yueranfly.top/gtpwryvisd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.dianchejie.cn/gtcnzdzode.html

TS:   nested.flat();
来源：http://hz.yuxming.cn/gtfurrdlcu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj202588.top/gtufhrnpve.html

Go:   // 手写双层循环
来源：http://hz.cheryme.top/gtegeqidpn.html

Ruby: nested.flatten
来源：http://hz.zhongyouzk.top/gtbnquudzg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xylfe.cn/gtazcpmpts.html

[D19] 按字段分组
来源：http://hz.yuanzhike.top/gtuqwznoql.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhengqikj.top/gtveawxjae.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sweek.top/gtxljuwtbg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhengqikj.top/gtmsrnoqxb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj20258.top/gtqkrrextr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.c1oappe.top/gtbgstytfn.html

Go:   // 手写 map[string][]T
来源：http://hz.9152youxi.cn/gtbpaitrou.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tianlin.xyz/gtrfkrvdad.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.316326.xyz/gtqjbtgvqg.html

[D20] 统计每个元素出现次数
来源：http://hz.pengpengdd.cyou/gtntztnffx.html

Py:   Counter(arr)
来源：http://hz.jinqigufen.top/gthiilring.html

PHP:  array_count_values($arr);
来源：http://hz.hammf.cn/gtlurekrac.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jyoumei.cn/gtyfvozhrr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhoulong.xyz/gtvzvbbqnr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.c1oappe.top/gtycfflujd.html

Go:   // 手写 map[T]int
来源：http://hz.jianghu66.top/gtymnegxlv.html

Ruby: arr.tally
来源：http://hz.redwolf501.top/gtjcfqpynr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.9152youxi.cn/gtniwxuwnv.html

[D21] 判断是否包含某元素
来源：http://hz.cucudq.cn/gtzqtkzyba.html

Py:   x in arr
来源：http://hz.yvedp.cn/gtjmdodjjj.html


<!-- 参考信息 -->