代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://hz.ywan-chungtsiang.top/gtrzmhallx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gtobxbpluc.html

C#:   f(a: 1, b: 2)
来源：http://hz.jqgfzy.top/gteymipoyr.html

[C05] 返回多个值
来源：http://hz.tanke756.top/gtbccnwhru.html

Py:   return a, b
来源：http://hz.ydjk.org.cn/gtdztnyefv.html

PHP:  return [$a, $b];
来源：http://hz.tianlin.xyz/gtlkonwsle.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zdqjudy.top/gtixxwdnjk.html

TS:   return { a, b };
来源：http://hz.jinghuilouyu.cn/gtpzebnaik.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gogol.net.cn/gtqgoryndx.html

Go:   return a, b
来源：http://hz.jyoumei.cn/gtveiwnity.html

Ruby: return a, b
来源：http://hz.mhx1999.top/gtkeinijxe.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sxryk.cn/gtrvmvdmjs.html

[C06] 匿名函数 / lambda
来源：http://hz.gotoacloud.top/gtlgafuxrc.html

Py:   square = lambda x: x * x
来源：http://hz.wangdashe.top/gtrdhgjjej.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yuxming.cn/gtxzmhjysc.html

JS:   const square = x => x * x;
来源：http://hz.guannengcc.top/gthuqmmakl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.mhx1999.top/gtgyxgtset.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gotoacloud.top/gtyuqwxpcd.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gogol.net.cn/gtxbyepali.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cdnleiting.top/gtpmqlxvzg.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sweek.top/gtokiactdk.html

[C07] 把函数作为参数传入
来源：http://hz.xuetiantiany.cn/gtvlyinlnr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yueranfly.top/gtvwnzsqty.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.meibo888.top/gtdyxwrsvh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dashuyun.cn/gtgimpieby.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangtech.top/gtmxopnvet.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xingfuxueyuan.xyz/gtxhiquyxl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yuxming.cn/gtdnsztjia.html

Ruby: arr.map(&:upcase)
来源：http://hz.feifeiyinyue.top/gtsyiusavn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gzhubu.top/gtnhuphaeh.html

[C08] 闭包
来源：http://hz.nanxuanxn.top/gtzwrzslez.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hfpthk.cn/gtojnccwjz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.mhx1999.top/gtanlwlfbu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.sufxvd.cn/gtctbbkoie.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jianghu66.top/gttdblyukm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.feifeiyinyue.top/gtsusoueut.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yonumen.top/gtpftrdypl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhixingplan.top/gthwgkatma.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xylfe.cn/gtizwczqnh.html

[C09] 递归
来源：http://hz.nanxuanxn.top/gtnjmpjhdf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ywan-chungtsiang.top/gtfumqewcs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jlsjyb.cn/gtygscvemd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hywenlv.cn/gthadbvvoj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258.top/gthtcwjvfo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.316326.xyz/gtwqfurohn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.smart0.xyz/gtzvxzlrrj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhixingplan.top/gtmecxfpkw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.iojbl.cn/gtzryxospu.html

[C10] 变量作用域
来源：http://hz.yueranfly.top/gtuztvvcao.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sweek.top/gtuehxwkhh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cqqwz.cn/gtgffwxpuo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.daxiang520.top/gtguvgccld.html

TS:   同 JS
来源：http://hz.jqgufenzy.top/gtqzbisdoe.html

Java: 方法内为块级作用域
来源：http://hz.52xcode.cn/gtoxifphpx.html

Go:   花括号块级作用域
来源：http://hz.birdmap.top/gtigqqaiof.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xinyue.icu/gtklcozrdo.html

C#:   块级作用域
来源：http://hz.sufxvd.cn/gtbelzbnlc.html

[C11] 模块导入与导出
来源：http://hz.yvedp.cn/gtxtdtptmc.html

Py:   from module import func
来源：http://hz.dianchejie.cn/gtlpshiflk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.wangdashe.top/gtecqstmkq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.316326.xyz/gtbkqqzqwx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tanke756.top/gttlvklczv.html

Java: import java.util.List;
来源：http://hz.jlsjyb.cn/gtiibsmsxh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.svipenyu.cn/gthcyqfnyo.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ehwqpu.com/gtgrdacnlp.html

