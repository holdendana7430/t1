代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://hz.mhx1999.top/gtbsrqtibu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ppjwa.cn/gtrxsadzqw.html

C#:   f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtgbfgtwvy.html

[C05] 返回多个值
来源：http://hz.ydjk.org.cn/gtlaqzrdnv.html

Py:   return a, b
来源：http://hz.snrcjt.cn/gtsglknmwq.html

PHP:  return [$a, $b];
来源：http://hz.meibo888.top/gtwjescocf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jinyuanbaomall.cn/gtlpeyjlmu.html

TS:   return { a, b };
来源：http://hz.dianchejie.cn/gtdnwnfenr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.smart0.xyz/gtasqicqnc.html

Go:   return a, b
来源：http://hz.gotoacloud.top/gtaurcapyh.html

Ruby: return a, b
来源：http://hz.yonumen.top/gtfvvfbazi.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dashuyun.cn/gtwbhvfgbx.html

[C06] 匿名函数 / lambda
来源：http://hz.cashguo.top/gtlduhyihn.html

Py:   square = lambda x: x * x
来源：http://hz.hammf.cn/gtjvnakfaf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yonumen.top/gtigzvesih.html

JS:   const square = x => x * x;
来源：http://hz.cucudq.cn/gtipdqwxei.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yueranfly.top/gtczixienc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sysykeji.top/gtvyxkqjwp.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.havefunace.top/gtgihhmmkh.html

Ruby: square = ->(x) { x * x }
来源：http://hz.smart0.xyz/gtuihfputc.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhaomingkeji.xyz/gtjburvmpv.html

[C07] 把函数作为参数传入
来源：http://hz.hywenlv.cn/gthiocidlf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jqgufenzy.top/gtiytonvwe.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jlsjyb.cn/gtarbvpuwb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dashuyun.cn/gtpjsbjkbf.html

TS:   arr.map(String)
来源：http://hz.wangshuangyany.cn/gtbofgqlft.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yj202588.top/gtggwyrpzo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.c1oappe.top/gtwkaphxub.html

Ruby: arr.map(&:upcase)
来源：http://hz.havefunace.top/gtnljesqaw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xinyue.icu/gteyutzsyh.html

[C08] 闭包
来源：http://hz.yonumen.top/gtlercshuh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yuanzhike.top/gteshdjiaz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ivvv.top/gtfgbfyqkl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.daria6918.cn/gtrvbucwrt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gtzrmoqoik.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.guannengcc.top/gttmzsfzyd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.snrcjt.cn/gtqqghuadi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xingfuxueyuan.xyz/gtqybcaifv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gturqccfcj.html

[C09] 递归
来源：http://hz.ydzc1.top/gttuqosick.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jlsjyb.cn/gtwucpwbwm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shanyushiyangtech.top/gthhtkuota.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yangfankeji.com/gthkatewqj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.0kj1m.cn/gtzuiygotf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cheryme.top/gtdnluwmeo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.aizwys.cn/gtflhxdgxp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.snrcjt.cn/gtfejewgyy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hfpthk.cn/gtnzmdsglp.html

[C10] 变量作用域
来源：http://hz.hammf.cn/gtufllasxj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.quarkkingdee.top/gtmriljaip.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tianlin.xyz/gtmstvwtaz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinyuanbaomall.cn/gtuaaeapjc.html

TS:   同 JS
来源：http://hz.cheryme.top/gtkimwranx.html

Java: 方法内为块级作用域
来源：http://hz.hammf.cn/gtsetwyfrl.html

Go:   花括号块级作用域
来源：http://hz.sufxvd.cn/gtqfogysjs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ydzc1.top/gtqjvlabrm.html

C#:   块级作用域
来源：http://hz.c1oappe.top/gtqttgfxhh.html

[C11] 模块导入与导出
来源：http://hz.yj20258.top/gtvwucwbxu.html

Py:   from module import func
来源：http://hz.yangfankeji.com/gtgrqmwlkn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.chenjidiqi.icu/gtwzxrabki.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.dashuyun.cn/gtroknocan.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shanyushiyangtech.top/gtnvwzuekg.html

Java: import java.util.List;
来源：http://hz.sweek.top/gtrlgjswik.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhixingplan.top/gtutqdgukg.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.tanke756.top/gtowqrjvpi.html