C#:   using System.Text;
来源：http://hz.ywan-chungtsiang.top/gtgbegoulr.html

[C12] 立即执行函数 IIFE
来源：http://hz.yanxiufei.cn/gtcvnvmgrp.html

Py:   (lambda: print("run"))()
来源：http://hz.chenlongwang.top/gtdhmlmfxt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.52xcode.cn/gthcfelkth.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydjk.org.cn/gtiocflcqq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yangfankeji.com/gtskcyxund.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.316326.xyz/gtnieosbfl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shangyingyoupin.top/gtufegdyri.html

Ruby: -> { puts "run" }.call
来源：http://hz.guannengcc.top/gtfxsrtmph.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hfpthk.cn/gtxrctnhuj.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuetiantiany.cn/gtsjmmjsqm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jlsjyb.cn/gtwbnxqcoj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jiagoushi.top/gtkmacxvum.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jqgufenzy.top/gtkhgrshmw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hywenlv.cn/gtbpwnpbui.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gtoqosuwww.html

Go:   func add(a, b int) int
来源：http://hz.sysykeji.top/gtaptgmjwn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.c1oappe.top/gtynfshuzn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xuanzx.com/gtfhexqeit.html

[C14] 泛型函数
来源：http://hz.jyoumei.cn/gtmskwxsev.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ywan-chungtsiang.top/gtaymcftns.html

PHP:  // 无泛型
来源：http://hz.chenjidiqi.icu/gtvhklprut.html

JS:   // 无泛型
来源：http://hz.316326.xyz/gtnporpuxh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cashguo.top/gtximxxiox.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhixingplan.top/gtvbwqarsh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.aizwys.cn/gtwbqvcmbu.html

Ruby: # 无泛型
来源：http://hz.daria6918.cn/gtjnpplced.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuanzhike.top/gtutwudlao.html

[C15] 解构 / 展开参数
来源：http://hz.pycfn.com/gtnimzqrzf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.meibo888.top/gtxxlzkuaf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.mhx1999.top/gttpdrnqtd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yongpay.top/gtvkdxwckc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.svipenyu.cn/gtkcaqzuez.html

Java: // 无解构
来源：http://hz.sufxvd.cn/gtokjoxcxi.html

Go:   // 无解构
来源：http://hz.vqdsnc.cn/gtglppvwgj.html

Ruby: a, b = pair
来源：http://hz.hammf.cn/gtynmpvtao.html

C#:   var (a, b) = pair;
来源：http://hz.guannengcc.top/gtxuvpeeww.html

[C16] 函数 / 方法重载
来源：http://hz.xingfuxueyuan.xyz/gtkdxwrcgm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yuxming.cn/gtfyqojyau.html

PHP:  // 无重载
来源：http://hz.tianlin.xyz/gtbtsjqagc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinyuanbaomall.cn/gtxcucfgml.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jianghu66.top/gtqrzwngcl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jyoumei.cn/gtboohwmng.html

Go:   // 无重载：用不同函数名
来源：http://hz.yangfankeji.com/gtrucxdakt.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhijiandao.cn/gtayhuazgc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ybcxt.top/gtvtwgqunk.html

================================================================================
来源：http://hz.birdmap.top/gtpojasqds.html

D. 数组 / 列表 / 集合
来源：http://hz.jlsjyb.cn/gtsvyuylil.html

================================================================================
来源：http://hz.sxryk.cn/gttslzliyh.html

[D01] 创建数组 / 列表
来源：http://hz.ybcxt.top/gtxtrxsjfj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.meibo888.top/gtmtikpfdm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guannengcc.top/gtkzvtwgfs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guannengcc.top/gtfhpjocey.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.redwolf501.top/gtrwpteqbk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.52xcode.cn/gtxrumirsl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhixingplan.top/gtbvyajcoc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jyoumei.cn/gtmianxmin.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.316326.xyz/gtzhvyuxwt.html

[D02] 追加元素到末尾
来源：http://hz.shanyushiyangtech.top/gtgkodlwwc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhijiandao.cn/gtcaiwqngg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinghuilouyu.cn/gtohxkfxno.html

JS:   arr.push(4);
来源：http://hz.zhijiandao.cn/gtzllfyolm.html

TS:   arr.push(4);
来源：http://hz.sufxvd.cn/gtwqqqgzus.html

Java: list.add(4);
来源：http://hz.yuxming.cn/gtbbhbuvwu.html

Go:   arr = append(arr, 4)
来源：http://hz.smart0.xyz/gtoixnyorq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhijiandao.cn/gtbcobexmb.html

C#:   list.Add(4);
来源：http://hz.sxryk.cn/gtyanpulgw.html

[D03] 在指定位置插入元素
来源：http://hz.sufxvd.cn/gtxadzeucj.html

Py:   arr.insert(0, 0)
来源：http://hz.shuidangran.top/gthyncetmm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jlsjyb.cn/gtsxenhhrk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yuanzhike.top/gtahqeybxr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yj20258.top/gtjmqszwzu.html

Java: list.add(0, 0);
来源：http://hz.316326.xyz/gtvnloylui.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.tianlin.xyz/gtuijybwmt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zdqjudy.top/gtgvjygonh.html

C#:   list.Insert(0, 0);
来源：http://hz.cqqwz.cn/gtugbyxenq.html

[D04] 删除元素
来源：http://hz.yvedp.cn/gtsckkhomo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.0kj1m.cn/gthdyzulhc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhongyouzk.top/gtlwlkpufo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xinyue.icu/gtdbwcamgu.html

TS:   arr.splice(0, 1);
来源：http://hz.daria6918.cn/gtahrsicdp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sweek.top/gtqyvjfwgd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jinqigfzy.top/gtvwpbuyla.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuetiantiany.cn/gtlwkkhnpr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.redwolf501.top/gtmvxyswiv.html

[D05] 访问与修改元素
来源：http://hz.jinghuilouyu.cn/gthtitvamf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.bjfxy.top/gtyamtwzpa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.9152youxi.cn/gttpjdcvqk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hongshengwenyu.top/gtvdwcmgec.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.aizwys.cn/gtndmengdf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ppjwa.cn/gteuosxfsv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.fengsongda.top/gtuhnkuxbp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jlsjyb.cn/gtltopfglc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.guowangkeji.top/gtvxazuowp.html

[D06] 数组长度
来源：http://hz.sufxvd.cn/gtdgovtljp.html

Py:   len(arr)
来源：http://hz.gzhubu.top/gttchktexw.html

PHP:  count($arr);
来源：http://hz.yuanzhike.top/gtfoamesvm.html

JS:   arr.length
来源：http://hz.yongpay.top/gtzymeicck.html

TS:   arr.length
来源：http://hz.zycfv.cn/gtwtqnbmeb.html

Java: list.size();
来源：http://hz.cqqwz.cn/gtdjasqjcz.html

Go:   len(arr)
来源：http://hz.jqgufenzy.top/gtxlcbwcxw.html

Ruby: arr.length; arr.size
来源：http://hz.zhongyouzk.top/gtbspzymcc.html

C#:   list.Count;
来源：http://hz.shanyushiyangtech.top/gthhymzamv.html

[D07] 切片 / 取子数组
来源：http://hz.zhiwuduotai.top/gtsbilpuls.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yj20258.top/gtajpaxhde.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jqgfzy.top/gtgmtwkkdp.html

JS:   arr.slice(1, 4);
来源：http://hz.pycfn.com/gtqyrsiqlu.html

TS:   arr.slice(1, 4);
来源：http://hz.hnxiangtu.top/gtpkwfxevm.html

Java: list.subList(1, 4);
来源：http://hz.zhongyouzk.top/gtdnzcmjho.html

Go:   arr[1:4]
来源：http://hz.wangshuangyany.cn/gtqwhgabuq.html

Ruby: arr[1, 3]
来源：http://hz.haohaochexian.top/gtgefzjjtx.html

C#:   list.GetRange(1, 3);
来源：http://hz.yvedp.cn/gtxibajkuv.html

[D08] 合并两个数组
来源：http://hz.sufxvd.cn/gtepugkgeq.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhijiandao.cn/gtcawunakm.html

PHP:  array_merge($a, $b);
来源：http://hz.kuanghao11.cn/gticjnogjw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shuidangran.top/gtbcsuvxcy.html

TS:   [...a, ...b];
来源：http://hz.cashguo.top/gtytbqkhal.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ydjk.org.cn/gtxbsjlkzw.html