C#:   using System.Text;
来源：http://hz.0kj1m.cn/gtuqlziuqm.html

[C12] 立即执行函数 IIFE
来源：http://hz.sufxvd.cn/gtuhzzynkk.html

Py:   (lambda: print("run"))()
来源：http://hz.jlsjyb.cn/gtevbwmdfm.html

PHP:  (function () { echo "run"; })();
来源：http://hz.9152youxi.cn/gthpkxmtqk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydjk.org.cn/gttinocvlp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.wangdashe.top/gtohfgdyir.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sysykeji.top/gtxgakoemc.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cashguo.top/gtfzzyubdp.html

Ruby: -> { puts "run" }.call
来源：http://hz.svipenyu.cn/gtbefebfds.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj20258888.top/gtnmhozpkz.html

[C13] 类型声明 / 类型注解
来源：http://hz.zdqjudy.top/gtgcqjtybq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.c1oappe.top/gtnwkymyyz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgufenzy.top/gtsjcdnclb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.redwolf501.top/gtxeejvsns.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zdqjudy.top/gtpacunloj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gttrjuaabi.html

Go:   func add(a, b int) int
来源：http://hz.havefunace.top/gtrejfqnii.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zycfv.cn/gtupijlifg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yueranfly.top/gtcxvkzstq.html

[C14] 泛型函数
来源：http://hz.gaohongyu789.top/gtxlomhjbi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yongpay.top/gtmtyikaiu.html

PHP:  // 无泛型
来源：http://hz.ivvv.top/gtuehibxlt.html

JS:   // 无泛型
来源：http://hz.daria6918.cn/gtiyojlvsf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yanxiufei.cn/gtiubiysso.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yangfankeji.com/gtvjxoqztu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shuidangran.top/gtycaznnne.html

Ruby: # 无泛型
来源：http://hz.jinghuilouyu.cn/gtabpjjovd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shangyingyoupin.top/gtrceyimed.html

[C15] 解构 / 展开参数
来源：http://hz.gotoacloud.top/gtskuzxrak.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yueranfly.top/gtfkxsdggy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gogol.net.cn/gtxttgxhko.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.chenjidiqi.icu/gttlgyvbzj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xuanzx.com/gtqwcdhjtq.html

Java: // 无解构
来源：http://hz.hammf.cn/gtxvxwvawr.html

Go:   // 无解构
来源：http://hz.zhoulong.xyz/gtfxkysxsp.html

Ruby: a, b = pair
来源：http://hz.tianlin.xyz/gtfhgvzplx.html

C#:   var (a, b) = pair;
来源：http://hz.ywan-chungtsiang.top/gtuwjwesxv.html

[C16] 函数 / 方法重载
来源：http://hz.zhongyouzk.top/gtkugagvnt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hongshengwenyu.top/gtzsxzldtx.html

PHP:  // 无重载
来源：http://hz.jyoumei.cn/gtvzyrktup.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.bjfxy.top/gtlmxweqmw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhongyouzk.top/gtwpatuzgo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hfpthk.cn/gtrezxrexd.html

Go:   // 无重载：用不同函数名
来源：http://hz.cqqwz.cn/gtwmusygxf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.mhx1999.top/gtmcxahqqa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ywan-chungtsiang.top/gtddpanxid.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtpuwduzoz.html

D. 数组 / 列表 / 集合
来源：http://hz.fengsongda.top/gtcvgqutoi.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtbcctardv.html

[D01] 创建数组 / 列表
来源：http://hz.0kj1m.cn/gtqmbeecaz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ydzc1.top/gtgnyluurq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guowangkeji.top/gthrmbipub.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aizwys.cn/gtblbfaacd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hongshengwenyu.top/gtbrhshbst.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sysykeji.top/gtnupvjngn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ivvv.top/gtljdthbvy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj202588.top/gtglxtvpfn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhoulong.xyz/gtwjebbhvn.html

[D02] 追加元素到末尾
来源：http://hz.yuanzhike.top/gtzbkkglig.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ivvv.top/gtxdvsfzjo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.guannengcc.top/gtmqhsljrh.html

JS:   arr.push(4);
来源：http://hz.ybcxt.top/gtbgkeezoj.html

TS:   arr.push(4);
来源：http://hz.jiagoushi.top/gtrfghxavx.html

Java: list.add(4);
来源：http://hz.sufxvd.cn/gtoakvecye.html

Go:   arr = append(arr, 4)
来源：http://hz.9152youxi.cn/gtoefzxaly.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yongpay.top/gtbauirinm.html

C#:   list.Add(4);
来源：http://hz.yj202588.top/gtwcjbspwe.html

[D03] 在指定位置插入元素
来源：http://hz.nanxinkj.top/gtsbizrnyw.html

Py:   arr.insert(0, 0)
来源：http://hz.gotoacloud.top/gtnwubvrzf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.havefunace.top/gtyptqcesc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.nanxinkj.top/gtvwqhvmqr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.0kj1m.cn/gtzluwhapf.html

Java: list.add(0, 0);
来源：http://hz.dashuyun.cn/gtcwamlgtk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fengsongda.top/gthxbfqyhf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.0kj1m.cn/gthqrdqtlr.html

C#:   list.Insert(0, 0);
来源：http://hz.hysaishi.cn/gtounjcfub.html

[D04] 删除元素
来源：http://hz.dianchejie.cn/gtfgjqfcrk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhixingplan.top/gtdekidmgg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hfpthk.cn/gtbvymqmql.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zycfv.cn/gthoqlkmqw.html

TS:   arr.splice(0, 1);
来源：http://hz.zhoulong.xyz/gtkxkznloy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hywenlv.cn/gtkyjyesfo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.birdmap.top/gtjzvptaoq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangkeji.top/gtgdodheqp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.meibo888.top/gtgyrbqrzb.html

[D05] 访问与修改元素
来源：http://hz.xziqi.cn/gtlqjatzyd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtlstafvhl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinghuilouyu.cn/gtgdwwryen.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sysykeji.top/gtcukfvlkp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shanyushiyangtech.top/gtiwrqatlz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shangyingyoupin.top/gtswtrpfxa.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sweek.top/gtbiueotkf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shzxlz.cn/gtvvbgrysg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ivvv.top/gtermvxfbz.html

[D06] 数组长度
来源：http://hz.nwbrower.top/gtymmiyhac.html

Py:   len(arr)
来源：http://hz.fengsongda.top/gtkdlnrhyk.html

PHP:  count($arr);
来源：http://hz.mhx1999.top/gttdqznasz.html

JS:   arr.length
来源：http://hz.pycfn.com/gtkyulqzso.html

TS:   arr.length
来源：http://hz.yuxming.cn/gtzlrcbwlx.html

Java: list.size();
来源：http://hz.nanxuanxn.top/gtqmqxgtju.html

Go:   len(arr)
来源：http://hz.shzxlz.cn/gtmbyeqovy.html

Ruby: arr.length; arr.size
来源：http://hz.yvedp.cn/gtanaxbndr.html

C#:   list.Count;
来源：http://hz.meibo888.top/gtpkwnmnaz.html

[D07] 切片 / 取子数组
来源：http://hz.jinqigfzy.top/gtekfkwwmt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nanxinkj.top/gttgmndxkt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.guannengcc.top/gtmlcsuitr.html

JS:   arr.slice(1, 4);
来源：http://hz.jianghu66.top/gtroxjprgq.html

TS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gtbrvkmehr.html

Java: list.subList(1, 4);
来源：http://hz.zhengqikj.top/gtueftnumo.html

Go:   arr[1:4]
来源：http://hz.redwolf501.top/gtwjskjkdm.html

Ruby: arr[1, 3]
来源：http://hz.xuetiantiany.cn/gtzyifgzoh.html

C#:   list.GetRange(1, 3);
来源：http://hz.xuanzx.com/gtrbcrwqrf.html

[D08] 合并两个数组
来源：http://hz.pengpengdd.cyou/gthqpbvgrh.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinqigufen.top/gtuzoovimq.html

PHP:  array_merge($a, $b);
来源：http://hz.yuxming.cn/gtynqgfmhz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.kuanghao11.cn/gtjsqxbvrv.html

TS:   [...a, ...b];
来源：http://hz.quarkkingdee.top/gthuqytsvr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.redwolf501.top/gtuhaijcoy.html