Go:   append(a, b...)
来源：http://hz.cucudq.cn/gtxiijxike.html

Ruby: a + b;  a.concat(b)
来源：http://hz.wangdashe.top/gtsosettou.html

C#:   a.Concat(b).ToList()
来源：http://hz.52xcode.cn/gtbkxgmxeg.html

[D09] 排序（升序）
来源：http://hz.cucudq.cn/gtzzpfawws.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhoulong.xyz/gtplfrmomm.html

PHP:  sort($arr);
来源：http://hz.chenzaomai.com/gttazguttm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.aizwys.cn/gtkljmdihw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gotoacloud.top/gtotwnqvnf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zdqjudy.top/gtmsfrhxwi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.pycfn.com/gttlytdlfe.html

Ruby: arr.sort
来源：http://hz.zhijiandao.cn/gtizwgzbro.html

C#:   list.Sort();
来源：http://hz.jianghu66.top/gtzgilrylz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ydjk.org.cn/gtwrxxgdfl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ydjk.org.cn/gtaoeyadkv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hywenlv.cn/gttedrvgxf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fengsongda.top/gtxaqqkace.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenzaomai.com/gtobyfzrou.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jlsjyb.cn/gtlzicqfur.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xylfe.cn/gthgzrfmxf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cqqwz.cn/gtvpeldqei.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.guannengcc.top/gttvctjuzq.html

[D11] 反转数组
来源：http://hz.daria6918.cn/gtnkdsowij.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.pycfn.com/gtfwyqvzrx.html

PHP:  array_reverse($arr);
来源：http://hz.mhx1999.top/gtotfbpyjy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ehwqpu.com/gtrjdxbsro.html

TS:   [...arr].reverse();
来源：http://hz.zhijiandao.cn/gtatvczwyx.html

Java: Collections.reverse(list);
来源：http://hz.jinqigufen.top/gtwsfkvkkf.html

Go:   slices.Reverse(arr)
来源：http://hz.hywenlv.cn/gtzsgpncsz.html

Ruby: arr.reverse
来源：http://hz.tianlin.xyz/gtlyjdvyuc.html

C#:   list.Reverse();
来源：http://hz.sufxvd.cn/gtqraxgwvp.html

[D12] 查找元素下标
来源：http://hz.shuidangran.top/gtwgocitcs.html

Py:   arr.index(x);  x in arr
来源：http://hz.yongpay.top/gtyfisbeti.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.wangshuangyany.cn/gtjafezpcv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.c1oappe.top/gteeookxes.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zdqjudy.top/gtoaxrhedo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuanzx.com/gtznrciptg.html

Go:   slices.Index(arr, x)
来源：http://hz.hongshengwenyu.top/gtngixzluj.html

Ruby: arr.index(x)
来源：http://hz.xingfuxueyuan.xyz/gtivfrqxoc.html

C#:   list.IndexOf(x);
来源：http://hz.sxryk.cn/gtvbrkxkhj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhijiandao.cn/gtwhftaqts.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhiwuduotai.top/gtajjkleso.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhixingplan.top/gtaiobezbp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.birdmap.top/gtproicelg.html

TS:   arr.filter(x => x > 3)
来源：http://hz.52xcode.cn/gtjjksvhbl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinqigfzy.top/gtvqkvrcoh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.fzhhl.top/gtrkaqwnvz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yangfankeji.com/gtmltoqmrf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shuidangran.top/gtgrqfdscj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.daxiang520.top/gtakysryrc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shuidangran.top/gtpocckqaz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.kuanghao11.cn/gtqexnzhdm.html

JS:   arr.map(x => x * 2)
来源：http://hz.shuidangran.top/gtbjwavukv.html

TS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gtwftzfjnc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tanke756.top/gtweozjtlw.html

Go:   // 手写循环
来源：http://hz.chenzaomai.com/gtxclbepnx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yvedp.cn/gtwsnxsvjj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shuidangran.top/gtzjfywcxj.html

[D15] 去重
来源：http://hz.guannengcc.top/gtcexpuefo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xziqi.cn/gtilqzpvkg.html

PHP:  array_unique($arr);
来源：http://hz.hysaishi.cn/gtfuqyujpc.html

JS:   [...new Set(arr)]
来源：http://hz.snrcjt.cn/gtumeixwbl.html