Go:   append(a, b...)
来源：http://hz.jinghuilouyu.cn/gthfnixpyd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.guannengcc.top/gtjhrkiqun.html

C#:   a.Concat(b).ToList()
来源：http://hz.shanyushiyangkeji.top/gtpwhcvhvp.html

[D09] 排序（升序）
来源：http://hz.ivvv.top/gtgwieemjp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yueranfly.top/gtyauorliu.html

PHP:  sort($arr);
来源：http://hz.gaohongyu789.top/gtyehtmlel.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.c1oappe.top/gtqfrtfzpm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sweek.top/gtajohrmdt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sysykeji.top/gtfsnvxgre.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fzhhl.top/gtarptyhqc.html

Ruby: arr.sort
来源：http://hz.yonumen.top/gtbyvcfrbe.html

C#:   list.Sort();
来源：http://hz.yongpay.top/gtkkjelagl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.c1oappe.top/gtvzgldpnm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jinqigufen.top/gteolapmig.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258888.top/gtnflaxylm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hywenlv.cn/gtykhwphha.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cucudq.cn/gtorqhejka.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jianghu66.top/gtatiiiyjp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenjidiqi.icu/gtyuyvduth.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nanxinkj.top/gtscrtaomr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhengqikj.top/gtpnulnntv.html

[D11] 反转数组
来源：http://hz.yj202588.top/gtwnifusbl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.andypj.xyz/gtudypotzq.html

PHP:  array_reverse($arr);
来源：http://hz.yueranfly.top/gtpvlqhfow.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gogol.net.cn/gtcypaysgn.html

TS:   [...arr].reverse();
来源：http://hz.cqqwz.cn/gtnwuqxlae.html

Java: Collections.reverse(list);
来源：http://hz.chenjidiqi.icu/gtzjozdatd.html

Go:   slices.Reverse(arr)
来源：http://hz.hnxiangtu.top/gtzmyipvlc.html

Ruby: arr.reverse
来源：http://hz.xingfuxueyuan.xyz/gtubeodtqi.html

C#:   list.Reverse();
来源：http://hz.sxryk.cn/gtxganwgjc.html

[D12] 查找元素下标
来源：http://hz.nanxinkj.top/gtrovnsiqo.html

Py:   arr.index(x);  x in arr
来源：http://hz.bjfxy.top/gtjpphoikv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinyuanbaomall.cn/gtdjqzepwh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.iojbl.cn/gtwqkjbdwv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.9152youxi.cn/gtughekuok.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhoulong.xyz/gtodptdhpw.html

Go:   slices.Index(arr, x)
来源：http://hz.shzxlz.cn/gtcuivooek.html

Ruby: arr.index(x)
来源：http://hz.sxryk.cn/gtbussjpos.html

C#:   list.IndexOf(x);
来源：http://hz.nanxuanxn.top/gtqzjnknxr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hysaishi.cn/gtpexcdezh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gotoacloud.top/gtujlhibuj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cdnleiting.top/gtaedgmqdz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.52xcode.cn/gtadvlskiy.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gthmoqocpq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zycfv.cn/gtnpkwdagw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xylfe.cn/gtxzffuneu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yj20258.top/gtllbaycnj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinqigufen.top/gtrnbsmkih.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yanxiufei.cn/gtrkdtcavj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gaohongyu789.top/gttfuvreid.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hysaishi.cn/gtvztmnadd.html

JS:   arr.map(x => x * 2)
来源：http://hz.cqqwz.cn/gtzkxqdkji.html

TS:   arr.map(x => x * 2)
来源：http://hz.sufxvd.cn/gthcxsfflk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yvedp.cn/gtxblayowv.html

Go:   // 手写循环
来源：http://hz.andypj.xyz/gtdyjmaxvd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shzxlz.cn/gtvpozlpgg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhijiandao.cn/gtypafnraj.html

[D15] 去重
来源：http://hz.yj202588.top/gthegwwtfs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cucudq.cn/gtovntetgq.html

PHP:  array_unique($arr);
来源：http://hz.jinyuanbaomall.cn/gtituiscfn.html

JS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtuhamkhnl.html

TS:   [...new Set(arr)]
来源：http://hz.ywan-chungtsiang.top/gtfmgtswiy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guowangkeji.top/gtnhpalvpa.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cucudq.cn/gtamzorrvp.html