TS:   [...new Set(arr)]
来源：http://hz.yj202588.top/gtlurvbhuq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.fengsongda.top/gtcvtlywti.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.guannengcc.top/gtktjsedlp.html

Ruby: arr.uniq
来源：http://hz.ydjk.org.cn/gtolaziiiz.html

C#:   list.Distinct().ToList()
来源：http://hz.nanxinkj.top/gtmtdubfvy.html

[D16] 求和与平均值
来源：http://hz.meibo888.top/gtewsxfbil.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuxming.cn/gtmvtgktga.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxuanxn.top/gtamifxtwc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtlqzwrctq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtusilfdea.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nanxinkj.top/gtvhhrwvkc.html

Go:   // 手写循环累加
来源：http://hz.guowangkeji.top/gtqwpauofp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.nanxuanxn.top/gttmuqkazk.html

C#:   list.Sum();  list.Average()
来源：http://hz.xuanzx.com/gtcqadeycl.html

[D17] 最大值与最小值
来源：http://hz.chenzaomai.com/gtnemjfaye.html

Py:   max(arr);  min(arr)
来源：http://hz.vqdsnc.cn/gtsryngsne.html

PHP:  max($arr);  min($arr);
来源：http://hz.hnqzz.top/gtzapdvirj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hongshengwenyu.top/gtwbfmjipk.html

TS:   Math.max(...arr);
来源：http://hz.jyoumei.cn/gtqkhguhwc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yanxiufei.cn/gtbmyqfsny.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shuidangran.top/gttkakeulu.html

Ruby: arr.max;  arr.min
来源：http://hz.fengsongda.top/gtgxvaeejm.html

C#:   list.Max();  list.Min()
来源：http://hz.xinyue.icu/gtdqgzpcrd.html

[D18] 扁平化嵌套数组
来源：http://hz.jinqigufen.top/gtwqbgvfcq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cashguo.top/gtxzxxatqc.html

PHP:  array_merge(...$nested);
来源：http://hz.cdnleiting.top/gtwkzkrpvp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gaohongyu789.top/gtfcypypzs.html

TS:   nested.flat();
来源：http://hz.quarkkingdee.top/gtvksffhrb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jqgufenzy.top/gtdqcpenne.html

Go:   // 手写双层循环
来源：http://hz.tian-w.cn/gtogpumaxb.html

Ruby: nested.flatten
来源：http://hz.snrcjt.cn/gtxqbegqga.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yonumen.top/gtnxxtbjzs.html

[D19] 按字段分组
来源：http://hz.yj20258888.top/gtbuksylfa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.redwolf501.top/gtmopgeekt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hongshengwenyu.top/gtazyblwor.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.havefunace.top/gtlktkvzln.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ppjwa.cn/gtsgiknhlr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jiagoushi.top/gtkittajnp.html

Go:   // 手写 map[string][]T
来源：http://hz.gogol.net.cn/gtldbgzpps.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ydjk.org.cn/gttxwrlsff.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cheryme.top/gtygmblyuc.html

[D20] 统计每个元素出现次数
来源：http://hz.sysykeji.top/gthidpecgj.html

Py:   Counter(arr)
来源：http://hz.ivvv.top/gterwbfbly.html

PHP:  array_count_values($arr);
来源：http://hz.ybcxt.top/gtwppnycri.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gaohongyu789.top/gtksanrcad.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sysykeji.top/gteitvixye.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jlsjyb.cn/gtvnkqasrk.html

Go:   // 手写 map[T]int
来源：http://hz.sweek.top/gtaijruqkj.html

Ruby: arr.tally
来源：http://hz.kuanghao11.cn/gtpdkkpddo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenjidiqi.icu/gteavmvzyv.html

[D21] 判断是否包含某元素
来源：http://hz.jianghu66.top/gtpbxblvqp.html

Py:   x in arr
来源：http://hz.jqgufenzy.top/gtkilloegj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.quarkkingdee.top/gtzplilacd.html

JS:   arr.includes(x)
来源：http://hz.birdmap.top/gttcsxfmxr.html

TS:   arr.includes(x)
来源：http://hz.yonumen.top/gtpzymwedp.html

Java: list.contains(x)
来源：http://hz.xingfuxueyuan.xyz/gttrohpsfb.html


<!-- 参考信息 -->