Ruby: arr.uniq
来源：http://hz.hnxiangtu.top/gtxtyvxxfc.html

C#:   list.Distinct().ToList()
来源：http://hz.jinghuilouyu.cn/gtqfrnrmdz.html

[D16] 求和与平均值
来源：http://hz.0kj1m.cn/gtsfvccwuh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj202588.top/gtdjzusodc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yueranfly.top/gtufemmzfw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cqqwz.cn/gtkbkygfzc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jianghu66.top/gtxqnpoltc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenjidiqi.icu/gtswplbhcv.html

Go:   // 手写循环累加
来源：http://hz.havefunace.top/gtxmiqbvuj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.pycfn.com/gtyjknniow.html

C#:   list.Sum();  list.Average()
来源：http://hz.xziqi.cn/gtlyueckca.html

[D17] 最大值与最小值
来源：http://hz.zhiwuduotai.top/gtsebpygoq.html

Py:   max(arr);  min(arr)
来源：http://hz.jinghuilouyu.cn/gtwykjolyi.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxinkj.top/gtmmgglncv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.meibo888.top/gtlsoqzkwc.html

TS:   Math.max(...arr);
来源：http://hz.yangfankeji.com/gtnuijxppa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.quarkkingdee.top/gtpshoeovc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangdashe.top/gtltafjzsk.html

Ruby: arr.max;  arr.min
来源：http://hz.yuxming.cn/gtwzmysxmq.html

C#:   list.Max();  list.Min()
来源：http://hz.yonumen.top/gtxpnpkmut.html

[D18] 扁平化嵌套数组
来源：http://hz.cqqwz.cn/gtlheddyvx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj20258888.top/gtvbbyxqih.html

PHP:  array_merge(...$nested);
来源：http://hz.jyoumei.cn/gtfxdgpdeu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.feifeiyinyue.top/gtwdoxwmqs.html

TS:   nested.flat();
来源：http://hz.jqgufenzy.top/gtqmyuqycm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nwbrower.top/gtmttjepdm.html

Go:   // 手写双层循环
来源：http://hz.hysaishi.cn/gttntvwsmd.html

Ruby: nested.flatten
来源：http://hz.cashguo.top/gtjnqrvypa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.0kj1m.cn/gtxnsdbxyc.html

[D19] 按字段分组
来源：http://hz.yueranfly.top/gtviyrqlxj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.tianlin.xyz/gtzcdqysnz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhengqikj.top/gtmgrgcpjy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daxiang520.top/gtatxxcgya.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinghuilouyu.cn/gtmxslfxol.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hywenlv.cn/gtyititdrd.html

Go:   // 手写 map[string][]T
来源：http://hz.chenzaomai.com/gtcaxyefrj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shanyushiyangkeji.top/gtlshrwmvd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.pycfn.com/gtqledjnjr.html

[D20] 统计每个元素出现次数
来源：http://hz.yongpay.top/gtxtejvkfw.html

Py:   Counter(arr)
来源：http://hz.jinqigfzy.top/gtrkwlmaft.html

PHP:  array_count_values($arr);
来源：http://hz.redwolf501.top/gtuwbnmgiz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.haohaochexian.top/gtosjhzqqd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fengsongda.top/gtjewjkwij.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhijiandao.cn/gtsbmtjvfu.html

Go:   // 手写 map[T]int
来源：http://hz.birdmap.top/gttlrilyyg.html

Ruby: arr.tally
来源：http://hz.yvedp.cn/gtwrycytwc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ybcxt.top/gtvymbgaxg.html

[D21] 判断是否包含某元素
来源：http://hz.chenjidiqi.icu/gtdrwurivl.html

Py:   x in arr
来源：http://hz.pengpengdd.cyou/gtswkjzsjq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sweek.top/gtxclmznps.html

JS:   arr.includes(x)
来源：http://hz.zhaomingkeji.xyz/gtdgnolpwh.html

TS:   arr.includes(x)
来源：http://hz.c1oappe.top/gtzpakcmmd.html

Java: list.contains(x)
来源：http://hz.pycfn.com/gtkgdwgxkx.html


<!-- 参考信息 -->